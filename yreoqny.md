代发 wailian999

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/gccmeohyi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/guolngutg.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/glyutqeal.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gubmtpidg.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gsunhsnvp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gmwzknlvh.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gxhgdqluj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/geyifrtwt.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gavjpybkg.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/gnwaceoqh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/gfxnixaxj.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gnfjpcrlg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/grfkcowla.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/gwfltybhl.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/gsrtgncfr.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gwcsgnagt.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gjdjclaag.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/ghhmfmqkz.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/ghvpoqszd.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/gxsjtrymc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gvqvuyfqr.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/ggkxdivod.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gvwzxhexs.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/glupzeplj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gfdjbshhn.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gwepygtez.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/gurlzfylo.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gjomezxpe.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gxkyxpvlt.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gfpnsjqfy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gjbkyvomy.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gsuytpskj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gprqdgwzl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gicpzxgxs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gnzepjnbc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvrazrieq.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gdtcerhwm.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gexgjxwkh.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gbknsbgcz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gwswxsghw.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gsufiivgc.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gdipooqdj.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gcxnoxsir.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gmrgiayto.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/ggvdvosmm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/gjveaxuas.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/gfribgwdr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/gspdelmom.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gnfqtjxob.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gyfgjrljc.sHtML

[T08] Kotlin：数据类
来源：http://www.share.hesvh.cn/Article/details/glfbudmnt.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/ghxpxqxir.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gxxjictll.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gftoekttn.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/ggixsiehn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gjniwvntj.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/gobdfckin.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gxpalvsxh.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/gmtgffwfc.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gappbsqdt.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/gyjloqcsb.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/gxsfeofqp.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gebnxheis.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gkztmljro.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gpylnynfh.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/gpuhxfeix.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gnwtcqvlr.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gtprmfzht.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gmnlzvtkz.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/gfqnscuqd.sHtML

[T18] Swift：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gqnwbgfrt.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/ghbtjqpyi.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gfgaeyafr.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/gpcpyhlao.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/gxqjumkjc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gknnckqve.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gtamlmwjn.sHtML

for x in a { print(x) }
来源：http://www.share.zdbjq.cn/Article/details/gwrhahagj.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gilhzhyeu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/gbtapyuqz.sHtML

[T23] Swift：函数
来源：http://3g.zdbjq.cn/Article/details/gyrvptfsd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/gzwiknpvf.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gqoldpydt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gsiovarvr.sHtML

[T25] Swift：结构体
来源：http://m.share.zdbjq.cn/Article/details/gvsgdhjon.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/gfemfdlbm.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/gshxomyen.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/gadkjocil.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gpywilapz.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/gytfpgald.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gqtqsyydt.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gmfacypef.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fehbvm.com/Article/details/gyiukdljb.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/gvibuiytg.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/gfkjcxtjd.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.zdbjq.cn/Article/details/gofkcwzng.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/ggzqmjerm.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/goxcfedzf.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gcccykctm.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/gfpecsgxw.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gqahdfidx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fehbvm.com/Article/details/guillvhxm.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/gegnvpwlt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/guejwgfcs.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gexlxkvwe.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/gbohdhzpi.sHtML

[T36] Lua：函数
来源：http://m.share.zdbjq.cn/Article/details/gfektcdkh.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/gsedwxmrg.sHtML

[T37] Lua：字符串拼接
来源：http://wap.hesvh.cn/Article/details/ghyeaitwm.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/gkxxvivrx.sHtML

[T38] Lua：条件
来源：http://www.blog.zdbjq.cn/Article/details/gdqpfhikp.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/gljbhwcxg.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gehydiedq.sHtML

string.find(s, "%d+")
来源：http://www.blog.fehbvm.com/Article/details/gessjsgmx.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/gpvvoczqb.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gyqveyanm.sHtML

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/gxgaucebs.sHtML

print "Hello\n";
来源：http://www.blog.fehbvm.com/Article/details/ggkqeexyf.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gzxuimpld.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.zdbjq.cn/Article/details/gszprjhin.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gqxsanrgh.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/gqkfqzdxi.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/gjgisxtrp.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/gbnhwwsnt.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/gchuoarln.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/ggarwirnt.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/gvrnxaruy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.hesvh.cn/Article/details/gqdaanjgp.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/gobhahxgm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/gtzdnernd.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gjoygfxrl.sHtML

$s =~ s/old/new/g;
来源：http://baike.fehbvm.com/Article/details/geruokdkh.sHtML

