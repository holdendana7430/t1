代发 wailian999

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/ghxltklhz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gdkndledb.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdisdnmrs.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/goxllnpyv.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gibmwtzrk.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaujlhnlq.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gcgtdtetd.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glklsgzrd.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgkrtblg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/goixrgoct.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/gjpffrtlo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxfytlay.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchkhnpew.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvxzvqwk.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqibyiikj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjmrpcge.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbbmlrhv.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgmvktda.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/goerlqkja.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvjohthy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcudnnprn.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gfktktkbg.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxvrpwrc.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gwzijrewq.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnygnaolz.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdcamsac.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gppstlhop.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/glzvhcvsg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqawirqrl.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gvrzdcykj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/grqvarjjm.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/ggpaafpeg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/geaszsjph.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gptzdiwub.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gkmicrrag.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvrlkvpj.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnelxocsr.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gegbuhnzw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvnrxdnk.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gewwdftxq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gqaiqcuoh.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gxvwjeqmj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdapebns.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvxovnby.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcidsyna.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyssiawt.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjudbffo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjljeeszi.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gwflmltyd.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcfgrcya.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslwmibyd.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gwlblpdlt.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gajamyqbl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gsszinfzq.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmvoammq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gcvoguhrz.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gywktkzyx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gneuudoch.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gtfixggez.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gfosnmhpb.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/guxomexnm.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gomxuyyuv.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxdhprft.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/gmhmghjfz.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/ghanovzqr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gvvggelji.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdscqyoz.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gablhsuej.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gqfqysbpx.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwuesblv.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gqaapxhxx.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpevdbnmn.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gsfasvkgr.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gdbdnnnsh.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gunfjqylh.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gksztbwtj.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gwobzmzkg.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/glcuflrzg.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyltncik.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/golibpmpu.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gilnntewg.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/gqoypdlla.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gmzgwajbd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fanxiaobao.xyz/Article/details/gjyqpkypp.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gozcizzah.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/govmmnafx.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gwvywxafb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdxcmddo.sHtML

[T23] Swift：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbipcisay.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gldgotadd.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gqtnzfdti.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gynmbpdry.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gixrenwpj.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjawzzky.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnigvajz.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvcirkky.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gjbjdjxos.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtglzxqak.sHtML

[T28] Swift：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxkomnqy.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqnwumys.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/glpotpqds.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gifcgbrux.sHtML

[T30] Swift：协议
来源：http://baike.fanxiaobao.xyz/Article/details/gyhpbcwri.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzjstqhs.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuyqrpcb.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmuegatk.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gnewizddd.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/ggxozycoj.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyirixerv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrycedng.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkbeaqbk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/geyzxlcos.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/grasuxncc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqetsipd.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/grcjrhiex.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gyejusjue.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gdwaldvem.sHtML

"a" .. "b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtiouuiok.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/ggeitdtjj.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtedqncas.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntezwlfe.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gafrvaqbh.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/ggizhjrom.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/gohgdipdu.sHtML

[T41] Perl：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzarnylh.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybfdzxge.sHtML

[T42] Perl：变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gejzsvkyy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemfkkoyr.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskyayaqd.sHtML

"值: $a"
来源：http://m.share.fanxiaobao.xyz/Article/details/guctupmme.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gabcnjktv.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdmovzwrj.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtzwywpw.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtqhrfguk.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/gypkbtwnp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggouvccfg.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrjezkjs.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvkccvgx.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjbgmxme.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrmfbhzq.sHtML

[T49] Perl：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gitrosbnh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnnnewrm.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygdgrdsb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyohipvvb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfffmtyx.sHtML

[T51] Scala：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/glngnnglx.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gmpmzzdmj.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gcbwqkzrq.sHtML

val a = 1;  var b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gnffwydar.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gntiipant.sHtML

s"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrsjimbx.sHtML

[T54] Scala：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gsxfusmlb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gspxxbbiw.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/ginmhcphm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmaebeus.sHtML

[T56] Scala：样例类
来源：http://mobile.fanxiaobao.xyz/Article/details/gpyqfgdha.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzudiyjqs.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/guwkdmxtp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fanxiaobao.xyz/Article/details/gdzjdgawn.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/guzvmahze.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdlfesdu.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/glrtcsjts.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gihmzryht.sHtML

[T60] Scala：折叠
来源：http://blog.fanxiaobao.xyz/Article/details/gdbewgnpk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/gjuvdkaua.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gczjtteug.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gwinykalv.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gvmtguovh.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagpouwes.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/gbycmqkuc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fanxiaobao.xyz/Article/details/gjvjjyfus.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkuxdqaj.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/goawcgoci.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyyprcwz.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/gthbmvsnf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/grhjkyafs.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/gjobpypwm.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdgrhcrb.sHtML

[U06] Py：合并两个字典
来源：http://3g.fanxiaobao.xyz/Article/details/gnatnifne.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpwizmcw.sHtML

[U07] Py：反转字典键值
来源：http://blog.fanxiaobao.xyz/Article/details/gjsajqvep.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gcxnsfjrw.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gjstbzlpw.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gbdlagcfv.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fanxiaobao.xyz/Article/details/gauzbumxu.sHtML

max(d, key=d.get)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqwoyoxw.sHtML

[U10] Py：按值排序字典
来源：http://baike.fanxiaobao.xyz/Article/details/gtolhincx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/gupdxaktk.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/ghifkoqdj.sHtML

