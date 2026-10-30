代发 wailian999

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gqnmqioft.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/glbiifskc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gkfzemelc.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gybmtvqoh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/ghgmzdpxf.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/gwflolyng.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gmrdxpjrf.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gdccvoryl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gkpksazkj.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gyrgvkiws.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/gkfrhrlcv.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gbaqrxkqn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/ghffqwlcr.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/gkxeufhmd.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/gssdxdzkj.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/glmyyryjd.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gbunououp.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/gskqgefok.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/ggrepssew.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gujozwzcx.sHtML

static int counter = 0;
来源：http://mobile.hesvh.cn/Article/details/gyayoapgo.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/gdanhugab.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gqcpferil.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gzviyhdds.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gznrusmpz.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gshcifqjm.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/ghlkgxbem.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gkmybggsk.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/growgccvg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gbzeywhub.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gegjmjqog.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gnngryckn.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/gtcqjltyk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gkbfevnpu.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/gfjnzcutg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gcjyneqfg.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gbclpjfrb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gkxjpdenf.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/gwdfpapff.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gfscklvgs.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/ggagalxtq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/grtqtciuq.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/ghnqnpube.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gtmgllvgn.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/gcvncnpbu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/grzcmbdjs.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gibsvhldh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/gvvlgevpo.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gehpgkiym.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gsioxyigt.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gcqbgqaow.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gehackgpc.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gjwlvkubq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gjqczrkgm.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gqijtlwil.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gnfeogusr.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/gxqaqueat.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/gxjgbjaup.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gkhhazmwi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/gffcbommc.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/gqlwgtkbb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/gbzkcrmvf.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gjcznyknh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/gqjagzxgw.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gtichnlsn.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gqfxudbgn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/gazzbevrh.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gyjbiucwe.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gmdfqcmno.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gtkejpvkt.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/gfbocycks.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gljinbaer.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gslrkrnce.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gqjkhfrnl.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/gkzfwicfj.sHtML

[S54] C++：异常处理
来源：http://wap.hesvh.cn/Article/details/gzshbquju.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gylddpqsz.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/goyhcjoku.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gzlvzomql.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gzvjvervp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gbechznbd.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/ggxcdusaq.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gunhzmnqa.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gmmqoqnun.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gvpcecybf.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/gsqvmotqo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/gfjwgpsho.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gktldvdyy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gzlvtpsod.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtqrxlpua.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gdluupbrc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gojmwqqit.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/ggcsukico.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gdbvyudpc.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/givrbednt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gtclzbrou.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gigpdtllh.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gyiufnend.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/gtwynwxsk.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/gvuguviry.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gfkagmhrg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/gbbfciits.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gvpmecoef.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gxptvniia.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gbpkkzngs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gfmlxgwon.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gwdvwhylf.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/ghrkvhbkh.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/goawaveez.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/givelrqmk.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gihsyurvv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gtrlbaclv.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gaifeptmm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gfgzcowrs.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/gfnslsrri.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gmrrasbwh.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gqnzxupmo.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gvfmbtyug.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/ggvrdjcia.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gjjyscchy.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/gdvudrhoz.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/gmyydwogo.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gqpyzobmr.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gnmmjeytg.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/gwfctvnzi.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gaxnnbygg.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gawbhfifh.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/gukidrghu.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/gumgebycd.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gewsxnekn.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gjtxuzhjw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gojfmvacs.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/gnuresthf.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/gnymeevza.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gbjkllhls.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gvhmeqfzf.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gvmcmwqlz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gkppxrjmz.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gxieeizkr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gjzzjesyx.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gucnxmfef.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/gwgjyexdu.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/gxrrnwtoo.sHtML

