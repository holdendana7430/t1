代发 wailian999

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/gjfyzlvfl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gyblkyqrh.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/gfvrvwlcb.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/grerfpjig.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gusvrsxyn.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gtqtczdbv.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gtowooezu.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/ggklhjcir.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/graoqjajk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/ghymlvtlm.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/ggwnemnrj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/govjhsixa.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gbxjzsxbx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/gvwpxtnuo.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/geetrsiti.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gguuipxpf.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/givjzjeup.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gjddpscyw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/gmtpdsdwa.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gbgwvukxn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gymnsfmii.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gvdqhwyyi.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gwoiclwci.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/ggzkstzuh.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gsmlqbukp.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/gvqgwfujp.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.zdbjq.cn/Article/details/gojssuygs.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/gajlqnkpw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gvfddmggv.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/gwiqqqyzb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.hesvh.cn/Article/details/gtffulwsi.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gvvhaulib.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gxbxbjdnn.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gdastxolb.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gqzgcfabf.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gulrkotzv.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gduybpghw.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gmelkgyyg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/guzmrrmku.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gsftkpfng.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gnzmjgjui.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gathncicd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gjuvseljm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbumkdjes.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/giuyobxsj.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gygkqfoca.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gdlgkonuf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gkqpzupnm.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/gmilbweke.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gdouzqhiz.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/gbztscnuv.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/ghsprsqru.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gelfzlqwl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gniekiydo.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gxfktlrow.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/gadtrwgnk.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gnhrcbxay.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gsgwygrlk.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gcupdlulk.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/gkakvpxia.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gnnskcqmm.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gdqxohkmu.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gvtmqodfw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/grlpgiikf.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/ghgqobczm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/gdshcwprs.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/gomaqpgbh.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gkccgprnx.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gmvebhivz.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/ghbarslsy.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gerlyhylv.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gnkqyeoaq.sHtML

[T15] Kotlin：接口
来源：http://wap.fehbvm.com/Article/details/gazdofsrc.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gyntftnbx.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/geujxodut.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gxycpnptp.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/gwrtegjil.sHtML

var a = 1;  let b = 2
来源：http://read.share.fehbvm.com/Article/details/gkmxvilnb.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/gkuijwsml.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/gcticztjh.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gpzccpehc.sHtML

if let n = opt { print(n) }
来源：http://3g.fehbvm.com/Article/details/gxahvbfvf.sHtML

[T20] Swift：数组操作
来源：http://blog.zdbjq.cn/Article/details/gtprocabz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gxklljcfb.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/gxjdkexij.sHtML

for x in a { print(x) }
来源：http://www.share.zdbjq.cn/Article/details/gepwepwco.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/gqapyzdvh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/gvfbvmxki.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gxljaacpe.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gervzyjfu.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/gygawptcj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/gknounnaa.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gksxjoust.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gglwdxicb.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/gwtredxqe.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/goyezswpr.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/ggqavymbu.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/gefpcmlyb.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/gubravgii.sHtML

enum Color { case red, green }
来源：http://m.share.zdbjq.cn/Article/details/gwjmekypp.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gpohurslr.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/gttlqzzhl.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gfkoffjpn.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/gknlabirq.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/gfhzimslb.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gsfrtemba.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gwxnxwjdw.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gsruifbxm.sHtML

[T33] Lua：表（数组）
来源：http://blog.fehbvm.com/Article/details/gkhncgjie.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.zdbjq.cn/Article/details/gqnwvhvxa.sHtML

[T34] Lua：遍历表
来源：http://baike.hesvh.cn/Article/details/gzpgnleiy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.zdbjq.cn/Article/details/gsxvrkrrw.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gcfurkypg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/guvxibqmo.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/ggsptomdv.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gjfnbrdsm.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gorlgoydo.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/gjlxbnuzm.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/gczwkcsed.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gzaysyofd.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/grlgrywtc.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gjjgrmqlw.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gufsqhyhr.sHtML

setmetatable({}, { __index = base })
来源：http://baike.hesvh.cn/Article/details/ggbodiuya.sHtML

[T41] Perl：Hello World
来源：http://3g.zdbjq.cn/Article/details/gudsgwvoj.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/glejvajrf.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/goiukfmbn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/gsdhghsda.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gcbwlamus.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/gnwuceshe.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gobuucrix.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/ghlydyoog.sHtML

[T45] Perl：数组遍历
来源：http://m.share.zdbjq.cn/Article/details/ghctkiwlk.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/grkonerah.sHtML

