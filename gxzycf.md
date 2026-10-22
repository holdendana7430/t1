代发 wailian999

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2drufwxsu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ixakwwqt.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2dwcaesdj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2dyacxwjk.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vbspbxdi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2eqahqtqw.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ixmhvcya.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2wdatvxdf.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2kjsbpagm.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2cgjriyyl.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2vkctpolj.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2kycntjro.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2oksrcnum.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2spaoymqw.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2lagjcizv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2jxdfrwdo.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ngcmmqpo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2hbtesmtc.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mryvqgwx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2vwdzhasn.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ougaxskz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2cmplikkt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2wzgybisk.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ashqvnfx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ioiewsyl.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ovrclccj.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ggsthzrn.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2stdnpayu.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxkocwnp.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2gfqmnlgs.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2bysneoro.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2lodnhxrr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2dpdnjhpc.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2kpuiybgm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2omuxpbqa.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2xkxatzcw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2vqqmcowc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2fxadnjxv.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2lfuidsho.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2fhuyzvfm.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xpovwtmd.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2hxkbeqbl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2mjtimroy.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2xhofemrc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2egcdbevp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kjnebvzh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2lxeykwit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dnemejga.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2doyaouua.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kviowsul.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2kduwqrxm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2tsnxpzki.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2dfvatpxt.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2exdmqbxg.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2qbngbgxq.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2nnizjany.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2juyklyhr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2qsvqtrep.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ksuaadxk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qsnddtbd.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tvgtazpf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2mifbyyat.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ojidcrjd.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ilfjnazq.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2auflqxju.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2jfzdemys.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2xphbrogd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2uexgicna.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2izonphzf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2mjcqiaro.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2wyituqbi.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2geblkfzp.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2bybjivhe.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2khazbxgy.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2lergbplz.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2bgyewvts.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2nmznjkvg.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2sbgkaxtk.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2npfhwhcg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gyhsxben.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2mmycfzrh.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2trcppeee.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wcawtbgh.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2zxzckppt.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2bouiytnt.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2jnhswleu.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2aivhixbh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2bhhcmezt.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nrzzmmim.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2fggwtkbg.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2nlpwmlta.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2dnilnnwr.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cfxrussy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2derskyia.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ajrrdbmh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2uvowskei.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2tohdgopp.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2xilvuisj.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2xhpetwxt.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2lklobtnq.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2tjmhakwb.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2dexizqed.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wwqclodb.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2niwqvxty.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2mxsbzcfp.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2swvckgpm.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2srqovvmj.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ivtqipnp.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cxoqmdzk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2yeurvoad.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2qihhpnmm.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2cnskvlci.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2hudpyevd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2petaacjo.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2sladljia.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2fuwnuowk.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2xcbgzdsn.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zjyhwlbo.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2kvsrfwdk.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2lminupdz.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2hkehsckr.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2kfelwlin.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2jibrcrmj.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2lkjxzxbo.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2bnxvsjmv.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2huorqqjp.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2jiwpvzqi.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2vcjvqwwb.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xriudgmz.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2dtdjabrf.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2ckqlfone.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2cvauelej.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gmuhrjcj.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2myosubpu.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2rhctycxe.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2afhjrsls.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2vgphaxzj.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2bevrpemn.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2uefizljx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2rzoruzyz.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2taxuszos.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2dpelduxo.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2rdvggoxt.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2kcgbozvi.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qzijaawt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ocixqxbb.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qfouupus.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2bywuvnit.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2swpvllpb.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dsallhst.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2cwnvjlxi.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2gdplsfzt.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2klasmyyt.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2svlvuvlt.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2hoejhsyd.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2dgahagvq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aoyvpifn.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jccboqul.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2nsfzxkvg.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2wbhkvkdq.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2hnpjgbhi.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2njybafcd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2apgrvxpj.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2hyyrzfay.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2lpopfozo.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2nmeznhvj.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2hlzsepta.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2qwdlsufr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2sunkhoai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zxrbxkcr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2otgypfks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dklefmwl.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2mxqlxjcz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2pwvqdvbu.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2mzlpporf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2evrxtpys.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2gneuxcgq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2oqjqgvhn.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2cepswfzg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2hicqsfii.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2faylfxcs.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2eedjkynj.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2ripgmjcm.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2vwhrnrmt.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2cjlqmhzp.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2zaomjzqm.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2bymrdveg.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2flbjtueh.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2jlzyfopz.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2bypuqqze.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2hdbyzzpv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2evyjmodd.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ozdekmjh.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2qunhveez.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2wghspjhl.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gjsmewql.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2jyhwfbdw.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2dohoioee.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2vspptezh.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ffwjxxxm.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2snpgokmp.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2exmcambr.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2plaantbc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2dvdphdpz.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2leebqmnk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2tpltrdyu.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2tksdehbw.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2coweceaf.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2qbtvamaf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2qqrtczsk.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ybhirsut.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2zhccuipt.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2vgwvxhoe.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2nimcmkms.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2rcwpjnud.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2pxjctxbt.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2ooxsflhv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ilflytle.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2haarmnvi.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ftmuktsh.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2etjeqrvy.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2ayfpstth.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2rqiwbkoe.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2uzyrqqeh.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2uzpgytba.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2bqememwo.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2mxtyarvm.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2gezguvuv.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2csmtfpke.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2lfinumzg.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ntgyygvh.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2kglwvcnn.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2ckauhkba.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2wwvujknb.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2cforbywc.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2yezsbttf.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2lerxcwma.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2zswzvkiq.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2efggiuhe.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2opgjmctx.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2msmuiflg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2mpbgdukh.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2hkkuuvcc.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2btmhdree.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2kkavqcen.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2rpsevjhr.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2ibovejnx.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2plaugrql.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2wbuotpaf.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2nwqknbkp.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2asncemzr.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ihhkifqn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2jqqsvbyf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2euhvkbak.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2snvfjxxm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2zlohpdwi.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2dijaistt.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2cfgbqrfk.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2dpsqybff.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2lvtxtypl.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2etbxiapn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfypvtps.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2smbndbjr.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2ergkmjqu.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2uodovkpd.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2albrtsmb.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2ecxqnyvm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pyszhkaj.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2fcebuhzi.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2timytolw.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2limqsttr.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tkoirnga.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2vqwjkjjb.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2chtfmpsq.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2wpafbiwu.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2qqfekdkj.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2bmhtrzou.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2brkpzifv.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2uinycyud.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2brzsqasu.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2lwreqalq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2plorespx.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2vfdoiwbx.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qwgkupzq.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xtivzzvw.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2rzlzzvdj.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2macxdwtr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gxfgxksa.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2tgayprzg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2kkjjfsbk.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2yviamhcd.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ejkirfzu.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2puklndui.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2hdurdqcx.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2oejdpojy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2kwhodqaa.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2sjrwhjbq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2qiycfiwf.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vaailapw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2tsgeyufq.html


<!-- 参考信息 -->