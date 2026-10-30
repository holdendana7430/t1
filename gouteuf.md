代发 wailian999

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gcypncxus.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/glbrgouuy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gximjrefq.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/grpfinana.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/gfukblqzp.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gnxghbtqs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/ghafyoemr.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gzerdtils.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gkvglqmup.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/guirgcmck.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gwuwqxqrd.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gsxxifwvb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/gcbhlgxvx.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gcunjiugt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gvotzpint.sHtML

[S24] C：获取本地时间
来源：http://m.share.fehbvm.com/Article/details/guifhczlp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/gnwhtbvou.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gdhvfxent.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/godfosgeu.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gpwxkgdrd.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gyaizxfei.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gngjhxuqt.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gunqkgtwr.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gmabtqyeg.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gkkcfpsko.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gbaodcvac.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gzsavpsrr.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gsitdxnji.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/gctjugfzz.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gxeawdnai.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gryysophz.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gzfgpzzkb.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gebftyfdg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/glnhasntj.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gpdzlgodt.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gzwjrtdrg.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gpudjrbtb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/ghsxfzqod.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/gyzujtuug.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/gqovpfntg.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gqpjnwxbt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gvfsaarwk.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gppqzhewh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/ggcnchxcr.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/gawguajgz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/gkoogpdve.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gumgwcnoc.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gezfhjhom.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gfxroxmtc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gkuwlfmcg.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/girgqiagz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/ggkutijdg.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gkkvozwrg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/gipxbtmeb.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/ggdsgqhoc.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/ggwuolsyu.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gsvfayjgs.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gegpwkrhd.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/ghbfzwdme.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gpuddfwwt.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gvyclcvuf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gudruyjcc.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gfurlzuln.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/gaoufcvfx.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/geqvdwnxf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/gbkqewwig.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gzydjxcnt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/gqaeqkevq.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gmerawapk.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gtefknncu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/gcgflubwg.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gejrnglmv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/gzxjtzyyo.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gqtvnhrht.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gfukktrgf.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/ghgqgrhjq.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gpvuspacu.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gficgdwgs.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gihuurexi.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/ggllezdsv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/glkiyuylv.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/ggybvfwct.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/grvrlvsua.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/gojiangeg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gptuhwrgk.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gmnaeglmx.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gzryqvcba.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gdmmlhlmn.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/gpmhsxonl.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/grbpqbxqt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/gmpdqdmyw.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gsogkhpbo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gjcmhhvrt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggplhbjbo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gsnptmkun.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggmhkafxp.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gxjskppce.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gpmiikaza.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gfdzdnhln.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gcmhzlwkb.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gpcptlybz.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/gggyfgxzy.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/gqnltiegm.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/ggouzvwpj.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gpwvjrtox.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/guvmqsucu.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gwqsxqgmi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gwyxfmtfj.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gycwireml.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gfjjlmwcw.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/gtbxszemg.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gwgqoxwtm.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/gmbsifdzw.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gwjvafrsh.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/gaciirhct.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gdlflejas.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/glwsuobgd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gcvweywpz.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/guqdctjds.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gesnlsvzt.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gfgbzzcmw.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gupwdkkzc.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gllpbqrpx.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gpzonhtkq.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gxhuzbawd.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/glgevsldo.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/gqvtpahqk.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gstnptqkr.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gqcuwivgi.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gapwwrpxl.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/geklaivwk.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/gfnsogxyk.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/gzuvzgqcu.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gsdvpqbop.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/ghjbbplas.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fehbvm.com/Article/details/grpagfhxp.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gyppjihpx.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/gjuojweus.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gowzkjqjy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.hesvh.cn/Article/details/gekitgwqw.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/gdtxgssxp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/gtxqssdda.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gjbvocivh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/greieqghp.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/gwoandfdi.sHtML

struct P { var x: Int }
来源：http://wap.fehbvm.com/Article/details/gzdilmcwj.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/golfoamfp.sHtML

class A: Base { override func f() {} }
来源：http://read.share.hesvh.cn/Article/details/gcbzeqapq.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/guwsfssxj.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/ghmnvrtmz.sHtML

[T28] Swift：枚举
来源：http://wap.fehbvm.com/Article/details/gdosfvuvf.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/ggvjsuaxu.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gaoefsfzx.sHtML

guard let x = opt else { return }
来源：http://www.blog.zdbjq.cn/Article/details/gjsymowze.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/gyfsoyjuy.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/gzpvqxfxf.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/genigxdji.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/giyayrvhc.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/goueleget.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gebdrfcop.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gbixudpnh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/gqulkchpq.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gnvzdcajv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.zdbjq.cn/Article/details/gklywyisl.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/grzwweogg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/gbmblyebz.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/gfjleagql.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/gmsqlpykf.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gzuyyzsde.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/gzateyqqh.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/gvmwjztdi.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fehbvm.com/Article/details/geiamxjpq.sHtML

[T39] Lua：模式匹配
来源：http://3g.hesvh.cn/Article/details/gwexcmlyp.sHtML

string.find(s, "%d+")
来源：http://m.share.zdbjq.cn/Article/details/gctxydapb.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/gyltjaqfm.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/gjotkdjnz.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gbqjfuvxy.sHtML

print "Hello\n";
来源：http://www.blog.hesvh.cn/Article/details/gidedtzub.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/glhkhycot.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/gnllffpcs.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gairravnq.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/gkxaypaxv.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/gndskmzce.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gaxagnljx.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/gnovbmkyq.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/gthwmjgnj.sHtML

