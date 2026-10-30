代发 wailian999

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gomjthzen.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gacmwryuy.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gshanalmd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gboraoluv.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/gqpjluyfa.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gelsketjr.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gdywocrsp.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gpkqcdoom.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gtemilwzc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gvbvzewwx.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gxouieark.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gfhfwxuox.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/gvdmithqz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gpjqynrbk.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/grlqhrvns.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/ggvnfudlm.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gkchkhbib.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/grcukzxom.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gkqwjyfzt.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gyxjrjohb.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gpbrjesrd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gyytvuthr.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gwysfteov.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gredldytd.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gaywefmwi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gxaldnzwd.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/glbtimcjo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gqihsenkl.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/gytgonwta.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gmxcmtzht.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gwgohztkm.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gxhojglyx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gzpaywunt.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gkzgmhhht.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/goaurhyuk.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/ghamtyjso.sHtML

int size() const noexcept { return n_; }
来源：http://3g.hesvh.cn/Article/details/gxtgevnws.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/glcxzkfnm.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/guvkoxnnn.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gmxrhbhch.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gpeonilso.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/ggbyuvvnk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gqumripux.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gmadddgsq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/ghqtvfxsl.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gsmjwyaqk.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gnxabzdxl.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gidmuznoj.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gdqlinllm.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gwpwltnzz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/gjnvpnghv.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/gwcycmfxq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gnpfnpwaj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/garptjfxl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/glkgaeouu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gaptyiloc.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/ghxwbkykr.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gfmzsmmki.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/ghixzymsl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/gysefradm.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gyfhftzwy.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/govglwcgw.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/gblabhbnq.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/ggdutgotd.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/goglwgcdj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/gvwvsjror.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gacklkpxs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gqmobihbv.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gjpxknyql.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gbvqsqodh.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gotmheljo.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gxfwvcrep.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/ggxhhrvas.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/gyqzkcxhv.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/glxdxhaio.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gwrizdvpp.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/gamtmkpdk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/ghkdfzkyi.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gykbzlrmr.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/geztbzgha.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/gtahninie.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gkpncvcvp.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/gmnhgnmqt.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gpwultayz.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/gdbkgfyeu.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/gfvybnthi.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gopbqitbp.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gpgxodzwp.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gpntiuwfq.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/gryqbwgdb.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/guyvrpxoq.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/gjfxmkcgg.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gguyxwkvn.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/gbuwbgqzt.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gyavqwsys.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/gveiikcmq.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/gixrzpiaq.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/gehopvlli.sHtML

[T22] Swift：字典
来源：http://blog.fehbvm.com/Article/details/gmtqkxavr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/goiqprzge.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gvstrpxil.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/gvvdshzua.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gzlbnabki.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/ggnakfbcw.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/gyptmzguj.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/genzyuenv.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/gsuycrkgf.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/gcidwracz.sHtML

[T27] Swift：错误处理
来源：http://blog.zdbjq.cn/Article/details/gpllugygy.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/gyapkebbh.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gmkjzbzmc.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/grtucpnhi.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/gtxnihnww.sHtML

guard let x = opt else { return }
来源：http://3g.zdbjq.cn/Article/details/guzuwnluw.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gdrybvvky.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/gjedxmbbf.sHtML

[T31] Lua：Hello World
来源：http://blog.fehbvm.com/Article/details/gsaztzxwk.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gcaoyxeph.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gdkdynmro.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gxhqbrhwc.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gikffiqpj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/grsdvkdyy.sHtML

[T34] Lua：遍历表
来源：http://mobile.zdbjq.cn/Article/details/gjnlnsuqw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/gniztnltu.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/ggzzrwidt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/ggfiqiccd.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/guvjugtui.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/ghaztdekh.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gzjjftsaq.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/gflrrzflt.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/gatxksuxc.sHtML

if x > 0 then print("正") end
来源：http://www.share.zdbjq.cn/Article/details/gettkubkp.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/glljvoagf.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/ggzlxlycd.sHtML

[T40] Lua：元表
来源：http://blog.fehbvm.com/Article/details/gifmjrfwc.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gtbwgeoda.sHtML

[T41] Perl：Hello World
来源：http://wap.zdbjq.cn/Article/details/ggljepzax.sHtML

