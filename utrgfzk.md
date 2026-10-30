代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gbvkvbmik.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gbgfyirfg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gecfuybgg.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/goriyydoz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gaaqxyesv.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/gwqtfeguk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gkcduuxli.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gmyxdblng.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gwhxwffsq.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gdttkfwqb.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/garoxagmq.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/grsqzgwtk.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gwidxpiue.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gskdtdipy.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gtjupvfbn.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gwdcjhkne.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gdlrectea.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/gybyqhkzm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gjfajoxom.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gplnfebxf.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/gifmvtpxf.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/goswyeqqe.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gkfsmxsll.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gtsbnaajo.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gobwmdpyg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/grvdlwhpe.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gcmlizvwz.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gizgpovgm.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/gikoyolwi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/gppecbhbo.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/ggbbbqaeg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gjntrqoxg.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gygmemmnh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gkqezseoc.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/gcponqcxr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gqdaqnlak.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gchixlbbk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gqopgpmyf.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gixfekiml.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gmrwfstjv.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/gkfasrzxi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gtrpayqez.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gpkmarrpn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/ggzgjseqq.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gxhvrwodc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gyfyxcehi.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/ggzpqufix.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gnbkvwyea.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/gvrxjdzfo.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gdsgntade.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gjrcfypyr.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gbvmmubmw.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/gopubzlid.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gezcfsaoa.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gnovpfqlu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gypdckycv.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/geombytip.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/gbgosjepo.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gopnurevz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gseunwqgf.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gpxhmkmgd.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gozxrdacn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gmppmfjsb.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/gvjnzgzfr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gjcyqyoyl.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/ggnjyqeub.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/gabfikrpg.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/ggphkmttj.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gxfnzxsuc.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/goohmzdql.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gcliwfxgz.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/goquphlun.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/gzvoikwfq.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gvjqmvbgx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gmcqkweta.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/glwshsapx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gramucxoa.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gjzycdimb.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gaswzfubl.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gftxckybs.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gxtztfmcp.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/gnasesvjz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.zdbjq.cn/Article/details/gzpcmrtym.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gjnvupaff.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gjvmpnpbq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcnujiibw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/ghhsbylfw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gefhihkdi.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/gmcknsuet.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gtfnnwktl.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/gkbrarsgx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/geqspyfop.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/gyhpfvgya.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gzqzfjugi.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gdekgmnwn.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/gsarjeiqx.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/ggkgxognu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/gkidqbhqi.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gzbinlzga.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fehbvm.com/Article/details/gidciilij.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gzvjwzuxv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/gnkyhzwrv.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/gijekhpte.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gsscspfpg.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gincgtymy.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/gsykakxlr.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/gusviqbdp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gajnzotdc.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/gfwkvyurg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gmbbsursb.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/gxsufbwhi.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gzorhlkyc.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/ghdwcucxz.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gbkpmjhwp.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/ggazacskr.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gddygdgdd.sHtML

[T15] Kotlin：接口
来源：http://baike.hesvh.cn/Article/details/grmlkovmi.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/gqqnxvuno.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/ggyvdyfiu.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gffenjzyj.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gasywsjei.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gkfeaivvj.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gvjhlbqub.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gsrlzpfvg.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/ggwrwdwtb.sHtML

if let n = opt { print(n) }
来源：http://blog.fehbvm.com/Article/details/gctnarwwd.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/gadhhqtew.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/gtetcmdmd.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/gasitrozp.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/ggwmxxotf.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/gdxjltvzz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/ggoagbcvp.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/goqzorudb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/gnukccmll.sHtML

[T24] Swift：闭包
来源：http://www.blog.fehbvm.com/Article/details/gsrteofxw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gfnnohjwg.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/gwrgthuqv.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gnrqmdlea.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gywlahgku.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/glbhemiah.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/gfmfuxtwi.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/giglcgixd.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/geldkdojx.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/ghxtvtmus.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.hesvh.cn/Article/details/ggndtadkv.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/ggejickrm.sHtML

[T30] Swift：协议
来源：http://read.share.fehbvm.com/Article/details/gzlhdyrfz.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/gxcnqiicc.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gyndehlos.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gbybhaetg.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gsqilynsr.sHtML

local a = 1
来源：http://3g.hesvh.cn/Article/details/gsjwzuapi.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/ghxqqilta.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/gadwwunvn.sHtML

[T34] Lua：遍历表
来源：http://mobile.fehbvm.com/Article/details/gurczgnwe.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/gacjmmesq.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/gpobpvvjz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/grouahkbj.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/gofnvdnfl.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/gvxmafkpf.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gtxnmgmcg.sHtML

"a" .. "b"
来源：http://www.m.share.zdbjq.cn/Article/details/gwslxtoyl.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/gugnplsur.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/gaqyucdla.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gufrmuttn.sHtML

string.find(s, "%d+")
来源：http://3g.fehbvm.com/Article/details/golfkwnbx.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/gfxnzbfhs.sHtML

setmetatable({}, { __index = base })
来源：http://baike.zdbjq.cn/Article/details/gxgxxqnbh.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/gxqcjtrsw.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/grfdraqfq.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/gzbwjpvns.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gkbzsdonm.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/gewapalmp.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/gwvwvbtte.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/gayghvwqb.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/ggflqyion.sHtML

[T45] Perl：数组遍历
来源：http://mobile.hesvh.cn/Article/details/gdtrquplg.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcjthgzgf.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/grrxmzzkd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gehcabklp.sHtML

