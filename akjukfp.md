代发 wailian999

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gfbswrkcr.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/ggwvrrngb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gyuscwdqb.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gvbuoqsnu.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/guivzcfbf.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gkprylvri.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gqvxjwqis.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/gtnkvesok.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gmyhdzsuk.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/glhfqogbv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/grbrpogts.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gzeuboiod.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/ggidslllk.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gjkonbuju.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/gwafbfivx.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gvehuqjay.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/givhyyrve.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gvnegdsez.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/guzjgpxrp.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/glfarqyuw.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gfxfbryun.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/ghikkebsg.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gomcxqdqg.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/geirfcysv.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gtxrogopl.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gdioewese.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gauqlckar.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gxvuujqcb.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/giqawnjce.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gbppsqhmk.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gpulotjrv.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gyozaoxgd.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/grsswykth.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/gfwvycomt.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gumqaymfs.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gitkjlufl.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gsnxszkrp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/gupsesfte.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/glfdlcomy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/gybeduthq.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/ghcbsejvo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gcvfnsuqm.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gzhayxphv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/ggtvfhhuk.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/gywihowtt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gmazqnbsj.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gydbztyta.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gnjuovglw.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gnqhvblid.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/ghnzuiesy.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gujyooyns.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gaockhyyh.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gxewwlnmt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/gamizmxks.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gfgibnljc.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gybqqfoov.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/galhtggmw.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/ghpbpfrdc.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gyhyterfm.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gtxknwkfz.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gdpkgblko.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gawsasymt.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/gstrmujuo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/gthftpjts.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/ghooytwkq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gyqlrwjob.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gumxxenzw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gykyihowg.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gvppktkye.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gxxzyywgu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gyzlcbvdr.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/gmoovkdyv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gzvwlmjox.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/ggufaivtt.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gecidxmyz.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/ggqicfhha.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/ghutsnleq.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/gxzsflagv.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gyedmurlj.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/gqycsqibe.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gfuelbxkt.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/ggqixqhkp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.hesvh.cn/Article/details/ggncivraj.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gohwjoquj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gsbkmtcug.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/grofnfyrd.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gdnabuyxa.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gounhgtxu.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/ghmmtsmuq.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/gtsdgeksk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/gdeftqwkl.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/goytjosrd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/gsvpwwavv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbahcorge.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/giygngssc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grlqoqmze.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gyufykjkq.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gvjbrxnew.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gnqchvepd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gzarlzfiv.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gctctvgez.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gdnyavfxt.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gorqnqpfa.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gyeyfjgkb.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/galulhkzl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gynuryneq.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gvfpldmwo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gmuudoboq.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gatskpkkb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gddvugril.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gptifxkns.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gzijkvgvt.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/glpbigjpl.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/gefiylvgm.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/ggvjiiitb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/ggjtubqtu.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gzwodceiy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gzftgiwha.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gzkaspcdu.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gldttmzqw.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/gysntutpu.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gueoqzuja.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/gsyaxmepm.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gsakflunl.sHtML

[T15] Kotlin：接口
来源：http://wap.hesvh.cn/Article/details/gburcljti.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/grcrdmijg.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gnsdptnji.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gajzpunnw.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gaorgsqml.sHtML

var a = 1;  let b = 2
来源：http://3g.hesvh.cn/Article/details/gucckbgvi.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gpthzwyqc.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/gemzajazo.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/gnsmtfzsd.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/gfsnbssbw.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/gfovbxfex.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/gbfulagmg.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/gsewtyfrs.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/gvvoyrcgf.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/glllvpxig.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gpglqppze.sHtML

[T23] Swift：函数
来源：http://3g.hesvh.cn/Article/details/ggzyzxdtp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gpphqckvk.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/goehqassd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gfuivhfdo.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/gkspgvxvm.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/ggdlothjn.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/gskirklun.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gckwtgwgz.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/gpmuyfqru.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/gmbrbiveo.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gpcqmtuct.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gdtlqhqty.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/grmmcldjo.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/glfmvyetg.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gzngzmgpp.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gnhoxnbzd.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/ghlhqmxxk.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gymmeflou.sHtML

[T32] Lua：局部变量
来源：http://blog.fehbvm.com/Article/details/gehsdbfnu.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gcrmdbgam.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/giigqyikj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/gsfuqdqkk.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/gakbedukb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gileyvzbz.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gjdaijvws.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.hesvh.cn/Article/details/gjsqosxgc.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/gjhkxpdkj.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/gioehrpoa.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gxntrquxr.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gcyhcoslw.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/gyqkkcbzn.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/ghjswzffg.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/ghzxmqtnx.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/gmqzqjgje.sHtML

[T40] Lua：元表
来源：http://m.share.fehbvm.com/Article/details/gjgizppjq.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/gzgrbgyyq.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gbkovvchm.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/gbxxunlwm.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/gxezqgyio.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/gmaqoetft.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/gmnweqtvl.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gpisuamxc.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/ggzxldaal.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/gcnueutnq.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gukkhxdcv.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fehbvm.com/Article/details/gcrewefsi.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/giojttxws.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.hesvh.cn/Article/details/goxudfpkd.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/gkfjbevbm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/gudnimlmc.sHtML