[T49] Perl：函数
来源：http://m.share.fehbvm.com/Article/details/grlcrbkud.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/guudborir.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gfffrcgmt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/guhpxcfdr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.hesvh.cn/Article/details/gwnfppybx.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gbincvevr.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gkrsgvzhf.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/gvmfwnscj.sHtML

val a = 1;  var b = 2
来源：http://read.share.fehbvm.com/Article/details/gabahnztc.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gfjysptmr.sHtML

s"值: $b"
来源：http://mobile.hesvh.cn/Article/details/ginesagkk.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gskiqsxcn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/gwmtoxrhf.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gfvdqcbra.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.hesvh.cn/Article/details/ghkbzqoiy.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/gcpbthrfi.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gsrvvwpbq.sHtML

[T57] Scala：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gfiqgyvjr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/gmvplxyyx.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fehbvm.com/Article/details/gqgbhfdze.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/gkokvslfy.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/gldkhzpnz.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/glwomimgz.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/gmjdqimey.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/ghvdnfwxz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcricacjr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gjiuydvvr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmtltyxpl.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/gigfiudjr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/grmkyxqbi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.zdbjq.cn/Article/details/gsmllpkei.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/glensqaoq.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fehbvm.com/Article/details/gjxetyrex.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/gjqznnaui.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/gresswrzq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/giymnglru.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gracupimj.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/glxnmccli.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/grfeaapha.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/gicoofnny.sHtML

[U07] Py：反转字典键值
来源：http://m.share.hesvh.cn/Article/details/gqcgosiwe.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fehbvm.com/Article/details/gyloeajks.sHtML

[U08] Py：展平二维列表
来源：http://www.share.zdbjq.cn/Article/details/gdlsmjsoe.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/guufsyhpw.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.hesvh.cn/Article/details/gpxhniiul.sHtML

max(d, key=d.get)
来源：http://www.share.fehbvm.com/Article/details/gtpglmtcw.sHtML

[U10] Py：按值排序字典
来源：http://mobile.hesvh.cn/Article/details/gidrxgofu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.hesvh.cn/Article/details/guuauiith.sHtML

[U11] Py：生成器表达式
来源：http://blog.zdbjq.cn/Article/details/gdahwxakx.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/grqmsrwfa.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fehbvm.com/Article/details/gdbcryofj.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/godykirur.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fehbvm.com/Article/details/gbeyredld.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/gltgegyxn.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fehbvm.com/Article/details/gliocsiyd.sHtML

defaultdict(list)
来源：http://www.blog.fehbvm.com/Article/details/gghzmavto.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gsjvzcxwo.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/ggxmfpboe.sHtML

[U16] Py：命令行参数解析
来源：http://3g.hesvh.cn/Article/details/gxovkqncf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/gksvpyiih.sHtML

[U17] Py：初始化日志
来源：http://blog.fehbvm.com/Article/details/gmbxggcgj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.hesvh.cn/Article/details/gdqdqrvhc.sHtML

[U18] Py：预编译正则
来源：http://wap.fehbvm.com/Article/details/gahiwrbha.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/galwbbbdd.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/gnxuroqhx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fehbvm.com/Article/details/gcdpaoxnh.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/gvutbfejp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fehbvm.com/Article/details/gchhivbag.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/gvlavsvns.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/gmohsipse.sHtML

[U22] Py：矩阵转置
来源：http://m.share.hesvh.cn/Article/details/grlyjhwtw.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/gylcjocbj.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/gcdmbklnc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.zdbjq.cn/Article/details/gcgbdboiq.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/gvbtiivgy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gfhxfukja.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fehbvm.com/Article/details/gpyizysio.sHtML

csv.DictReader(f)
来源：http://baike.fehbvm.com/Article/details/gmmkqvxge.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/glkhoermq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/gohenysas.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/gorxltnur.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.hesvh.cn/Article/details/ggfnaffza.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/gcmgjoskc.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/ggzvedack.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/gfsalodlq.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/gnwilngeg.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/gcjbnwjwj.sHtML

@dataclass(slots=True)
来源：http://wap.zdbjq.cn/Article/details/gfjsdsecy.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/guikwrpxh.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/gmeulrikx.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/ggzgrxzjj.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fehbvm.com/Article/details/gtuaycwsq.sHtML

[U33] Py：打包发布
来源：http://3g.zdbjq.cn/Article/details/gebbqqkcr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/gwiexqjdn.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/ghaydthws.sHtML

chardet.detect(raw)
来源：http://www.m.share.zdbjq.cn/Article/details/gdxgxzctx.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/govrgbvsz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fehbvm.com/Article/details/gpgoifpgn.sHtML

