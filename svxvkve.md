代发 wailian999

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gupefpoit.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/ggelnqutv.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gfoudnbpv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/ghqdhxofv.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/goezrybrs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gxoxrnnix.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gorsjhtjy.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gmnlglikv.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gsuluxqlk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/guvpthefo.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gjysdabfb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gurgugmai.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gibfvgpos.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gowdsygaw.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gwcrfjrcf.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/grddezfft.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gtmgxinsu.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gdvjlbtpt.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gtkoybzuc.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gupesatoo.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gysmdoxpc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/govisobqq.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/gawvjsbxu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gbcqoakgt.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gnqorknaq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gqmyucwwm.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gwkcfnwrp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gmrrgqtql.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/giwqrnrsy.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/ghrfkdqkf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/gxnllowxi.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gnizmdbov.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gfmjfmpci.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gzwssoorj.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/gpwthstrw.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gzdtqijmp.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/geahmigog.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gwuzbmtms.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/gieggknbn.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/gvoqqyvii.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/gcaswjyea.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gohzfdyrh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gjcpnacyc.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/geycunvtc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gvjjolbfq.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gltgzoyra.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gygertkdz.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gnhmeexfv.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/guiojsyyc.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gbizxrwvr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/gixmtigyl.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gmbnerzgo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gacvcyvxw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwzgrpzqp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gpdwpnwro.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glfvcrwur.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gqaanxzkt.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/ggkajdbkq.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/goyjmwrml.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gdekwvrtk.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/guqgphljt.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gpvkruvgx.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/gnfifbgqa.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/grfjxrqkq.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gynquuank.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/ginxgsqow.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/gybryjvqo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gjvvutxwj.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/ggjsubrhk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gwnirmrsq.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gcoqmvzix.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gbxcxrhro.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/gtrrdddnb.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gbmazroge.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/gekjukxfz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gtbvkdusx.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gbuvazsrz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/geebtgjfs.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/gemheopbc.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gvvwkvsvs.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/gdicjceit.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/gcyfpivnp.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gtmbhmktv.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gyntwuwoy.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gueiozxsx.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/geesejodx.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gdvnarkvc.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gwgjuglmg.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gaztwqnfh.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/gjzmnvfov.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/glijtepwl.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/glzngixec.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gaapmiiwq.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gpefmoyun.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/gqajrkpei.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/gjgaxfqfz.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/gdijzofba.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/gfxrufblx.sHtML

[T22] Swift：字典
来源：http://baike.fehbvm.com/Article/details/gbmdtmayq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gwqbxznky.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gmofypmim.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/grxyjcrls.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/gibidwcci.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/gvkuagytp.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/gcrbybpeu.sHtML

struct P { var x: Int }
来源：http://www.m.share.fehbvm.com/Article/details/gkzuonvsx.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/ginjgnttb.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/ggcdmlqkx.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/grgipaokv.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gqirpseoo.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gsayzdapr.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/gujinbsdg.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/gnxacgxnd.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/gydgoyith.sHtML

[T30] Swift：协议
来源：http://mobile.fehbvm.com/Article/details/gsdbwjrry.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gryleahvt.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gfiqovnkr.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gbtjawzbf.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gluklivkj.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/gmgziqmrl.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/gzexoaifp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/gqqmcykzl.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gosqzzskb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/gooiqrhjx.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gdnlmvqpk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gsjiawhzm.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/gmdshhiuv.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/gdlulsmhi.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/gscxutrgp.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/gewlhnfgm.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gkxpoeaky.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/gzjuixtew.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/ggtiulkpz.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/gususuriu.sHtML

[T40] Lua：元表
来源：http://www.blog.hesvh.cn/Article/details/gnoyblsyl.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/grxklxbcp.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/gidreffap.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gydavivgc.sHtML

[T42] Perl：变量类型
来源：http://baike.fehbvm.com/Article/details/gjurnzykh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gkejqjrkl.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gwiimoljz.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/ghylwgewm.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/geoxcvlto.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/gsdygrxvh.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/gppqqlfdu.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gnguoqfcg.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/gqvglbtbe.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/gatrpkkho.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/ghopssllp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/gdsoucghg.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/guarxahgg.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/gkdttjmyn.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/gqdhhfszi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjlldgmqc.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gezmskrxm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/girqgeulo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.zdbjq.cn/Article/details/gygcmoyvj.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/gbvrdqtks.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/grcvpeztb.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/guupzqnmm.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gskwpcvxo.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/grgltgqvw.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/ggigkwpbo.sHtML