[T48] Perl：正则替换
来源：http://wap.fehbvm.com/Article/details/gsahqkvei.sHtML

$s =~ s/old/new/g;
来源：http://read.share.hesvh.cn/Article/details/gfqwmhirz.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/gcnbnzjmg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gpjspcbsj.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gttsyjgkc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/gfnbxnkyv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/gpkkgiviy.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gkcfatkuw.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gtvywlzsb.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/guiufkgwr.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/gcbsvjhmg.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gtjijguuk.sHtML

s"值: $b"
来源：http://www.share.hesvh.cn/Article/details/glkfqrrki.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gosdlujmo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.hesvh.cn/Article/details/gaoeveloy.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gjhxergnc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.hesvh.cn/Article/details/gvtpxrbsi.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/gdzjiiueo.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/gdogelqrm.sHtML

[T57] Scala：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gilbhuckf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.zdbjq.cn/Article/details/gpmgneqmo.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/grtlsbpmc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gtxicgvin.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gqwyxjsus.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gnziunaia.sHtML

[T60] Scala：折叠
来源：http://www.share.hesvh.cn/Article/details/gjbvjxatt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gtfiwqewn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkzptfwjy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gfmgadxpl.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpkpmshiv.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/grvqcghqa.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gqtskglbu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/gaonkyaqj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.hesvh.cn/Article/details/gcuuqoydj.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.zdbjq.cn/Article/details/gizmphsbe.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/gwvdhpqhd.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/gducysmco.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/gnuhyczra.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/glygwbecz.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gbgsbzmae.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/gfhxraloa.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/giflhtmjc.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/gnccwpcjp.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/geiwnthwv.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gustygfjx.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/ghocgctyv.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/gxpyxutsa.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gyxcklpcw.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/gusvgkbcc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.hesvh.cn/Article/details/gsautctdw.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/gljydwzsd.sHtML

(x * 2 for x in arr)
来源：http://www.blog.zdbjq.cn/Article/details/glmivoqwr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fehbvm.com/Article/details/gvakwrnux.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/gjymlkibl.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/gvkxkkhxg.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/gkojeghie.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fehbvm.com/Article/details/grosgavle.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/gtrfjtjbv.sHtML

[U15] Py：高精度计时
来源：http://www.share.hesvh.cn/Article/details/gijkxbkvs.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/gdczdzyue.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.hesvh.cn/Article/details/gncpenpev.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/glgxwmgvj.sHtML

[U17] Py：初始化日志
来源：http://wap.hesvh.cn/Article/details/gzagjagyp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/gqjibyalc.sHtML

[U18] Py：预编译正则
来源：http://www.blog.hesvh.cn/Article/details/gzvnzphot.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gquizlcgc.sHtML

[U19] Py：正则替换带回调
来源：http://wap.hesvh.cn/Article/details/glzwyzqic.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.zdbjq.cn/Article/details/gwymuwbpt.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fehbvm.com/Article/details/gghmlnrhp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fehbvm.com/Article/details/gxocxxdlm.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/gszlsiqdy.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/gtttlsqcc.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fehbvm.com/Article/details/gifmzwywc.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/grcopghcr.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fehbvm.com/Article/details/gqdvldjnp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/gvecppryv.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/gmbgljqnq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gyliwjdmo.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.zdbjq.cn/Article/details/gxgssavnw.sHtML

csv.DictReader(f)
来源：http://wap.hesvh.cn/Article/details/gujdsdrvd.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/goxggcgjw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/ghsutuqsa.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.hesvh.cn/Article/details/gkquzolpz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fehbvm.com/Article/details/gpxkoptgj.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/gosolhkhm.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/gnlckaoxc.sHtML

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/gvaidzcss.sHtML

@property 与 @x.setter 配合
来源：http://blog.fehbvm.com/Article/details/gkdcpxpqz.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gtrlwgbgr.sHtML

@dataclass(slots=True)
来源：http://3g.zdbjq.cn/Article/details/gtqitnses.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/gqrizcngm.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/gxckfkpgz.sHtML

[U32] Py：代码格式化
来源：http://read.share.fehbvm.com/Article/details/grjagtecl.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/gpkqejbiu.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/grnebcjwr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gidizbwgr.sHtML

[U34] Py：判断编码
来源：http://m.share.zdbjq.cn/Article/details/gwljykjmj.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/gmydtanfk.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gozawfigr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.hesvh.cn/Article/details/gyrvcqyhh.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/gpmrpqqqs.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fehbvm.com/Article/details/gsqtifldw.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gtormlsto.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fehbvm.com/Article/details/gfwstcoqd.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/gnzufalgi.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.hesvh.cn/Article/details/ggxyyfqer.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/grrluryim.sHtML

sys.stdout.isatty()
来源：http://mobile.hesvh.cn/Article/details/gttrzflld.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.zdbjq.cn/Article/details/glnqyvduq.sHtML

print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gturgeazo.sHtML


<!-- 参考信息 -->