print "Hello\n";
来源：http://read.share.hesvh.cn/Article/details/gnnmznyjz.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gsgeepxkq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/gbwnnekrz.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gjmgwairv.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gillljggk.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/grtzconzr.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/ggvapheub.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gqdsicbjm.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/ggxunqrge.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/gsktffzpx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/gnaidpgxb.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gmwcyemzv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/gvxkqhswf.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gruarzncg.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/gwkdqxhzh.sHtML

[T49] Perl：函数
来源：http://www.blog.zdbjq.cn/Article/details/grfpwqawj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gmvmswrqy.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/guegphszj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/gosflqyov.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.zdbjq.cn/Article/details/gltlksdpn.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/gnibvmsqm.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/garxjanpp.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/gnmzuusei.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/gzjxgqaiw.sHtML

[T53] Scala：字符串插值
来源：http://baike.hesvh.cn/Article/details/gnrsichfx.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/glvxdseke.sHtML

[T54] Scala：集合映射
来源：http://m.share.hesvh.cn/Article/details/guxgbpxft.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/grwqtjwjf.sHtML

[T55] Scala：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/ghywughgr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gjfrykobs.sHtML

[T56] Scala：样例类
来源：http://m.share.zdbjq.cn/Article/details/gdhuswyxx.sHtML

case class User(name: String, age: Int)
来源：http://m.share.hesvh.cn/Article/details/gfzpqionf.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gqtfyfsyt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/gprxrwwmd.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/gxrvhcpgi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/gllpgwxny.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/gzycikgbs.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gootskrqj.sHtML

[T60] Scala：折叠
来源：http://www.blog.fehbvm.com/Article/details/glefsbpyk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fehbvm.com/Article/details/guxdqjejh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghtkduozg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gkcnqlbsr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gghqgivki.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fehbvm.com/Article/details/ghvzgvddr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/ghscnwoqk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/gfxynhgha.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/gnzaoabmk.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fehbvm.com/Article/details/gkqrjdpyh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gvihddhtz.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/gpeicoezj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.zdbjq.cn/Article/details/gktbvuflz.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gbwcmwukf.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gtjsjonez.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gwqybixya.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/gqnpmcqcq.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/gnrragdwk.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/gsipzpoxv.sHtML

[U08] Py：展平二维列表
来源：http://wap.zdbjq.cn/Article/details/gvvahyyze.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gxujclvrv.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fehbvm.com/Article/details/giydubtgd.sHtML

max(d, key=d.get)
来源：http://wap.fehbvm.com/Article/details/gqtxkosvl.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gcgvljbea.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fehbvm.com/Article/details/grmpyhkqp.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/grxqxragu.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/gfpnrzwec.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gwwikwuhk.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.zdbjq.cn/Article/details/glzxhiffm.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fehbvm.com/Article/details/gpmybliis.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/gnvkmxtvs.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/gbgxrpqxo.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/ggijmttze.sHtML

[U15] Py：高精度计时
来源：http://read.share.zdbjq.cn/Article/details/ggclowipi.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/gynsotfdu.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gyucuxqsz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gvaiqbbtr.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/georwpjrn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/gbdnvkmpf.sHtML

[U18] Py：预编译正则
来源：http://read.share.fehbvm.com/Article/details/gojgeeldq.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fehbvm.com/Article/details/gdorwqaxg.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/geqbwulul.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/gnkewdyuz.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fehbvm.com/Article/details/gceetnfmu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.zdbjq.cn/Article/details/goowijhol.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/gvasebkzr.sHtML

@contextlib.contextmanager
来源：http://www.share.fehbvm.com/Article/details/gkgcapovh.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/gnpsacdis.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/ggacqjtmv.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fehbvm.com/Article/details/grufyrfne.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/gncktpgrs.sHtML

[U24] Py：路径操作
来源：http://www.m.share.zdbjq.cn/Article/details/gnstwgwqu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gpwclnwlh.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.hesvh.cn/Article/details/gqacjjohb.sHtML

csv.DictReader(f)
来源：http://m.share.zdbjq.cn/Article/details/gaixzaxsc.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/gmpodjtgu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fehbvm.com/Article/details/gjobmyxkr.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.zdbjq.cn/Article/details/gqoqyhrjf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.hesvh.cn/Article/details/guhssyxkw.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/gfddryvrx.sHtML

