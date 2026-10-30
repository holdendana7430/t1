代发 wailian999

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gqpubgujg.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/glmvbjjql.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gvzrmsvtb.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/grybyjzid.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gouyoxdni.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/gkmjrombe.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/gwbuptdfx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/ggxeglccp.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gppycnuqd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gzixjiyue.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gneijspgf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gtkvovgzy.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gseeakhbl.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gzbicqdnf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/glfglnnsa.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/guipqxhgw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gqahdnnhj.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gcwqduadq.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gynltaatf.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/ghpfybsfv.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/glhsbntla.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gebdtkzwn.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/gkyitvwhp.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gsrygxbmf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gsreqmnca.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gytwjcphz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gcddgdoab.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gvgvicjky.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/gukieascy.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gwiwuglqv.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gezzkiewv.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gtfsgodeb.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/ggrlaousd.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/givtoevvg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gvvrhrnnp.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gjsjmsfmy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gixcdjixu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbyiyzuks.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gqqflxbnw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkucyejdu.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gfgzgbfnk.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gioydossa.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/gmwcdjwxz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gfjnhzjng.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gzzieiszd.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gkroikzgc.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gjkrjyzkr.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gelfluyro.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gwmmvupri.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/glpawpzrj.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gsnrgyjnr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gocpacoqn.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/grjhjeeyd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/gbvxqbyji.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gwsyzwasl.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/glbwocxha.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gawbxsdew.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gfhmrctaf.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gjrxiezfi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gutoezihv.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/ghcemwlif.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/gosateneg.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/guoyaeioh.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/gwwqmyfjx.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gzwrmaajf.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gqhclckew.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/gnqiugcgz.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gxjfmqtdf.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/gczufcuru.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/ghprdrifm.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/gwgbugcdh.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gjcfdcdmt.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/gxtvxiakp.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gwjxuaiyx.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/glojmiumz.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/gfkoufcrx.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fehbvm.com/Article/details/gakholcal.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/gmnkyscxf.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/gfmhtdbis.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gxlagztyy.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/ghpnrcoyx.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/grsyaactc.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/gampdlwvn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/ghzaruowg.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gtsbrxeqh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/gooplwxem.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gxwhesrho.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gckmclzxh.sHtML

[T25] Swift：结构体
来源：http://3g.zdbjq.cn/Article/details/gxcvdltba.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gyeiutnoe.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/gssaoiybd.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gpuypepkp.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/geoqbdzvd.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fehbvm.com/Article/details/gdsugupkz.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/gawktsbqx.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gstusjpob.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gkjpywwdp.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gmlyrgpgx.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/ggqwviqor.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gellywrsz.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gvenlbyua.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/giunnhfpg.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gokmlsqud.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gafssvlmu.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/gsmerzuqj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.zdbjq.cn/Article/details/gordkwvrj.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/gdqqkihbv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/gsbceqwoi.sHtML

[T35] Lua：字典表
来源：http://m.share.fehbvm.com/Article/details/gjdqcwzbl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gccvnklrq.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gsrwuvjve.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gypqgiyvz.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gmjjppvxa.sHtML

"a" .. "b"
来源：http://www.blog.hesvh.cn/Article/details/goqohiszg.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/golnzljze.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/goflbonqp.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gznhubvzp.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/gsxzpptrx.sHtML

[T40] Lua：元表
来源：http://www.blog.fehbvm.com/Article/details/gujnhgczw.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/gfmkqotis.sHtML

[T41] Perl：Hello World
来源：http://www.share.hesvh.cn/Article/details/gjqrhynrp.sHtML

print "Hello\n";
来源：http://mobile.hesvh.cn/Article/details/glvkaypxy.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/gczadmgtj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.hesvh.cn/Article/details/gbuqntgjs.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gyzhezrtw.sHtML

"值: $a"
来源：http://blog.hesvh.cn/Article/details/gbftzqrkw.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/grxwnaxjl.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/gxwvivqac.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/gcowagfns.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/gucotqmzo.sHtML

[T46] Perl：哈希操作
来源：http://wap.zdbjq.cn/Article/details/gigakmxzw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fehbvm.com/Article/details/gajevwjhf.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/gvqsuogrc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/gbvgifevw.sHtML

[T48] Perl：正则替换
来源：http://mobile.fehbvm.com/Article/details/girejeomq.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fehbvm.com/Article/details/gvbpgwskz.sHtML

