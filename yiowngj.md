代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gfvrstdrw.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/grckdudep.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gfqzuvnph.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gjjjdkukg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/gisxlgubz.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/grylfesoa.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gqkpfumlx.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/glndhigqb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gfeqgvibw.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gdapjseaa.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/gnxjzqvyz.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/gbwnqrocb.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gjlqptspc.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/glwwsddhi.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/ggzwasxhh.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gdhtwipve.sHtML

static int counter = 0;
来源：http://mobile.hesvh.cn/Article/details/gwhvxnagv.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gcbzemkay.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/gmkinzeod.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gavkjfrdy.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gkbdxrjiw.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/guptvosfs.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/gpeuxaumu.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/garpmckip.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gckvqekda.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gxdmgtmfi.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gfrlxlsuy.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/ghuxhjkzc.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gqhmxxfwe.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/gsotzmdxu.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gdeqnbnsb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gvugcgcuu.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/ghrosztnj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gxtgrsuer.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gcqgaffca.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/guhhxdtny.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gtybhrjlr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gsxgxakqb.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gdjjoxnml.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/gmgvxnikk.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gphnkxjae.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gpratfjvu.sHtML

[S40] C++：查找元素
来源：http://www.blog.fehbvm.com/Article/details/gmiuobcez.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gdidxgusf.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gyoggepcy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/gwbpkfzgf.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/grrnztwws.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/goslphizg.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gtublwgqt.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/geuenemjf.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/gwdbrgmrm.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gutujxism.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gvbinjxtg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/govyolgay.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/gbejswkbe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gbgvmtwjp.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/grmsgeqgs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gbojbovsf.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gsiirzdbm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gqfsxgwjl.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/gxxwxjcli.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gzqvkdfap.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/ghkwbiwpy.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gialofrtu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gynqtmgnt.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/glmnkgdbr.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/gbzxuwwef.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/gvyofossj.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gkmgdacsf.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gymandhij.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/gwppiuzjn.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/grhkmtlqp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gmtnhfpem.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/gerzmfcbc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/gxlzwpmts.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gyulscbqw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gjcrohyvo.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gtttkcycc.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/godikyhbk.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gfrjeyicw.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/guxcaocwa.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gkuhhxhuf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gxefesxnk.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gvrifavke.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gpvdfqvvr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gaeqvpcso.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gnshbmqrl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqvwhqppc.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gjgovpokv.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gzjateplv.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/goamnqtbg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gbswpgitt.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gicisedgy.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gagbuhgmj.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/ggaqltijb.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/gxxqqeedf.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gbmwqtphv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gmsnworiy.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gekbthshk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gokrnzgze.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gsyffafqe.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gmwpywott.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gnohtlocz.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gmirkoued.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gqevxubyt.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/glvajplvz.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gxrmuktki.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/guidpkjry.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gvyfbwxfx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gfsgnptlo.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/gqkaluxpb.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gzrdoctsi.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/gcdfpghnu.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmrvauifk.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/ggzygqecq.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gxpgaqvda.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/ggpzqfwle.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gleylrgma.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gecvbxmqx.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gznxfgrsn.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gjphgeafk.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/gatnaiiec.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/ggbmgfttv.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gjwtrvqzn.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/gbiynqiyu.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/gaxtyxzrp.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/glfpovqna.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/gmoepwdho.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/gmgvruvmb.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gyeglfozy.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/goriyvvbl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/gfudvznzs.sHtML

[T23] Swift：函数
来源：http://3g.zdbjq.cn/Article/details/gqbtkortw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gmjpukhze.sHtML

[T24] Swift：闭包
来源：http://read.share.zdbjq.cn/Article/details/gixebpzpg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/gvbximzts.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gwcimnamt.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gjjbjvgdu.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gjqzsihbz.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/gukhmafsc.sHtML