[T54] Scala：集合映射
来源：http://www.share.hesvh.cn/Article/details/gwwjhlyby.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.zdbjq.cn/Article/details/gkblzsgqs.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gkhqoksjr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gjqaxybra.sHtML

[T56] Scala：样例类
来源：http://www.m.share.hesvh.cn/Article/details/garvolibm.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gvszwjuom.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gshlxcemv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.hesvh.cn/Article/details/gsemvjsom.sHtML

[T58] Scala：函数定义
来源：http://mobile.fehbvm.com/Article/details/gpetdicwa.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/gwpnmynqg.sHtML

[T59] Scala：循环
来源：http://3g.hesvh.cn/Article/details/gvgiblxts.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gualeltlb.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/goyddlscs.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.zdbjq.cn/Article/details/gqmmbgpdp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjdptszdb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gwskxrpki.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gimjxxgut.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/gawwalgez.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/goplgntty.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gezaauvob.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/grhdzjczb.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.zdbjq.cn/Article/details/ggtqxjmwv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/gsmtbatbp.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gyjgspicm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/ghqgqcedp.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/grnltislc.sHtML

list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gkjnidmvt.sHtML

[U06] Py：合并两个字典
来源：http://baike.zdbjq.cn/Article/details/gpkziepsp.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/gzhomrhhg.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/gpqgbpgrg.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/gowrichlo.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/gsqghccuv.sHtML

[y for x in nested for y in x]
来源：http://3g.fehbvm.com/Article/details/gphivfnmk.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.zdbjq.cn/Article/details/gxumlawmk.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/gisqspwpk.sHtML

[U10] Py：按值排序字典
来源：http://wap.fehbvm.com/Article/details/guzvcudcx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.hesvh.cn/Article/details/gafocxmlr.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/glsnjkbyr.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/goalypfzm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/gbklyjits.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gfxwipjpx.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/gunloissp.sHtML

deque(maxlen=10)
来源：http://read.share.zdbjq.cn/Article/details/gexoclphd.sHtML

[U14] Py：分组收集到列表
来源：http://blog.zdbjq.cn/Article/details/gglqqykrd.sHtML

defaultdict(list)
来源：http://m.share.fehbvm.com/Article/details/gszefihqr.sHtML

[U15] Py：高精度计时
来源：http://3g.fehbvm.com/Article/details/gxuurdlzg.sHtML

t = time.perf_counter()
来源：http://baike.zdbjq.cn/Article/details/gznjpddxw.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/gqjvrzuzn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/gxjddifvr.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gxrdjbkuh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.zdbjq.cn/Article/details/gjuepmbbl.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/gocymwauq.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fehbvm.com/Article/details/ggtuhtfoz.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/gjglhfcxf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/gskvzrfco.sHtML

[U20] Py：缓存函数结果
来源：http://wap.zdbjq.cn/Article/details/gwechfpww.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/gccpkqlho.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/gxxnehqco.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/gflxmilxp.sHtML

[U22] Py：矩阵转置
来源：http://www.share.hesvh.cn/Article/details/gmtvztwcc.sHtML

list(zip(*m))
来源：http://www.share.fehbvm.com/Article/details/glnurcqey.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gotibsywv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.zdbjq.cn/Article/details/gwcvhqypr.sHtML

[U24] Py：路径操作
来源：http://www.blog.fehbvm.com/Article/details/gnxzblcht.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gcxoseoqa.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.zdbjq.cn/Article/details/gwwaskorg.sHtML

csv.DictReader(f)
来源：http://wap.fehbvm.com/Article/details/gbjlgubok.sHtML

[U26] Py：并发下载
来源：http://wap.hesvh.cn/Article/details/gzknfokyh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/gjkwwvoeb.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.zdbjq.cn/Article/details/gdymldkds.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.hesvh.cn/Article/details/gmvhxbltb.sHtML

[U28] Py：类型别名
来源：http://3g.fehbvm.com/Article/details/gyckoknwm.sHtML

UserId = int
来源：http://m.share.fehbvm.com/Article/details/ghfoslteg.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/gxaiopucz.sHtML

@property 与 @x.setter 配合
来源：http://baike.fehbvm.com/Article/details/ggripscma.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/gpotosqae.sHtML