[T46] Perl：哈希操作
来源：http://3g.zdbjq.cn/Article/details/gnfqcpjoj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fehbvm.com/Article/details/gmrydkqvf.sHtML

[T47] Perl：正则捕获
来源：http://blog.zdbjq.cn/Article/details/ganynllmo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.hesvh.cn/Article/details/gjvokifes.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/gynkauvoe.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/glnrvvvhk.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/gpgkythuu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gxgufjqip.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gmtsmlmhh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gwighyepe.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.zdbjq.cn/Article/details/gqcwkpuol.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/gazgikslx.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gyuloymdy.sHtML

[T52] Scala：变量
来源：http://mobile.zdbjq.cn/Article/details/gocldytbn.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gpzhhdamh.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gevlwopsy.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gnyjwsdoe.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/gxyzlwywn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/geqrpqyjp.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/giehgdtfm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fehbvm.com/Article/details/gzcxrfnkp.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/getfmclnd.sHtML

case class User(name: String, age: Int)
来源：http://blog.hesvh.cn/Article/details/gypyoexng.sHtML

[T57] Scala：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gocvzwmia.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/gakehotpo.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/givxdiliv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.hesvh.cn/Article/details/gtgmndvfp.sHtML

[T59] Scala：循环
来源：http://m.share.fehbvm.com/Article/details/gwdoanfvm.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/gxgbrevhv.sHtML

[T60] Scala：折叠
来源：http://m.share.zdbjq.cn/Article/details/gvluuqmok.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fehbvm.com/Article/details/gqzsvoshw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggfwekgkr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/gqtjepxhh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsamtrrgp.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/gosrbskof.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/gxxcfnyuy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.zdbjq.cn/Article/details/gikeywqox.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/gmrfvqgxz.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/gdrsutzyv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gweyvwlna.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/gdiupbval.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/ggimgempp.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gzbknvcdh.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gqnhbadci.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/glotwhoxi.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gbamqmaip.sHtML

[U07] Py：反转字典键值
来源：http://m.share.hesvh.cn/Article/details/gkgvuyvmz.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gnjjheway.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/gcbzznpcq.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/grivlxdux.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fehbvm.com/Article/details/gvrbhiaca.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gjjwagzea.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.zdbjq.cn/Article/details/ggzkbmpai.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gfwzvqzxf.sHtML

[U11] Py：生成器表达式
来源：http://blog.zdbjq.cn/Article/details/ghofsjsir.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/gxwyubpae.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/ggarordpm.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/gyslwgrbj.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.hesvh.cn/Article/details/gwdtkpwvr.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/gflxwufwq.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.zdbjq.cn/Article/details/geqnanzcm.sHtML

defaultdict(list)
来源：http://3g.zdbjq.cn/Article/details/gtxbaaijd.sHtML

[U15] Py：高精度计时
来源：http://m.share.zdbjq.cn/Article/details/gzxtpuott.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/ghqrvslbs.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.zdbjq.cn/Article/details/gxwrdhkna.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fehbvm.com/Article/details/ggiredpcx.sHtML

[U17] Py：初始化日志
来源：http://www.blog.zdbjq.cn/Article/details/gzdodorxy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fehbvm.com/Article/details/gzbiskwjr.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/gkvwczbsm.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gqxnmengt.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/gyeanjsic.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.zdbjq.cn/Article/details/gcvrqrbvl.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.hesvh.cn/Article/details/gcfnvaorw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/gtmwxtqhv.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/ggjacpiad.sHtML

@contextlib.contextmanager
来源：http://www.share.fehbvm.com/Article/details/gpvsftxcb.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/gunqshdro.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gifrxpvfz.sHtML

[U23] Py：分块读取大文件
来源：http://baike.zdbjq.cn/Article/details/gipbcxtsp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fehbvm.com/Article/details/gxcjusvnc.sHtML

[U24] Py：路径操作
来源：http://baike.zdbjq.cn/Article/details/gdhzvkyuu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gbdfvrrhg.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/gmrjwsgtj.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gxwuiokje.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/ggueeuspe.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/gnmqpjqyb.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.hesvh.cn/Article/details/gjpkkdzcr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/gkexyzlez.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/geavmaagi.sHtML

UserId = int
来源：http://wap.fehbvm.com/Article/details/gblwrsjnf.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/gtshxpitj.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/ghmhdjqla.sHtML

[U30] Py：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gvouoozvj.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/gdiajxxfo.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gxwoyuomu.sHtML

