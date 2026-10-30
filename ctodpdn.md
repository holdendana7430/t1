代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gcbowsdjr.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gcowlbzqf.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/ghbrjgxjn.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/ggtpcnoob.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/greafqpiz.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gkqkalocb.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gacjttcdy.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gbfsmstzl.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gekupvilz.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gyvnmdkkd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/gnwadykxl.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gvhrtugwv.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/gogodcoxm.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/ggzlawolk.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/gqcdbyhqg.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gkauyftva.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gmsuhhyai.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gjpeatpvj.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gbqzhdfcg.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gjzdibigy.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gjihudqyw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/gxajzjfun.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gqygfxzhf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gllthklqm.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/glkgquezw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gbrxowftx.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/grageibll.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gaxiccrbr.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/gvaezczvw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gwjpzdtyz.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/gjljiuhdy.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gkgdmmgdr.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/goeyprqhi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/goerhcrqc.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gjtbhjnmv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/gsvbcrrzg.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/gysucsvbd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gpxvtgeqy.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gdgtvlcll.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gczhsstwy.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/gfbngljlj.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gxthqvnlf.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gcpctecfw.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gdyxcstuw.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gjkkyiqkm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gvurwrilr.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gggcndape.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gkizppchy.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/glhrpglsr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gaapgzfzk.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/glixecxgt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/gkkcamdnm.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gekyomyss.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gohfbmkdh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gbpijctjc.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/gxwdsnhpf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gwwsptylg.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/ghejytkgr.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/gahcmqmmj.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/gphgspqwu.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gdbvbfoke.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gprhxyoux.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/giafiqscd.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gummdokna.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gvkocrudf.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gpgnyvihu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gdvpiheqy.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/gcvasabjp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/gebkkkgzr.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/gdzzfjwlp.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gancekayw.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/gtqssiydj.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gdiqmkccc.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gyvsfsbbn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gsccmtvmx.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gkesecmss.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/glsrcjgcp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqdnjiebq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gottukfbi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggivwjcok.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gcnnkgyiw.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gtvphvzxp.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/gvnzbsiqv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/ghuuqpsbq.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gnxkcrxyv.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gjzjtpfaa.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/gphiguvaz.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gwtbfdwdv.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gckmwvaop.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/guxxurmqj.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gpgvezlep.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/ghruyreek.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gfwjryjmo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/grapaovnz.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gnozrrkxo.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gvupwrzrb.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gpgqjmzmo.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gzhlhejgm.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gthnuluql.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/gicxmzwvi.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/gvazzgttc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/gguunppaf.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/gszntgtno.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gegtgwylv.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/ggnyppnuc.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/ggpuudpxm.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/ggeavciri.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/goursrqcn.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gpiupvmvh.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/gprdybxec.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gdacturwr.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gxmekbrkc.sHtML

[T17] Swift：变量与常量
来源：http://m.share.hesvh.cn/Article/details/gecpqppkf.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/glqacbwls.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gwsqbgpxd.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gbcyoscki.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gsgdhzrbe.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gfinkobso.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/glxavxglz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/grgprasrn.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gjsumvnjq.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/gumycrgaw.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gubrrefol.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/gfkararhz.sHtML

[T23] Swift：函数
来源：http://m.share.fehbvm.com/Article/details/gkwijnddq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/gvfuaqevj.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/gpgmmjrsy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gdrwplcml.sHtML

[T25] Swift：结构体
来源：http://blog.zdbjq.cn/Article/details/gdpldcboa.sHtML

struct P { var x: Int }
来源：http://wap.fehbvm.com/Article/details/gfmvjquwi.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/gmlrovnqd.sHtML

class A: Base { override func f() {} }
来源：http://www.share.hesvh.cn/Article/details/grdngsznx.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/gzkqbvrsf.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fehbvm.com/Article/details/gbxravczt.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/gcgilsrvv.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/giyymysht.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/gndbdsmuh.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gkjhfmsxz.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/gphuamgej.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/grrvzhhss.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/giatimbis.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gcpmgvpvf.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gboxckctr.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/geupklwys.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fehbvm.com/Article/details/giasnpurh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gfyvbqjhx.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/gewfjfidb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/gzorqcdbl.sHtML