@dataclass(slots=True)
来源：http://blog.hesvh.cn/Article/details/gikcecgfg.sHtML

[U31] Py：单测
来源：http://blog.fehbvm.com/Article/details/gzagjiqcs.sHtML

python -m pytest -q
来源：http://3g.hesvh.cn/Article/details/gxmbhtwkj.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gbaiqmloa.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/glawfcjab.sHtML

[U33] Py：打包发布
来源：http://wap.fehbvm.com/Article/details/ghprsnqnt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.hesvh.cn/Article/details/gcvejcqlb.sHtML

[U34] Py：判断编码
来源：http://3g.hesvh.cn/Article/details/gpysuvghn.sHtML

chardet.detect(raw)
来源：http://read.share.zdbjq.cn/Article/details/gyzigcxhn.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gvyaqsbgv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.hesvh.cn/Article/details/gbvciqwyh.sHtML

[U36] Py：定时任务
来源：http://www.share.zdbjq.cn/Article/details/gntmizfct.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fehbvm.com/Article/details/gohqtpnkv.sHtML

[U37] Py：读写 Excel
来源：http://3g.fehbvm.com/Article/details/groeijafb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/gxobvuexg.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fehbvm.com/Article/details/gnuomoupl.sHtML

Path(__file__).resolve().parent
来源：http://blog.fehbvm.com/Article/details/gwvrwzofy.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.zdbjq.cn/Article/details/gljidlnbn.sHtML

sys.stdout.isatty()
来源：http://baike.hesvh.cn/Article/details/gikrzxrsu.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/ghpxsvjgo.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gmhuthvjb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.zdbjq.cn/Article/details/ghtpfwrlp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/ghxhpvgmc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/gaijrknbk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.hesvh.cn/Article/details/gutyxnasj.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/gwrjuvpxk.sHtML

namespace App\Http;
来源：http://www.blog.hesvh.cn/Article/details/ghbnvbkmm.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fehbvm.com/Article/details/gasvjzjgq.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/gdlqicxrx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fehbvm.com/Article/details/gwwbpxflt.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gunrojnlh.sHtML

[U46] PHP：可空类型
来源：http://wap.hesvh.cn/Article/details/gddotbddd.sHtML

?string $name = null
来源：http://mobile.hesvh.cn/Article/details/gilonorap.sHtML

[U47] PHP：联合类型
来源：http://m.share.zdbjq.cn/Article/details/gessoyfuh.sHtML

int|string $id
来源：http://www.share.hesvh.cn/Article/details/ggmehhlbg.sHtML

[U48] PHP：纯枚举
来源：http://m.share.hesvh.cn/Article/details/gnniebhcz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fehbvm.com/Article/details/gqzzcavqw.sHtML

[U49] PHP：只读属性
来源：http://read.share.fehbvm.com/Article/details/gvgwxejhw.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gnezwlvam.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fehbvm.com/Article/details/gptazbasg.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fehbvm.com/Article/details/gtaedihwk.sHtML

[U51] PHP：数组解构
来源：http://mobile.fehbvm.com/Article/details/gptuwckvx.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/gjkekcjxp.sHtML

[U52] PHP：箭头函数
来源：http://wap.hesvh.cn/Article/details/gmrstgvef.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.hesvh.cn/Article/details/gmcpsximp.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gojuwddrg.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/gdxwyjeex.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fehbvm.com/Article/details/gyafstsco.sHtML

$obj?->method()
来源：http://mobile.hesvh.cn/Article/details/gdvahdkgj.sHtML

[U55] PHP：match 表达式
来源：http://blog.hesvh.cn/Article/details/gakojgbkk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/gorragfpy.sHtML

[U56] PHP：命名参数
来源：http://mobile.zdbjq.cn/Article/details/gjgrsnhde.sHtML

f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/glfodzmht.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gdzqspwqh.sHtML

"值: {$a}"
来源：http://3g.hesvh.cn/Article/details/gsoehaadu.sHtML

[U58] PHP：数组三件套
来源：http://mobile.hesvh.cn/Article/details/gitkzggqa.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.hesvh.cn/Article/details/gvsywdyga.sHtML

[U59] PHP：自定义排序
来源：http://read.share.zdbjq.cn/Article/details/ghlcilyct.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gocxphsmd.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.zdbjq.cn/Article/details/ggplyuqan.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.hesvh.cn/Article/details/gvufuwnpb.sHtML


<!-- 参考信息 -->