(x * 2 for x in arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gihrsmhkz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/ggturzsyj.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/giaqcfhwr.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gmksllrgc.sHtML

deque(maxlen=10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsowzscv.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gztvmkwzm.sHtML

defaultdict(list)
来源：http://baike.fanxiaobao.xyz/Article/details/gsyimvwek.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrevswvr.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/gimylikrf.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguwtoinu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fanxiaobao.xyz/Article/details/godunflxg.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gthsbzklu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpacqzth.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtayfkxv.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhjrrpoo.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/gybyzewpr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/gicinhodj.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gayultkas.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/gktpblibe.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fanxiaobao.xyz/Article/details/gerbbnudh.sHtML

@contextlib.contextmanager
来源：http://baike.fanxiaobao.xyz/Article/details/gqcnjgilw.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fanxiaobao.xyz/Article/details/gnetnfqoa.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/gboaevyzp.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrhhihls.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuejjbtv.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gycfpklws.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gasbblhzo.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fanxiaobao.xyz/Article/details/glbqydvry.sHtML

csv.DictReader(f)
来源：http://baike.fanxiaobao.xyz/Article/details/gtmyxiyba.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/gttwjydqy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjiuqcgn.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpcswodz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqkzvptu.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gxsucaccy.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwcitqya.sHtML

[U29] Py：属性校验
来源：http://blog.fanxiaobao.xyz/Article/details/gcdsgjbua.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/gnnuphaom.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfafulbqt.sHtML

@dataclass(slots=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gejxbgznx.sHtML

[U31] Py：单测
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzuuwkfj.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvxkloqx.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gzxmravco.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fanxiaobao.xyz/Article/details/glkgqpnly.sHtML

[U33] Py：打包发布
来源：http://www.share.fanxiaobao.xyz/Article/details/grfwevcgx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxamfanbt.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftzupfav.sHtML

chardet.detect(raw)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycqdqpnc.sHtML

[U35] Py：发送邮件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlxqkgoj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqulvgsp.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbiegyepc.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fanxiaobao.xyz/Article/details/govxkkjbo.sHtML

[U37] Py：读写 Excel
来源：http://wap.fanxiaobao.xyz/Article/details/gyrddzhzf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fanxiaobao.xyz/Article/details/girhrxdkn.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygbosmiy.sHtML

Path(__file__).resolve().parent
来源：http://blog.fanxiaobao.xyz/Article/details/gdjnbknsf.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fanxiaobao.xyz/Article/details/gufckctbd.sHtML

sys.stdout.isatty()
来源：http://m.share.fanxiaobao.xyz/Article/details/gewvtccej.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fanxiaobao.xyz/Article/details/glynwuuid.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/gcdilsfqp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqzkxhob.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fanxiaobao.xyz/Article/details/gkppjwnuq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fanxiaobao.xyz/Article/details/gatwqskjr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxledsjo.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsacanfz.sHtML

namespace App\Http;
来源：http://m.share.fanxiaobao.xyz/Article/details/gejujzjop.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcwrrrfq.sHtML

declare(strict_types=1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywnqhxlm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fanxiaobao.xyz/Article/details/gikpmewlh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnohacpov.sHtML

[U46] PHP：可空类型
来源：http://baike.fanxiaobao.xyz/Article/details/ghofstekg.sHtML

?string $name = null
来源：http://blog.fanxiaobao.xyz/Article/details/gvshcmrpl.sHtML

[U47] PHP：联合类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzhqgiaq.sHtML

int|string $id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzcozkjf.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntfjgycq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fanxiaobao.xyz/Article/details/geeekcgjd.sHtML

[U49] PHP：只读属性
来源：http://3g.fanxiaobao.xyz/Article/details/gavrpipxs.sHtML

public readonly string $name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzhdzvjp.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fanxiaobao.xyz/Article/details/gwkkddpjw.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuotmfqn.sHtML

[U51] PHP：数组解构
来源：http://wap.fanxiaobao.xyz/Article/details/ghjxxnmum.sHtML

[$a, $b] = $arr;
来源：http://wap.fanxiaobao.xyz/Article/details/gqsubtuyd.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/givdgksgp.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/grzekvrfs.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fanxiaobao.xyz/Article/details/gscewjyds.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fanxiaobao.xyz/Article/details/gsqkeyxwx.sHtML

[U54] PHP：空安全调用
来源：http://3g.fanxiaobao.xyz/Article/details/gtokwkvrr.sHtML

$obj?->method()
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbxxrjzs.sHtML

[U55] PHP：match 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gwasiqkuc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fanxiaobao.xyz/Article/details/gkmorypee.sHtML

[U56] PHP：命名参数
来源：http://blog.fanxiaobao.xyz/Article/details/gzlyrrsuf.sHtML

f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtygmldit.sHtML

[U57] PHP：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gnobpazfh.sHtML

"值: {$a}"
来源：http://wap.fanxiaobao.xyz/Article/details/glscoaffd.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqwktvrz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gejfzvsqq.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gawbradrc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gumkhenqh.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fanxiaobao.xyz/Article/details/grflqkdgs.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gxwfetyrq.sHtML

[U61] PHP：正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdbambdr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gminyqqbp.sHtML

[U62] PHP：日期对象
来源：http://3g.fanxiaobao.xyz/Article/details/gvdbzrqdp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqyvgqwf.sHtML

[U63] PHP：文件读写
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtgpzomq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fanxiaobao.xyz/Article/details/goacrqomw.sHtML

[U64] PHP：目录遍历
来源：http://baike.fanxiaobao.xyz/Article/details/grnwvhfts.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fanxiaobao.xyz/Article/details/gkehdjfoq.sHtML

[U65] PHP：会话
来源：http://read.share.fanxiaobao.xyz/Article/details/glysdcsmj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyldqibyb.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkuuvpuu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gasxuwrat.sHtML


<!-- 参考信息 -->