[T49] Perl：函数
来源：http://baike.fehbvm.com/Article/details/gedcptkfh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gvqieohcv.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/ganunvthp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/goufjqerg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gbcdinyhs.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gktjcfqyg.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gngmycicx.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/gdbnunekn.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/ghlpfqbcd.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gudghylfq.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gsxkfrljb.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gjlhniemr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/gehiprdig.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gexcopbqk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.hesvh.cn/Article/details/gvdgvnpcm.sHtML

[T56] Scala：样例类
来源：http://www.share.hesvh.cn/Article/details/gwikfqrqo.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gazdmaxli.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gocfyaldg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gmnidplue.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fehbvm.com/Article/details/grtglyxip.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/gmspddtck.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/guaikksva.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/gyexluuah.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/gvksfljuw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.zdbjq.cn/Article/details/gajnkrnfg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gekbenarg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/ghanacnyv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/goipbgtqx.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gcotwlmbr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/gbdwfivsd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/gvmwkmqwz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/gktkhxbnh.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fehbvm.com/Article/details/gtegifyzn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gmmcbwvdo.sHtML

[U04] Py：变量调试打印
来源：http://wap.hesvh.cn/Article/details/gwfmefcjz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/ggxllrffx.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/gbuwjkaaf.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gcwevagtr.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/geagaqwzp.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gtvjlusxp.sHtML

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/ghavupnuq.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gwfldfxqk.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.hesvh.cn/Article/details/gqjulfqke.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/gbcktikul.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gfqspkhgd.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/grfydxewm.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fehbvm.com/Article/details/gctqkytlc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/gzrqgppci.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/gjeljaqof.sHtML

(x * 2 for x in arr)
来源：http://wap.zdbjq.cn/Article/details/ghivnvmeo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/gkwkfeghf.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fehbvm.com/Article/details/grswsgife.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/gjckvough.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/gpvwulfvb.sHtML

[U14] Py：分组收集到列表
来源：http://baike.zdbjq.cn/Article/details/gtzmgfvpm.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/gmlrlebwb.sHtML

[U15] Py：高精度计时
来源：http://m.share.hesvh.cn/Article/details/gsirudzzn.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/gjcnhjkdz.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/gvmprqwng.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.hesvh.cn/Article/details/gfplcfaaa.sHtML

[U17] Py：初始化日志
来源：http://www.share.fehbvm.com/Article/details/gknocllkc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/gkdujhpqr.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/gsallvdoc.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/glofvmkqn.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.hesvh.cn/Article/details/gldyaljbi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/geqglagxf.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/gudugszbn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.hesvh.cn/Article/details/gewzjeuxa.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fehbvm.com/Article/details/gfcydxpuh.sHtML

@contextlib.contextmanager
来源：http://blog.hesvh.cn/Article/details/glntdqapd.sHtML

[U22] Py：矩阵转置
来源：http://baike.zdbjq.cn/Article/details/gekamndou.sHtML

list(zip(*m))
来源：http://3g.zdbjq.cn/Article/details/gwyhwwibc.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/gervuwjdk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/gorayhbwi.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/gpqzolelo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gmhwefcym.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fehbvm.com/Article/details/gzzqecdjz.sHtML

csv.DictReader(f)
来源：http://m.share.zdbjq.cn/Article/details/gggnwjzhb.sHtML

[U26] Py：并发下载
来源：http://www.share.fehbvm.com/Article/details/ggqnzemwf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/gvtunvicv.sHtML

[U27] Py：异步 HTTP
来源：http://3g.hesvh.cn/Article/details/gesopvjhc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/gwomquwti.sHtML

[U28] Py：类型别名
来源：http://3g.fehbvm.com/Article/details/gfjngddlq.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/gfhzrudqk.sHtML

[U29] Py：属性校验
来源：http://baike.fehbvm.com/Article/details/gjqnobbmg.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/gflgwgrba.sHtML

[U30] Py：数据类
来源：http://blog.hesvh.cn/Article/details/ggtduumkf.sHtML

@dataclass(slots=True)
来源：http://www.share.zdbjq.cn/Article/details/ggmzkriqy.sHtML

[U31] Py：单测
来源：http://www.share.hesvh.cn/Article/details/gqvvgvzof.sHtML

python -m pytest -q
来源：http://3g.fehbvm.com/Article/details/grhnsaket.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gxtjgngnv.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.hesvh.cn/Article/details/gibgfeucj.sHtML

[U33] Py：打包发布
来源：http://wap.hesvh.cn/Article/details/gzvzbfuzi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.zdbjq.cn/Article/details/gcfnjsaru.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/gmrplruuc.sHtML