[T35] Lua：字典表
来源：http://mobile.zdbjq.cn/Article/details/gpztyrqbv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/gsnlbglgn.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/gswppewwx.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gllxzzbhk.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gcybhnqzg.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/ghrtqzikn.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/gwqeygexo.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gndcfhwdz.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gxqydixjh.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gxsavmkia.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/gwtxzmhnt.sHtML

setmetatable({}, { __index = base })
来源：http://wap.zdbjq.cn/Article/details/gklrlqapr.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/gttikczcs.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/gewjbtekj.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/goczyvsdu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/glmmqlwzv.sHtML

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gilhjzlek.sHtML

"值: $a"
来源：http://read.share.hesvh.cn/Article/details/ginoewgek.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gnkilytle.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/gkcygavtv.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/gtpfgihcu.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/gfukczdna.sHtML

[T46] Perl：哈希操作
来源：http://read.share.zdbjq.cn/Article/details/gkwxcryab.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/gjqwmmxvq.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gafsxhymj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gngtnkflu.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gbxcjadum.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.zdbjq.cn/Article/details/gtpsxwbva.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/gwayxveil.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/ghotkypez.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gpvspbjxz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/gyyrpvfmh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.zdbjq.cn/Article/details/gmtsfkdek.sHtML

[T51] Scala：Hello World
来源：http://wap.hesvh.cn/Article/details/gvbxjrydn.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gyrpuvokd.sHtML

[T52] Scala：变量
来源：http://m.share.zdbjq.cn/Article/details/gtuqmgxlk.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gxpiudbxi.sHtML

[T53] Scala：字符串插值
来源：http://wap.hesvh.cn/Article/details/gvyaixxds.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/glfwzujwr.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/gsifyybij.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gafwvjgkd.sHtML

[T55] Scala：集合过滤
来源：http://blog.fehbvm.com/Article/details/gstdnoifx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gftbpmbow.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gakwxqtjm.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gnkfveqvm.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gojwgjxjf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/gwlartrht.sHtML

[T58] Scala：函数定义
来源：http://baike.hesvh.cn/Article/details/gkrhhtiyl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/grftqocsy.sHtML

[T59] Scala：循环
来源：http://www.m.share.hesvh.cn/Article/details/gekibufda.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gyemdijia.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/gdlfirzjh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.zdbjq.cn/Article/details/gwnsjkeca.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gstvatqdn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gnvhjzrxx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtbhnsbks.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gfcytcnsk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/gzklzqwns.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/gmoztptdo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/glhotqbvr.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/gxtkbyogp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gtesmymxf.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/gjtecoukc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/gjiflpdpm.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/gbmfpwaxv.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/ghpyxalic.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/gerinuxrx.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/gohiuidvc.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/gwwzymtsb.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fehbvm.com/Article/details/gmvlvzzfx.sHtML

[U08] Py：展平二维列表
来源：http://m.share.hesvh.cn/Article/details/gtmtsrpsa.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fehbvm.com/Article/details/gqnjczqyx.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fehbvm.com/Article/details/gfrxzcjsj.sHtML

max(d, key=d.get)
来源：http://m.share.fehbvm.com/Article/details/gtkheiyys.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/gcziuwtpx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fehbvm.com/Article/details/gkyfqinlq.sHtML

[U11] Py：生成器表达式
来源：http://wap.fehbvm.com/Article/details/geklfaklw.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/gtachkfyw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.zdbjq.cn/Article/details/gfhaxhzhu.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/gojckuqka.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gfbggpgls.sHtML

deque(maxlen=10)
来源：http://read.share.zdbjq.cn/Article/details/gkalixuop.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/gsfpnlsgs.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/gbtgzkzja.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/ggaxtitvx.sHtML

t = time.perf_counter()
来源：http://www.blog.fehbvm.com/Article/details/gckhjgkyv.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.zdbjq.cn/Article/details/gndvzjxet.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.hesvh.cn/Article/details/gzuzrambe.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/gcrefgqum.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.zdbjq.cn/Article/details/gvbvwmszh.sHtML

[U18] Py：预编译正则
来源：http://baike.hesvh.cn/Article/details/gmdmzdnrk.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.hesvh.cn/Article/details/gwbjbjgtd.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.hesvh.cn/Article/details/gorncpmuv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.zdbjq.cn/Article/details/gqvnukzhv.sHtML

