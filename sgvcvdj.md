代发 wailian999

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmgzcvuw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gfpdomdrp.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gihgpysgz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gstfqnnqz.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gmocurxlr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/giirwwzto.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/ggbkfnouo.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gunwtjwep.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gwffgjwjc.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/grumtzlnb.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gwmyvffok.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvtehudlj.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gkvjwluwt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdlhaxwx.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gjcqbyxwd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghqcgybhf.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/ggsbnkepq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grfpogkof.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gtcooirxe.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/genxvazsl.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfhifbtx.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruxmjilk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gldasdads.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gueliamkf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdleikrj.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/goopejfqr.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gfptiwnin.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gxpyfpfdu.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghxosnyhg.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gtnrqmphj.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gefyienqd.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gptlcqjyt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/ggvabxabb.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guiutsacr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlgzepcn.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gztplrmvi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjpgyvwg.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/glapsbofz.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gdvdjgyvy.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gyfmrwuwb.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaomyzgfv.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfigbzxhc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbltukbh.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxkcccoh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gigiylydz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyplxfpxm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/grpjiigqu.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghomhldps.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gcmchtssz.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gskfunthp.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwweymvwc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/garcbfkmy.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqoghktfz.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaukhiokf.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbktvdpb.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gwswuumsh.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gpovqskiy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrcfylmf.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajigjmvr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/grtjottto.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gkpwzlnsp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grentlyew.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdwmrwza.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gcgotbhhs.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjwjgqbo.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxptnxii.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gglqftoso.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgasihdz.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gfpsdgogu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghipwxazc.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqftazde.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gltczpelc.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrdylbbr.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gnebhcvpm.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjtlkrpq.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxiubmsju.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/glzlovqse.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gdavyjlbo.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gyolblqcx.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gwfnjuweb.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gokgyfmvm.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxbcmfcl.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdfyqeck.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/glclqsmuj.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/grbbqqzmg.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbehmpbe.sHtML

[T20] Swift：数组操作
来源：http://m.share.fanxiaobao.xyz/Article/details/grzavdsis.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gjwusshgr.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/ggteorlev.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/ggyhwbkul.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gzdvvplfb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gyuyitmae.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/glripolme.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gsrykhkqi.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/guvnjkmdp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gcfmtlwor.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzohplax.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfgupihu.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhhwefbg.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/geevlnlnx.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/gvthyglnf.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxansgim.sHtML

[T28] Swift：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnaoynbd.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gjgftyafc.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/grikgsiuv.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikiznuyo.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsfwxxcd.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gufqjzxfc.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/glpqhzlzn.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gatnclfte.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gytmqzneb.sHtML

local a = 1
来源：http://baike.fanxiaobao.xyz/Article/details/ginvftsxd.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqylgngp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/gsdgdgocp.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/gtcclfmsd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjpsofqf.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/gankpgxlk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gnemuqmop.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwgqxrjv.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyfwtpmk.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gslhsevix.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/gkkljegno.sHtML

[T38] Lua：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkmhqbrq.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/guhmvkgws.sHtML

[T39] Lua：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gfznnjyqc.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gknmeoaag.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqlgefus.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gsmzoddie.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhbaiton.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gybzyzsif.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfjlmjba.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjgqudrn.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/glwgfseob.sHtML

"值: $a"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmktvaslr.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzjtjsoa.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gutniqnrw.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzcwnwte.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gviqoeqwo.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/gukebtmwz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnickheli.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/ghsngqycs.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjdhszmqr.sHtML

[T48] Perl：正则替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfuyhttx.sHtML

$s =~ s/old/new/g;
来源：http://baike.fanxiaobao.xyz/Article/details/gclisflsb.sHtML

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gaikcftog.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlteanqe.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjzzdztm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnlipfkc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdurcdzeg.sHtML

[T51] Scala：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gkphuhnoi.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykeyjsvl.sHtML

[T52] Scala：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gaocaqxsg.sHtML

val a = 1;  var b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gptwszych.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gyphenkch.sHtML

s"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqaiksds.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrfiwhpk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmmnovcz.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gsrfweumv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/ghoqdawus.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgemuhjf.sHtML