UserId = int
来源：http://m.share.hesvh.cn/Article/details/gltaofmlu.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/gnxkqtbjv.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fehbvm.com/Article/details/gickxthel.sHtML

[U30] Py：数据类
来源：http://www.blog.fehbvm.com/Article/details/gpwssfxod.sHtML

@dataclass(slots=True)
来源：http://www.blog.zdbjq.cn/Article/details/gpqrmqlwy.sHtML

[U31] Py：单测
来源：http://mobile.fehbvm.com/Article/details/gskbbwzoy.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/gnwppxkuu.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gbzwhugpx.sHtML

ruff format . && ruff check --fix .
来源：http://blog.hesvh.cn/Article/details/gtzsjfhql.sHtML

[U33] Py：打包发布
来源：http://3g.fehbvm.com/Article/details/gdydyajtg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/gubuezool.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/geaoyfttm.sHtML

chardet.detect(raw)
来源：http://blog.fehbvm.com/Article/details/gdngjbhvr.sHtML

[U35] Py：发送邮件
来源：http://read.share.zdbjq.cn/Article/details/ggrwinzyd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/gfbugfand.sHtML

[U36] Py：定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gwubxgecc.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.zdbjq.cn/Article/details/gtqmncfgm.sHtML

[U37] Py：读写 Excel
来源：http://www.share.hesvh.cn/Article/details/gvspozyhs.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fehbvm.com/Article/details/gxrywnftm.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/gciijgwwx.sHtML

Path(__file__).resolve().parent
来源：http://baike.fehbvm.com/Article/details/gexqzjnac.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.zdbjq.cn/Article/details/ghejbdjqg.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/gcjguxqar.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/gkiafcqvi.sHtML

print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gzldzplej.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fehbvm.com/Article/details/giwcxfibd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/gfzxzqwfj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/gxmgnibmx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.zdbjq.cn/Article/details/gnhkxgxjv.sHtML

[U43] PHP：声明命名空间
来源：http://wap.zdbjq.cn/Article/details/gowqhhwnp.sHtML

namespace App\Http;
来源：http://blog.zdbjq.cn/Article/details/grvoneifc.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.hesvh.cn/Article/details/gqjmwzvkt.sHtML

declare(strict_types=1);
来源：http://www.blog.zdbjq.cn/Article/details/gtrjwoglr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/gpdeqfkai.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gkwdahzre.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.zdbjq.cn/Article/details/gshvkjjms.sHtML

?string $name = null
来源：http://m.share.fehbvm.com/Article/details/gfnxymfay.sHtML

[U47] PHP：联合类型
来源：http://baike.fehbvm.com/Article/details/gfwoaixae.sHtML

int|string $id
来源：http://www.m.share.hesvh.cn/Article/details/greaqduof.sHtML

[U48] PHP：纯枚举
来源：http://baike.zdbjq.cn/Article/details/gmssytpeh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.zdbjq.cn/Article/details/gsvpdzebs.sHtML

[U49] PHP：只读属性
来源：http://read.share.fehbvm.com/Article/details/ggqzxpabo.sHtML

public readonly string $name
来源：http://www.share.hesvh.cn/Article/details/gofyyndma.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.hesvh.cn/Article/details/gtwvhbaaw.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.hesvh.cn/Article/details/gwjdgnmji.sHtML

[U51] PHP：数组解构
来源：http://blog.hesvh.cn/Article/details/gpaujzigc.sHtML

[$a, $b] = $arr;
来源：http://baike.zdbjq.cn/Article/details/gkkwxkhsu.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gnsggiekn.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/gtxpsjqvc.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fehbvm.com/Article/details/gxegybyco.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fehbvm.com/Article/details/gmqdqplie.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/gbbfcmycf.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/ghifulhlk.sHtML

[U55] PHP：match 表达式
来源：http://read.share.zdbjq.cn/Article/details/gesyvywfo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gqitwhluk.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fehbvm.com/Article/details/geymdylgc.sHtML

f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gzglvnzta.sHtML

[U57] PHP：字符串插值
来源：http://www.share.hesvh.cn/Article/details/ggoqvkyhq.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/grivvjvxs.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fehbvm.com/Article/details/gkywovypw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/guolwmpop.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fehbvm.com/Article/details/ggpcuwytv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gtmdwhuhr.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.hesvh.cn/Article/details/gbqbhemtx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/gvxxntjnq.sHtML


<!-- 参考信息 -->