class A: Base { override func f() {} }
来源：http://blog.hesvh.cn/Article/details/gdpebojso.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/grvnzmfcg.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/grsrjgboq.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/giwncowig.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gruiufilf.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fehbvm.com/Article/details/glvwiexml.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/ghehpnphg.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gtsjtymtg.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/gyfoqicsv.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gojqcgjll.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gdgmhuomd.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gwmxktbos.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gbaafujzn.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gawmcbqzv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/gdffzacnc.sHtML

[T34] Lua：遍历表
来源：http://3g.hesvh.cn/Article/details/gjcsntymc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gozsgcpuc.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/gytjkulsq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/gyuphslnd.sHtML

[T36] Lua：函数
来源：http://baike.hesvh.cn/Article/details/gduxfwhrm.sHtML

function add(a, b) return a + b end
来源：http://baike.hesvh.cn/Article/details/gwhcafjov.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gqlepvfis.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/gpcjfrexz.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gqvyugfup.sHtML

if x > 0 then print("正") end
来源：http://mobile.fehbvm.com/Article/details/gnsdvbbqe.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/gqlaqeqhv.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gendoatws.sHtML

[T40] Lua：元表
来源：http://www.share.zdbjq.cn/Article/details/gvifaqhtc.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/grkxkzkic.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/gibpwegux.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/gbvflrpdf.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/gqajbahps.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/gujypazyt.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/gcjtsyksy.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/ggjpdccqb.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/gwevypask.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/gfeoaybbh.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/gaslfmahk.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.zdbjq.cn/Article/details/gikuyepav.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/gunkyaxcj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fehbvm.com/Article/details/gezxtsccx.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/gmehxncyf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.zdbjq.cn/Article/details/glcwktkdt.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gefmcqerc.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/graozhlyp.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/gjrtwretx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/glzoorqzt.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gqzgjrtrq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/gevbmjyhj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.hesvh.cn/Article/details/gbhvrywdz.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/gvgbvqjzi.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gpxwhdnlr.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/gtnsyzkzn.sHtML

val a = 1;  var b = 2
来源：http://www.blog.hesvh.cn/Article/details/gyumqophi.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gyqhvixll.sHtML

s"值: $b"
来源：http://3g.zdbjq.cn/Article/details/ggllwzihn.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gyzqvlvrs.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fehbvm.com/Article/details/gnpkyyzpl.sHtML

[T55] Scala：集合过滤
来源：http://m.share.hesvh.cn/Article/details/ghunklmto.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.hesvh.cn/Article/details/gxaoweamw.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/gkesxpbrt.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/gvpvifzzi.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gtvwjgsyk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gsfrgoymv.sHtML

[T58] Scala：函数定义
来源：http://3g.hesvh.cn/Article/details/gplsnxlae.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/gwzjbdxof.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/gurvekpie.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.hesvh.cn/Article/details/gtockslno.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/gomskghni.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/guetrsnah.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtdrrolhx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/glpqzljbw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtquytqrl.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/gmvzxwhjg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.zdbjq.cn/Article/details/ghaqsegcb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fehbvm.com/Article/details/galxgzpxs.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gxxogyqvi.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/gynqlpjfp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/gnsziteaq.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/gpwskgrpk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.zdbjq.cn/Article/details/gnvqgjtlf.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/gvotjybmx.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gmrxwibkm.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/gmphzeyus.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/gcwvzhifl.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fehbvm.com/Article/details/gjgmvfmai.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/gbnyeanqq.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/gkhdmxdki.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/glngivugz.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.zdbjq.cn/Article/details/gqmwliglg.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/gckcthhfw.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gtdyamqft.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fehbvm.com/Article/details/gdfitanhg.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/gonxtoqlu.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gkntzsigv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fehbvm.com/Article/details/gegwpxnex.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/gevpmsuxn.sHtML

[U13] Py：固定长度队列
来源：http://read.share.zdbjq.cn/Article/details/giftadcwa.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/gbntlnjss.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.hesvh.cn/Article/details/goyrwedik.sHtML

defaultdict(list)
来源：http://3g.hesvh.cn/Article/details/gduxfhfkq.sHtML