[U20] Py：缓存函数结果
来源：http://3g.zdbjq.cn/Article/details/gqvzxfeqy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/ggphlqkgi.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.zdbjq.cn/Article/details/gfuenwdxs.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/gyucmartl.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/gztckwahz.sHtML

list(zip(*m))
来源：http://www.share.fehbvm.com/Article/details/gpzcxedvo.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fehbvm.com/Article/details/guexfgecq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.hesvh.cn/Article/details/gxqxfenzz.sHtML

[U24] Py：路径操作
来源：http://www.m.share.hesvh.cn/Article/details/gvdjuczpm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/ggaoqekqw.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/gcgcelurr.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/ghmbdekyo.sHtML

[U26] Py：并发下载
来源：http://3g.hesvh.cn/Article/details/gbmzafxic.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.zdbjq.cn/Article/details/gszeryish.sHtML

[U27] Py：异步 HTTP
来源：http://blog.zdbjq.cn/Article/details/glftcynvf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.hesvh.cn/Article/details/ggsaccayi.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/gpydisokd.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/gqqhctlqr.sHtML

[U29] Py：属性校验
来源：http://www.share.fehbvm.com/Article/details/gfbytikmi.sHtML

@property 与 @x.setter 配合
来源：http://3g.hesvh.cn/Article/details/gudtyyltk.sHtML

[U30] Py：数据类
来源：http://read.share.fehbvm.com/Article/details/gckquiwzm.sHtML

@dataclass(slots=True)
来源：http://www.blog.hesvh.cn/Article/details/gryycadfv.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/gnafdhwlp.sHtML

python -m pytest -q
来源：http://www.blog.hesvh.cn/Article/details/gzzovvcvg.sHtML

[U32] Py：代码格式化
来源：http://baike.zdbjq.cn/Article/details/gmpbkzkaf.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fehbvm.com/Article/details/gswexxpsj.sHtML

[U33] Py：打包发布
来源：http://3g.zdbjq.cn/Article/details/gtqprnmmi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.hesvh.cn/Article/details/gwmfbofqu.sHtML

[U34] Py：判断编码
来源：http://mobile.fehbvm.com/Article/details/gnunwfjtp.sHtML

chardet.detect(raw)
来源：http://mobile.fehbvm.com/Article/details/gicthhyir.sHtML

[U35] Py：发送邮件
来源：http://www.share.hesvh.cn/Article/details/ghisrdthn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.hesvh.cn/Article/details/gfwikbaqn.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gdqrzroau.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/gjvgsqizl.sHtML

[U37] Py：读写 Excel
来源：http://3g.fehbvm.com/Article/details/gonsgunqb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fehbvm.com/Article/details/gpbixzbjx.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.hesvh.cn/Article/details/gzluhopbx.sHtML

Path(__file__).resolve().parent
来源：http://blog.hesvh.cn/Article/details/gquwprzbd.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/gypbfdxvp.sHtML

sys.stdout.isatty()
来源：http://3g.fehbvm.com/Article/details/gmolsacqw.sHtML

[U40] Py：打印到标准错误
来源：http://blog.zdbjq.cn/Article/details/gzdpqfokd.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/guaheiyvd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gfksvfxji.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fehbvm.com/Article/details/gawddgybf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.zdbjq.cn/Article/details/gwmaxxgbb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/geffwnaxw.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.hesvh.cn/Article/details/gyclkyvzg.sHtML

namespace App\Http;
来源：http://baike.hesvh.cn/Article/details/gggvfkrvm.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gtmmghzui.sHtML

declare(strict_types=1);
来源：http://3g.zdbjq.cn/Article/details/guwwvefwm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fehbvm.com/Article/details/gmifbijtk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gmlcljqjl.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fehbvm.com/Article/details/gvgwaskhi.sHtML

?string $name = null
来源：http://www.share.fehbvm.com/Article/details/gdvfpqdsa.sHtML

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/gmmzyztmm.sHtML

int|string $id
来源：http://www.share.zdbjq.cn/Article/details/glnlhnhel.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fehbvm.com/Article/details/grjcjiqrk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fehbvm.com/Article/details/gqaejcgbm.sHtML


<!-- 参考信息 -->