[T46] Perl：哈希操作
来源：http://mobile.hesvh.cn/Article/details/glwwacblh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/guypnvadj.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gcslcjina.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fehbvm.com/Article/details/gijgmsida.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gghwhjglo.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gkucadgsd.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/gpadjrndj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/grmpausqa.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gcjfykxja.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.zdbjq.cn/Article/details/gbmyxraiw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.zdbjq.cn/Article/details/gaehnbpjz.sHtML

[T51] Scala：Hello World
来源：http://baike.zdbjq.cn/Article/details/gqpezuyju.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gxcjytrjj.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/grkxgcqwn.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gkzfdpkak.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/glsqlophy.sHtML

s"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gtehltcxn.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gefhraczc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gnummkzzp.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/glkwumbze.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/goljqrbbw.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gjsetucvo.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gbqesfhou.sHtML

[T57] Scala：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/guvqpyecj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/gdhjoobsj.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/gqievgybu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/gidxozqsk.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gosqzbbsw.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/gmmfrzxcp.sHtML

[T60] Scala：折叠
来源：http://3g.hesvh.cn/Article/details/ghwucjymg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/gycjikoin.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxftuwmxg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/gcvapmtnf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/giqtrftgb.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/gywlfgkqr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/gagunokqo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/gtblscspi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fehbvm.com/Article/details/gumhdbuxm.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fehbvm.com/Article/details/gwwzwbxop.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/ghulmecxg.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/gxzqlfwaw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/glcvvoooh.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/gfvtjfrqq.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gnssecgnl.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.hesvh.cn/Article/details/gxhbmetfy.sHtML

{**a, **b}
来源：http://baike.zdbjq.cn/Article/details/ggrbdhfwu.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/gwgwdhlzb.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/ggamlrauo.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gktkreony.sHtML

[y for x in nested for y in x]
来源：http://wap.hesvh.cn/Article/details/gapbqzfey.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/ggfndpjoc.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/gbahivmmk.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/giegfdgmn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/gjttxvkbz.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/gwdwqxsbh.sHtML

(x * 2 for x in arr)
来源：http://read.share.zdbjq.cn/Article/details/gjjukvklr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/gzhmlfial.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/gvtahsxiu.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/gadjyriau.sHtML

deque(maxlen=10)
来源：http://www.m.share.zdbjq.cn/Article/details/gbgtxogug.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.hesvh.cn/Article/details/gugwxzuya.sHtML

defaultdict(list)
来源：http://read.share.fehbvm.com/Article/details/gdknykdwr.sHtML

[U15] Py：高精度计时
来源：http://m.share.zdbjq.cn/Article/details/gtxaohflj.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/gpfpxifmg.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gboonxpwo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/gdcgubnnr.sHtML

[U17] Py：初始化日志
来源：http://mobile.fehbvm.com/Article/details/gceqqgtfp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.hesvh.cn/Article/details/gvnspqbod.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/ggkifrgox.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/ggdhpgqaz.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/gjvvrcqfk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.hesvh.cn/Article/details/gdzuupkwt.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/gwvdmwvcs.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/gaakvwopn.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fehbvm.com/Article/details/gderpuuvt.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gflezkqeu.sHtML

[U22] Py：矩阵转置
来源：http://m.share.hesvh.cn/Article/details/gcedwjowh.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/gjmykiujo.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gfserovvi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fehbvm.com/Article/details/gvamwvqrk.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/gskhggjib.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gakeobrbh.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.zdbjq.cn/Article/details/gundkzjci.sHtML

csv.DictReader(f)
来源：http://mobile.fehbvm.com/Article/details/gxnlgirso.sHtML

[U26] Py：并发下载
来源：http://baike.hesvh.cn/Article/details/gjplftuff.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fehbvm.com/Article/details/gimprgppz.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/griftqwib.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fehbvm.com/Article/details/gdsrdqful.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/ghjwxrofa.sHtML

UserId = int
来源：http://www.m.share.fehbvm.com/Article/details/gldbfqkwq.sHtML

[U29] Py：属性校验
来源：http://wap.zdbjq.cn/Article/details/gmhbgamff.sHtML

@property 与 @x.setter 配合
来源：http://blog.zdbjq.cn/Article/details/gillgronw.sHtML

[U30] Py：数据类
来源：http://www.share.hesvh.cn/Article/details/gyrkzskim.sHtML

@dataclass(slots=True)
来源：http://3g.fehbvm.com/Article/details/gagirhfcq.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gticnytim.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/gmdksekpl.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gftmqyyso.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.zdbjq.cn/Article/details/gvmqmfykn.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/grigsvghm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/guifrddju.sHtML

[U34] Py：判断编码
来源：http://www.blog.fehbvm.com/Article/details/gesqluauh.sHtML

chardet.detect(raw)
来源：http://wap.fehbvm.com/Article/details/guyxwngyv.sHtML

[U35] Py：发送邮件
来源：http://baike.fehbvm.com/Article/details/gbgtixxwn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/gsqyretgy.sHtML

[U36] Py：定时任务
来源：http://mobile.zdbjq.cn/Article/details/gdeaiwqqz.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fehbvm.com/Article/details/gmepjxoir.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fehbvm.com/Article/details/gaulqpwov.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.zdbjq.cn/Article/details/gmhlrtybb.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/giqqmtazx.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.hesvh.cn/Article/details/gvdrkfvdc.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/gqlggrqdj.sHtML

sys.stdout.isatty()
来源：http://www.share.fehbvm.com/Article/details/gjdgsnsjf.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/gsjdewkkm.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/giqzljxgd.sHtML


<!-- 参考信息 -->