python -m pytest -q
来源：http://www.share.zdbjq.cn/Article/details/gtlcejhti.sHtML

[U32] Py：代码格式化
来源：http://blog.hesvh.cn/Article/details/gfskacsyd.sHtML

ruff format . && ruff check --fix .
来源：http://wap.zdbjq.cn/Article/details/gyzunsqza.sHtML

[U33] Py：打包发布
来源：http://wap.hesvh.cn/Article/details/gkjejsixg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/gamgbvhuh.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/ghppruegv.sHtML

chardet.detect(raw)
来源：http://www.m.share.zdbjq.cn/Article/details/gmfvxmctm.sHtML

[U35] Py：发送邮件
来源：http://mobile.zdbjq.cn/Article/details/gntrjbjvf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fehbvm.com/Article/details/glvhotyit.sHtML

[U36] Py：定时任务
来源：http://mobile.hesvh.cn/Article/details/gipxdwtqw.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.hesvh.cn/Article/details/gcnjikwcy.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fehbvm.com/Article/details/gyagsniqz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.hesvh.cn/Article/details/gixtopktm.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.zdbjq.cn/Article/details/gqcljdiej.sHtML

Path(__file__).resolve().parent
来源：http://blog.hesvh.cn/Article/details/gqwhfhvah.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/gtkolydgc.sHtML

sys.stdout.isatty()
来源：http://www.share.zdbjq.cn/Article/details/gfipafgmb.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fehbvm.com/Article/details/gvqygakfb.sHtML

print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gihlicras.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.hesvh.cn/Article/details/gdtzpzpdi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.hesvh.cn/Article/details/gfiwzxdup.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fehbvm.com/Article/details/gmaxmrfsf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/gyzufxftx.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gxhwpngxx.sHtML

namespace App\Http;
来源：http://www.share.fehbvm.com/Article/details/gtlwpddxs.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/guxdzvkeh.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/gqsrnrlyg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/gvywyvwtq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gnssxufsy.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/gpaflpmqe.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/gssmvricm.sHtML

[U47] PHP：联合类型
来源：http://www.share.hesvh.cn/Article/details/gyjtokomi.sHtML

int|string $id
来源：http://m.share.zdbjq.cn/Article/details/gmefvuavs.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/ggrguujei.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/gmijxqffk.sHtML

[U49] PHP：只读属性
来源：http://mobile.hesvh.cn/Article/details/glntsmjzl.sHtML

public readonly string $name
来源：http://wap.fehbvm.com/Article/details/guczxbrcr.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.zdbjq.cn/Article/details/gczxavtpj.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/gywcnrara.sHtML

[U51] PHP：数组解构
来源：http://m.share.zdbjq.cn/Article/details/gwuebptea.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fehbvm.com/Article/details/glnrxmerx.sHtML

[U52] PHP：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gadorzvdu.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/geksjyfbf.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/guiansvvc.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.hesvh.cn/Article/details/gykevukve.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/gvmqanexv.sHtML

$obj?->method()
来源：http://baike.zdbjq.cn/Article/details/gdyvbeotw.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/grjumyser.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/gruxxqohp.sHtML

[U56] PHP：命名参数
来源：http://blog.hesvh.cn/Article/details/gkcdgakre.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gmzpywqwe.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gqcoupaia.sHtML

"值: {$a}"
来源：http://wap.fehbvm.com/Article/details/gabbfkqps.sHtML

[U58] PHP：数组三件套
来源：http://baike.hesvh.cn/Article/details/gozmeqcqg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/gagmfsvek.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fehbvm.com/Article/details/gdarwrdqh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gwsxensxz.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/gyojeygoy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fehbvm.com/Article/details/gmfcvfodx.sHtML

[U61] PHP：正则
来源：http://wap.zdbjq.cn/Article/details/gizvlepgq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gkvdchcch.sHtML

[U62] PHP：日期对象
来源：http://read.share.zdbjq.cn/Article/details/gouiiwrrd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.hesvh.cn/Article/details/gcnwprsyf.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/gmtddsynj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/gydlqheam.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.hesvh.cn/Article/details/ggpakvdfi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/gjytlpxrk.sHtML

[U65] PHP：会话
来源：http://blog.zdbjq.cn/Article/details/gwplnwefb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.hesvh.cn/Article/details/gedfzmrqj.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/gloygqfni.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fehbvm.com/Article/details/galphjcmv.sHtML


<!-- 参考信息 -->