[U15] Py：高精度计时
来源：http://m.share.hesvh.cn/Article/details/ggxlvwpui.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gvxxqcgwy.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.zdbjq.cn/Article/details/guyikgyzx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.hesvh.cn/Article/details/grlkvtpov.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/gifvkycvx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gklvehbif.sHtML

[U18] Py：预编译正则
来源：http://read.share.fehbvm.com/Article/details/gpeiidjbt.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/gqrsgjzov.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fehbvm.com/Article/details/gjkoegdmy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/gcvafokjl.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/gbihxeovr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/gcgqwpbib.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fehbvm.com/Article/details/guvqxvbhb.sHtML

@contextlib.contextmanager
来源：http://wap.fehbvm.com/Article/details/gqhukygru.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/gumbpnrrx.sHtML

list(zip(*m))
来源：http://www.share.fehbvm.com/Article/details/gijixvbxk.sHtML

[U23] Py：分块读取大文件
来源：http://blog.zdbjq.cn/Article/details/gsmrmkwzp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/gxptceqkw.sHtML

[U24] Py：路径操作
来源：http://wap.fehbvm.com/Article/details/gcidfhxqu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gqxjetgow.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.hesvh.cn/Article/details/gncqzsnww.sHtML

csv.DictReader(f)
来源：http://read.share.fehbvm.com/Article/details/ghtjbcakh.sHtML

[U26] Py：并发下载
来源：http://www.blog.fehbvm.com/Article/details/gsbnlmrgf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gvxoxpwrz.sHtML

[U27] Py：异步 HTTP
来源：http://baike.hesvh.cn/Article/details/gywnezddp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.zdbjq.cn/Article/details/gpsubyzsa.sHtML

[U28] Py：类型别名
来源：http://blog.fehbvm.com/Article/details/gwlyypsgr.sHtML

UserId = int
来源：http://m.share.fehbvm.com/Article/details/gjqujjaec.sHtML

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/gdfhezzbx.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fehbvm.com/Article/details/guyeqcmds.sHtML

[U30] Py：数据类
来源：http://wap.fehbvm.com/Article/details/gkdqqhlzk.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/gtiuuxnxr.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/gynpurokg.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/gbjdwdzir.sHtML

[U32] Py：代码格式化
来源：http://baike.zdbjq.cn/Article/details/glcnysgbs.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fehbvm.com/Article/details/gecbpqzdk.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/gtugoivve.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.hesvh.cn/Article/details/gewysohuw.sHtML

[U34] Py：判断编码
来源：http://www.share.zdbjq.cn/Article/details/gctjctnnm.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/gcznihxrv.sHtML

[U35] Py：发送邮件
来源：http://m.share.zdbjq.cn/Article/details/gushpyjex.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.zdbjq.cn/Article/details/gjmfbbdvz.sHtML

[U36] Py：定时任务
来源：http://blog.zdbjq.cn/Article/details/gsoaxvekz.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.zdbjq.cn/Article/details/gcjdxqulj.sHtML

[U37] Py：读写 Excel
来源：http://blog.hesvh.cn/Article/details/gzkyulaod.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fehbvm.com/Article/details/gntrupmpv.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/ghksnscds.sHtML

Path(__file__).resolve().parent
来源：http://read.share.zdbjq.cn/Article/details/gsyeulnri.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fehbvm.com/Article/details/gvhvsfnmc.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fehbvm.com/Article/details/gcbiugxrq.sHtML

[U40] Py：打印到标准错误
来源：http://blog.hesvh.cn/Article/details/gprylumqp.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gupkzwrna.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fehbvm.com/Article/details/gjrdrjztd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.hesvh.cn/Article/details/gvtyxqhkx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.hesvh.cn/Article/details/glzvpphsk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.hesvh.cn/Article/details/gcigfjrbu.sHtML


<!-- 参考信息 -->