[T27] Swift：错误处理
来源：http://mobile.zdbjq.cn/Article/details/gbammasjd.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/guklxwvpc.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/gpaxyasgi.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/gwqijsfkz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gsgpwejlw.sHtML

guard let x = opt else { return }
来源：http://baike.zdbjq.cn/Article/details/ghtqujzyt.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gkuperyuf.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/gtwizrskv.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/genhllhdn.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gkohnwdub.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/ghzzgaakn.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gadzgqnsf.sHtML

[T33] Lua：表（数组）
来源：http://blog.fehbvm.com/Article/details/gryhetlss.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/ggeapgksf.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/ghadxyytq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/ghhurdwlk.sHtML

[T35] Lua：字典表
来源：http://blog.zdbjq.cn/Article/details/gjekudjqx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/gaxbchfhl.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/glexpntzr.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/giplgfhkb.sHtML

[T37] Lua：字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gfttikoid.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/gwpfbaxiy.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gvoutslpa.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/girrqcpoo.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/gsbtuhmxn.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/girahqtxh.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/ggocetocv.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/giuwaztvd.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/gpbmuvkbo.sHtML

print "Hello\n";
来源：http://3g.zdbjq.cn/Article/details/gcwrvfkhv.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gymojkkop.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/gwppsatvj.sHtML

[T43] Perl：字符串插值
来源：http://3g.hesvh.cn/Article/details/gffyeimdy.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/gdguiuzsq.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/gssbkilky.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gqjqkbtpa.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/gfniepodt.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/guzbjchyf.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/ggojlqzxt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/glqagdxqw.sHtML

[T47] Perl：正则捕获
来源：http://blog.zdbjq.cn/Article/details/gzmhqsgjq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/getlqqozb.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/gwwiwiash.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/glzsitwpf.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/gjoebrlpp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gyqxlghid.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gkayfqlxx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/gaxwawjqn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/gbkvgwzlc.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/glfxfnsor.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/geyuojinn.sHtML

[T52] Scala：变量
来源：http://www.blog.zdbjq.cn/Article/details/gflnigrkc.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gujylnveo.sHtML

[T53] Scala：字符串插值
来源：http://wap.fehbvm.com/Article/details/gewezyamj.sHtML

s"值: $b"
来源：http://wap.fehbvm.com/Article/details/gopyfmkfv.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gqgpipfqv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/gyviaznlr.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gercaerkz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/grumizyme.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/gvulbxdre.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gdvtkodtc.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gxjsxetpe.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/gppkdrtld.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/gegaqhbpi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fehbvm.com/Article/details/gyltthavi.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/getkiilrg.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gvsoraxet.sHtML

[T60] Scala：折叠
来源：http://baike.hesvh.cn/Article/details/gkftvtvee.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/grnupxasi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gecykuiqe.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gerkbaxgr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbzzzugsv.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fehbvm.com/Article/details/gpxkmcjen.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gslmfclrr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/geilkrsgw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/gmqpcsdil.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.hesvh.cn/Article/details/gjhhxdgpo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/gjgiakdvx.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/gxrisaiuh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.zdbjq.cn/Article/details/gajioxzfd.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.hesvh.cn/Article/details/gwotzmmga.sHtML

list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gznqfhpyb.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gizgwandg.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/grmtsezdk.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/gpzubzbwd.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/gigmlicwz.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gleggxhki.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/ghwxvddpl.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/gotezsbkn.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gseghwmlm.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/ghstinnaj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.hesvh.cn/Article/details/gpgatwndg.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/gdhugknia.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/goyrlkhva.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/gbwcsnirn.sHtML

Counter(arr).most_common(3)
来源：http://mobile.hesvh.cn/Article/details/gqxkhlsan.sHtML

[U13] Py：固定长度队列
来源：http://baike.hesvh.cn/Article/details/gnbdzlxfv.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gshfmsjoe.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fehbvm.com/Article/details/gapwqwavb.sHtML

defaultdict(list)
来源：http://wap.hesvh.cn/Article/details/gswstqajh.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/gkhcotjyi.sHtML