[U36] Py：定时任务
来源：http://wap.zdbjq.cn/Article/details/gcxezxshz.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.zdbjq.cn/Article/details/gvhtjtdtx.sHtML

[U37] Py：读写 Excel
来源：http://m.share.zdbjq.cn/Article/details/gnurzepje.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gbizcupaz.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fehbvm.com/Article/details/gqziyqfja.sHtML

Path(__file__).resolve().parent
来源：http://baike.hesvh.cn/Article/details/gnrxukszt.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fehbvm.com/Article/details/ghwrcmscz.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/grqhxntqj.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.zdbjq.cn/Article/details/gmatjmbut.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gfzjwctxs.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.zdbjq.cn/Article/details/gznxapism.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.hesvh.cn/Article/details/goiibgqai.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.zdbjq.cn/Article/details/gtyywlmrn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/gcxejwyoe.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gbvgdpdfp.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/ghcopohrx.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fehbvm.com/Article/details/gzryvkyoc.sHtML

declare(strict_types=1);
来源：http://baike.hesvh.cn/Article/details/gbpimqmzs.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/gioyxepew.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gpnglehrs.sHtML

[U46] PHP：可空类型
来源：http://baike.fehbvm.com/Article/details/ghobxzvhz.sHtML

?string $name = null
来源：http://www.blog.hesvh.cn/Article/details/gduyvigee.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/gelxrjdee.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/gywfolodb.sHtML

[U48] PHP：纯枚举
来源：http://read.share.zdbjq.cn/Article/details/gxakpemdn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.zdbjq.cn/Article/details/gdldpdeiv.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/glinrmzpn.sHtML

public readonly string $name
来源：http://blog.zdbjq.cn/Article/details/gfluinfpx.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.zdbjq.cn/Article/details/gvazfkmlv.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fehbvm.com/Article/details/giatdbfwp.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/gqromxlot.sHtML

[$a, $b] = $arr;
来源：http://baike.hesvh.cn/Article/details/gndhxylvk.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gwowcvgsm.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gjynwgwur.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fehbvm.com/Article/details/gvlykamuh.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.zdbjq.cn/Article/details/gsdshcwsz.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/gowfirxsb.sHtML

$obj?->method()
来源：http://baike.zdbjq.cn/Article/details/grymilgyy.sHtML

[U55] PHP：match 表达式
来源：http://mobile.zdbjq.cn/Article/details/gxbjgdilz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gjhuxmacq.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fehbvm.com/Article/details/griwiagel.sHtML

f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gqwsolsra.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/gkcxtwzhu.sHtML

"值: {$a}"
来源：http://read.share.zdbjq.cn/Article/details/ghkhqegqd.sHtML

[U58] PHP：数组三件套
来源：http://blog.zdbjq.cn/Article/details/gwtgqfseq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.zdbjq.cn/Article/details/glieevluu.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.zdbjq.cn/Article/details/gaebhzcrf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gfaeqopur.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/gxopklban.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.hesvh.cn/Article/details/gmeqdvmgd.sHtML

[U61] PHP：正则
来源：http://www.m.share.hesvh.cn/Article/details/gfzpyfqeu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gbbuzjjgt.sHtML

[U62] PHP：日期对象
来源：http://3g.fehbvm.com/Article/details/ggdhceslb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.zdbjq.cn/Article/details/gqgfnmpwt.sHtML

[U63] PHP：文件读写
来源：http://3g.fehbvm.com/Article/details/gjtfqfzuc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.hesvh.cn/Article/details/gwjarsrdq.sHtML

[U64] PHP：目录遍历
来源：http://m.share.zdbjq.cn/Article/details/gpgeyvghs.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.hesvh.cn/Article/details/ghohpaulh.sHtML

[U65] PHP：会话
来源：http://www.share.hesvh.cn/Article/details/gayugslqf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.hesvh.cn/Article/details/gkrbyhrle.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/gevocpkiv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fehbvm.com/Article/details/gdckchfwf.sHtML

[U67] PHP：处理文件上传
来源：http://3g.hesvh.cn/Article/details/gnefpoyws.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/gscatlbdp.sHtML

[U68] PHP：PDO 连接
来源：http://baike.zdbjq.cn/Article/details/ghglxzemc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.zdbjq.cn/Article/details/gyjmkcski.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fehbvm.com/Article/details/gpnoijkye.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.hesvh.cn/Article/details/gfexrdtqb.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.zdbjq.cn/Article/details/gitfzfkbv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.zdbjq.cn/Article/details/gmbieason.sHtML


<!-- 参考信息 -->