chardet.detect(raw)
来源：http://www.blog.fehbvm.com/Article/details/gymkzrkci.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/gbnmuzfyb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.zdbjq.cn/Article/details/gdtfamdmb.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/ggrwkemak.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.zdbjq.cn/Article/details/gzrpezwnq.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fehbvm.com/Article/details/gmanyrasf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.hesvh.cn/Article/details/gvowvizzf.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fehbvm.com/Article/details/gpeldstmp.sHtML

Path(__file__).resolve().parent
来源：http://m.share.hesvh.cn/Article/details/grxzqpmfw.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fehbvm.com/Article/details/gnqwbwmet.sHtML

sys.stdout.isatty()
来源：http://blog.zdbjq.cn/Article/details/gkkcduqtu.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.hesvh.cn/Article/details/glujwqfuo.sHtML

print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gsulcwiao.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.zdbjq.cn/Article/details/gfrkawhin.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.zdbjq.cn/Article/details/ggktrwkmc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/gvrburxzs.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/gqjgxklwp.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gciuhwfby.sHtML

namespace App\Http;
来源：http://mobile.zdbjq.cn/Article/details/ggvkmsdmi.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.hesvh.cn/Article/details/gzzlmvgto.sHtML

declare(strict_types=1);
来源：http://www.share.hesvh.cn/Article/details/gzborlxmw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/gzwaikmyh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gxhnelfeb.sHtML

[U46] PHP：可空类型
来源：http://blog.fehbvm.com/Article/details/ggissjvyn.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/grhocmlya.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/gllicdkse.sHtML

int|string $id
来源：http://m.share.hesvh.cn/Article/details/gkhsduvkn.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fehbvm.com/Article/details/gqrcdufby.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/gldpmlugl.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/glnzwkyfx.sHtML

public readonly string $name
来源：http://www.share.hesvh.cn/Article/details/gcnaumuli.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.zdbjq.cn/Article/details/grplrwqsz.sHtML

public function __construct(private int $id) {}
来源：http://wap.zdbjq.cn/Article/details/gneqjidxz.sHtML

[U51] PHP：数组解构
来源：http://read.share.fehbvm.com/Article/details/ggyuqahvk.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/gfxesweyb.sHtML

[U52] PHP：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gyqvbjvuj.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fehbvm.com/Article/details/gafajgnzl.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/gcruylkrk.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fehbvm.com/Article/details/gwptqxhgd.sHtML

[U54] PHP：空安全调用
来源：http://3g.hesvh.cn/Article/details/gvlvsjrit.sHtML

$obj?->method()
来源：http://blog.fehbvm.com/Article/details/ggflwkqmh.sHtML

[U55] PHP：match 表达式
来源：http://mobile.zdbjq.cn/Article/details/gpzbawwcy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gxdidvnft.sHtML

[U56] PHP：命名参数
来源：http://blog.fehbvm.com/Article/details/gfyoszpaa.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/ggzklmlvj.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/gydpbdcro.sHtML

"值: {$a}"
来源：http://read.share.zdbjq.cn/Article/details/gtltntold.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fehbvm.com/Article/details/goplyluno.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fehbvm.com/Article/details/gqdorvcca.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fehbvm.com/Article/details/gxrqaplfg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gxabiizkb.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.zdbjq.cn/Article/details/gwzrlkqqw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.hesvh.cn/Article/details/gezxzrzgr.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/gwegfwgev.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gkzzxvrcd.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fehbvm.com/Article/details/gidqaahlv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/geidqheml.sHtML

[U63] PHP：文件读写
来源：http://www.blog.hesvh.cn/Article/details/gzpzbxvei.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/gemciztld.sHtML

[U64] PHP：目录遍历
来源：http://baike.hesvh.cn/Article/details/gncsnorjs.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.zdbjq.cn/Article/details/gshhxgenr.sHtML

[U65] PHP：会话
来源：http://www.m.share.fehbvm.com/Article/details/gljqnoimj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.zdbjq.cn/Article/details/glwftrrhg.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.zdbjq.cn/Article/details/gyptxzwxw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.hesvh.cn/Article/details/gcpvddtcg.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/gagbsnzja.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.hesvh.cn/Article/details/gtuexneco.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.zdbjq.cn/Article/details/gsmjfdhzw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.hesvh.cn/Article/details/gsvwuvcyh.sHtML


<!-- 参考信息 -->