t = time.perf_counter()
来源：http://www.blog.fehbvm.com/Article/details/goumoyvqa.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fehbvm.com/Article/details/gnkmvvkre.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gsoujfoto.sHtML

[U17] Py：初始化日志
来源：http://mobile.zdbjq.cn/Article/details/gveqwiwlp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/gnxwypmvl.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/gswqvrrla.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/gzhwdmbev.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/gxxpquqez.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/glkysmwwk.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/gyxievzgw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.zdbjq.cn/Article/details/gmjovqmit.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/gwwjjumzs.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/gifpnvlek.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fehbvm.com/Article/details/gphggcnij.sHtML

list(zip(*m))
来源：http://www.share.fehbvm.com/Article/details/grmjygwpz.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fehbvm.com/Article/details/gemvbswxw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/gvzbaijgh.sHtML

[U24] Py：路径操作
来源：http://www.share.fehbvm.com/Article/details/gifvxjzff.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gzubhiphl.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/gvwuvrxpp.sHtML

csv.DictReader(f)
来源：http://read.share.hesvh.cn/Article/details/gkvvlqoax.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/girfaelsr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/glssrhhvj.sHtML

[U27] Py：异步 HTTP
来源：http://baike.zdbjq.cn/Article/details/grwgzroti.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.zdbjq.cn/Article/details/gxyoukynd.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/gutdzwdjb.sHtML

UserId = int
来源：http://wap.zdbjq.cn/Article/details/gmruydxcu.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/grnoagzds.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/gqhtpntjq.sHtML

[U30] Py：数据类
来源：http://baike.fehbvm.com/Article/details/glvmdgtas.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/gdukzaczw.sHtML

[U31] Py：单测
来源：http://mobile.zdbjq.cn/Article/details/guedluvvx.sHtML

python -m pytest -q
来源：http://3g.zdbjq.cn/Article/details/gsttotebe.sHtML

[U32] Py：代码格式化
来源：http://m.share.fehbvm.com/Article/details/glkozcoje.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fehbvm.com/Article/details/gflxbhiou.sHtML

[U33] Py：打包发布
来源：http://baike.zdbjq.cn/Article/details/gmezgcyuq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fehbvm.com/Article/details/gtjcnrcea.sHtML

[U34] Py：判断编码
来源：http://www.blog.fehbvm.com/Article/details/gtncdbpqr.sHtML

chardet.detect(raw)
来源：http://www.m.share.hesvh.cn/Article/details/gbkawkznb.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.hesvh.cn/Article/details/gpfoqwtts.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fehbvm.com/Article/details/gokcwwsrd.sHtML

[U36] Py：定时任务
来源：http://baike.hesvh.cn/Article/details/ghlhfcekq.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fehbvm.com/Article/details/grgtqnamf.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.zdbjq.cn/Article/details/gbnrkwuze.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/gktdcnrjd.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/gnomqabso.sHtML

Path(__file__).resolve().parent
来源：http://wap.zdbjq.cn/Article/details/gidleecxt.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fehbvm.com/Article/details/gmsudsfyh.sHtML

sys.stdout.isatty()
来源：http://www.blog.zdbjq.cn/Article/details/gksykrobo.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fehbvm.com/Article/details/gqodfxgyx.sHtML

print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gheknbhjh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.zdbjq.cn/Article/details/gthmkvfho.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/gpfprvcdx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.hesvh.cn/Article/details/gfuqxazoe.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.hesvh.cn/Article/details/gtughikmd.sHtML

[U43] PHP：声明命名空间
来源：http://baike.zdbjq.cn/Article/details/gfkmvizxa.sHtML

namespace App\Http;
来源：http://wap.hesvh.cn/Article/details/gagdlpkbj.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.zdbjq.cn/Article/details/gxyvmaawb.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/gxmkdvpow.sHtML


<!-- 参考信息 -->