case class User(name: String, age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gbcokmwgu.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmzcjnvs.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fanxiaobao.xyz/Article/details/gufuvwjke.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvewzerk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gvmzlbgmo.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gzzilvwax.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gxoueloek.sHtML

[T60] Scala：折叠
来源：http://wap.fanxiaobao.xyz/Article/details/ghijpsxsm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giosbrpmx.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gkqzslnzr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/goixpzxiz.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcmykpvl.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/gzpypetag.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbwkeajo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/gwvaaxssl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gwvpxbiyb.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gbtnndihb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/gmlgpftgu.sHtML

[U04] Py：变量调试打印
来源：http://blog.fanxiaobao.xyz/Article/details/gdvbwxkqe.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyaefsqw.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxjfyxft.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gbtvrzrub.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/gpcxvhhzd.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzghkgvt.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fanxiaobao.xyz/Article/details/greufjxeq.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/glhzecync.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/gznrnpxic.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/gfwwszvbd.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fanxiaobao.xyz/Article/details/gqteblhqg.sHtML

max(d, key=d.get)
来源：http://blog.fanxiaobao.xyz/Article/details/gjfhgqavv.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmgaheag.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesbozpkf.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gdftspoet.sHtML

(x * 2 for x in arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gcdandzkf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gkaambnaz.sHtML

Counter(arr).most_common(3)
来源：http://3g.fanxiaobao.xyz/Article/details/grrtpfxni.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gefgalrzx.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnppqidbz.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gjdgebjmd.sHtML

defaultdict(list)
来源：http://blog.fanxiaobao.xyz/Article/details/gmsngamvv.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjdukbng.sHtML

t = time.perf_counter()
来源：http://baike.fanxiaobao.xyz/Article/details/gkjhqfqxz.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grebtdbog.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fanxiaobao.xyz/Article/details/gnlcyyvwz.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtfbniqq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fanxiaobao.xyz/Article/details/gtcoouwmi.sHtML

[U18] Py：预编译正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gvayjkges.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gugxpsdfv.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwrspfup.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fanxiaobao.xyz/Article/details/gserhtqme.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjorrnhg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/gddhbkvhi.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fanxiaobao.xyz/Article/details/gdxzmlooo.sHtML

@contextlib.contextmanager
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhegxphc.sHtML

[U22] Py：矩阵转置
来源：http://baike.fanxiaobao.xyz/Article/details/gxjbccfkg.sHtML

list(zip(*m))
来源：http://blog.fanxiaobao.xyz/Article/details/goszkbtyp.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvbmjery.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqhvgyya.sHtML

[U24] Py：路径操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcwnhhre.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwuroodq.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gfnwevkoh.sHtML

csv.DictReader(f)
来源：http://wap.fanxiaobao.xyz/Article/details/gbhwfrvzf.sHtML

[U26] Py：并发下载
来源：http://www.share.fanxiaobao.xyz/Article/details/gayfhwivu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmexusazj.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtufubda.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fanxiaobao.xyz/Article/details/gviqhzcow.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/gxefcmlro.sHtML

UserId = int
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqnihokm.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskpvkssp.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/gapuufmpo.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gvvqavucn.sHtML

@dataclass(slots=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzikphshg.sHtML

[U31] Py：单测
来源：http://m.share.fanxiaobao.xyz/Article/details/gaooyprtf.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlzlekge.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdnmckad.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgaugdoo.sHtML

[U33] Py：打包发布
来源：http://3g.fanxiaobao.xyz/Article/details/gmmlbtgsf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fanxiaobao.xyz/Article/details/gmmruaiov.sHtML

[U34] Py：判断编码
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbksyifv.sHtML

chardet.detect(raw)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyblrjnwt.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkthigsi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fanxiaobao.xyz/Article/details/guxqkesbe.sHtML

[U36] Py：定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gszybejtt.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fanxiaobao.xyz/Article/details/geuokqatq.sHtML

[U37] Py：读写 Excel
来源：http://3g.fanxiaobao.xyz/Article/details/gznuuxyaf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gaapefymt.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fanxiaobao.xyz/Article/details/glqcglunn.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjbeqlje.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcmizvhk.sHtML

sys.stdout.isatty()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbpmrydt.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhuizrob.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gffwijqdp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fanxiaobao.xyz/Article/details/glvbltcnm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvfhrkds.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwfzswho.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gglzytgkj.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gtglrvdtb.sHtML

namespace App\Http;
来源：http://www.share.fanxiaobao.xyz/Article/details/grqqbugkb.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fanxiaobao.xyz/Article/details/gncisdpke.sHtML

declare(strict_types=1);
来源：http://blog.fanxiaobao.xyz/Article/details/gthhzedjv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpggmmqb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbzqfnqvf.sHtML

[U46] PHP：可空类型
来源：http://wap.fanxiaobao.xyz/Article/details/grbcgkrty.sHtML

?string $name = null
来源：http://wap.fanxiaobao.xyz/Article/details/gdrmzclpl.sHtML

[U47] PHP：联合类型
来源：http://3g.fanxiaobao.xyz/Article/details/gmglvjvez.sHtML

int|string $id
来源：http://3g.fanxiaobao.xyz/Article/details/gtbajgiuc.sHtML

[U48] PHP：纯枚举
来源：http://blog.fanxiaobao.xyz/Article/details/geyevrteu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfhejjgve.sHtML

[U49] PHP：只读属性
来源：http://blog.fanxiaobao.xyz/Article/details/giznvaist.sHtML

public readonly string $name
来源：http://3g.fanxiaobao.xyz/Article/details/gtklqgtff.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fanxiaobao.xyz/Article/details/gffbsxkhl.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkmimafa.sHtML

[U51] PHP：数组解构
来源：http://blog.fanxiaobao.xyz/Article/details/gukmwjexc.sHtML

[$a, $b] = $arr;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqgmenyv.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfkxmdnj.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gztyhvmua.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpcmlbaj.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fanxiaobao.xyz/Article/details/gzelhfvmi.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fanxiaobao.xyz/Article/details/gidhhtcri.sHtML

$obj?->method()
来源：http://baike.fanxiaobao.xyz/Article/details/gcjisekhh.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlgyrjah.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fanxiaobao.xyz/Article/details/gmcrnrymv.sHtML

[U56] PHP：命名参数
来源：http://blog.fanxiaobao.xyz/Article/details/gmuigsnmm.sHtML

f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gmqbrktjf.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcvyfkrx.sHtML

"值: {$a}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgjvycez.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgytbtix.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnmjlmpc.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyamduci.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfrqdjzl.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fanxiaobao.xyz/Article/details/gyvjupala.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcztgxlyi.sHtML

[U61] PHP：正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuociyii.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmypuiett.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqymqfihc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fanxiaobao.xyz/Article/details/gztklhnch.sHtML

[U63] PHP：文件读写
来源：http://3g.fanxiaobao.xyz/Article/details/gytsresuf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqppzhhsx.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduiwfegu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgpiwgvg.sHtML


<!-- 参考信息 -->