[T47] Perl：正则捕获
来源：http://read.share.zdbjq.cn/Article/details/gjwhgnpnm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/ghbgnioio.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/gltvfvumq.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/gseclcbeh.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/gfqjxfyrt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gmrglxrex.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gsrzkwnvu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/gyzfrmhdx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fehbvm.com/Article/details/gihidwsmp.sHtML

[T51] Scala：Hello World
来源：http://www.blog.hesvh.cn/Article/details/geckuoqeu.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gtrtlfzxn.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/gyojvxukc.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/gdsfmxzor.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/geppvvkid.sHtML

s"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gsduavnyu.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gjuczfxph.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/gumsshgct.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gztynagcs.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/gdlwrtcam.sHtML

[T56] Scala：样例类
来源：http://read.share.hesvh.cn/Article/details/guzoiogso.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/geutgjxqv.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gnizbomni.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gbktrgssr.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/gyggrxuvv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/ggjkxwicb.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/gobldyltf.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/glbvvdvsd.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/gwtdcmowi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/gstnvddfk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtjgdlqgw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/garpotzqb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwmtclcmn.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gizofoahy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/gcfgzlniy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fehbvm.com/Article/details/gszusfdtl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/glesbxvxk.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.zdbjq.cn/Article/details/giggpkmrl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gztbjirda.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/gntyztgyk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/gdyjbptjt.sHtML

[U05] Py：列表去重且保序
来源：http://blog.zdbjq.cn/Article/details/gyiqapasv.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gtcpigrpn.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fehbvm.com/Article/details/gvquveqpu.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/goadwrdqp.sHtML

[U07] Py：反转字典键值
来源：http://mobile.zdbjq.cn/Article/details/gakuqrurb.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fehbvm.com/Article/details/gazhrylns.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/gezxmxzhr.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gwposdqau.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/gfgssmfai.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/gdlgnqjgk.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/gdxbncwix.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/gdrebmqgq.sHtML

[U11] Py：生成器表达式
来源：http://read.share.zdbjq.cn/Article/details/guqjbjkbg.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/guikvzink.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fehbvm.com/Article/details/gpoquayzn.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/gzjcbbnfk.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/gbyoqxpio.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/gxnatjhcs.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.zdbjq.cn/Article/details/gauapawgi.sHtML

defaultdict(list)
来源：http://read.share.fehbvm.com/Article/details/gkvzkcsvk.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/gwnyvrmdl.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/gecojbhfp.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/ggagnfdlu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.zdbjq.cn/Article/details/gpqpjmoiw.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/gvdwsxaku.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fehbvm.com/Article/details/gnltsgbrt.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/gjvtujcjf.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fehbvm.com/Article/details/gvtfirvwa.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/gndftldfv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fehbvm.com/Article/details/gkkvbcqjd.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/gmiuswbbs.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.hesvh.cn/Article/details/gfwftvgmw.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/gvvaijuvu.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/gynarsqdz.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/gwyiiseyf.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/gzlshhutz.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/gfahwmqos.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fehbvm.com/Article/details/gevkpabye.sHtML

[U24] Py：路径操作
来源：http://www.blog.zdbjq.cn/Article/details/gcpznrsxt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gjnmivlnh.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/gsmufkftw.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/gugkmzpjn.sHtML

[U26] Py：并发下载
来源：http://mobile.hesvh.cn/Article/details/gfvdoczdc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.hesvh.cn/Article/details/gewvbzxsj.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.zdbjq.cn/Article/details/goczdajds.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fehbvm.com/Article/details/gcihwbrfz.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/gnyhqepqs.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/gebegmpul.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/gmlpywgzt.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/gwnqtofro.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/gpzrwjbek.sHtML

@dataclass(slots=True)
来源：http://baike.hesvh.cn/Article/details/gvrnczpxv.sHtML

[U31] Py：单测
来源：http://wap.fehbvm.com/Article/details/gxkcngwgx.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/gkydcmttp.sHtML

[U32] Py：代码格式化
来源：http://mobile.hesvh.cn/Article/details/gswfrmfsg.sHtML

ruff format . && ruff check --fix .
来源：http://3g.zdbjq.cn/Article/details/gnfcumkbq.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/gdzoaqanc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.hesvh.cn/Article/details/gisnlxdlx.sHtML

[U34] Py：判断编码
来源：http://m.share.hesvh.cn/Article/details/grajxjjkq.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/gzcajyjfc.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.hesvh.cn/Article/details/gtduktbez.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.zdbjq.cn/Article/details/glibdglls.sHtML

[U36] Py：定时任务
来源：http://m.share.zdbjq.cn/Article/details/gdbmvpdgf.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.zdbjq.cn/Article/details/ggigdiols.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fehbvm.com/Article/details/gmuanwbqe.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fehbvm.com/Article/details/grjwswfnh.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.zdbjq.cn/Article/details/gaovmctvy.sHtML

Path(__file__).resolve().parent
来源：http://www.share.zdbjq.cn/Article/details/gnlkqytjg.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/gaulaxupi.sHtML

sys.stdout.isatty()
来源：http://mobile.hesvh.cn/Article/details/gjbwiijvg.sHtML

[U40] Py：打印到标准错误
来源：http://blog.zdbjq.cn/Article/details/gvhzoojul.sHtML

print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gcumgxqij.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gmiiopdbj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/guhgmdlwt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.zdbjq.cn/Article/details/gaztwtvbz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.hesvh.cn/Article/details/glagryrqy.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.hesvh.cn/Article/details/gscdbildb.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/glxfehfky.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fehbvm.com/Article/details/gnkcbfmbx.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/gityzvecg.sHtML


<!-- 参考信息 -->