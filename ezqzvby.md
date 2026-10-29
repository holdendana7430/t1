代发 wailian999

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/ggamwgdiz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gneyhhcug.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gpwadxjxg.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gacmgthat.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gvznaojge.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/gdelhgmmo.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gjcxxrfsb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gxtbzonsi.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/gknzrsqku.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gyrralmzw.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmdukpjqt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/gugrnkyca.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gwzloznfo.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gzhcqjzbh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/gqbhbtkrh.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gqanvgnud.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gznadaizs.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/gkeytyzhy.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/gauwczczr.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gmqdhtxto.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/ghwuqlnfd.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/grulaezqe.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/ghcuhpiqs.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gfexfjujz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gmrxgwlqs.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/goxiahoff.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gzlezyjgn.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/ghwjgvifw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/grvxeqsam.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/giflraseu.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/gztrsxtzf.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/ganrdjvey.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/gdmjasggq.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/ghspfjhva.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gicxkbste.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gpvufxnfq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/gbjqnyvtw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glelfswco.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gykrbkrru.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwcdlfrir.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gmamqkgdy.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gknvgcgon.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/gfakysiim.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/gkwgzqwyb.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gdprxjavn.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gpvshrcxe.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gsnhklppj.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/glhqiauqb.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gxbvswkgk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/griiwkmvz.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gnfqiijxx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/gdtpsxurx.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gkmjqvroh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gpmsfvsvz.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/guwyltknr.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/gltwmvrok.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/gongtydse.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gjnmfqinn.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/gvjllrebb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/gvdmdoziy.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/gvcqolkon.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gaahppsod.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gpcgeywmz.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gyaagbswo.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gohewnhkb.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/gnvhlcsgf.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gqpsjmiew.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gcgtscutk.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gawlxnfjb.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.zdbjq.cn/Article/details/guhovvzyk.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/ghccsbgnr.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gsnvuinje.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gotrqoash.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gpwemyewr.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gkkyumjps.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/getbdacku.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gzlkcpsdg.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/gmffwoisi.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/gofflhsrq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/gpstxcjcq.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gtjrbylds.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/ghedzexri.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gxedmixto.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gjenczcbm.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/gboxndhgu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/gzacmlxxk.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/gjnwizvuv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gdlvmwvxd.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/gkpojqbdo.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/gjexjcxov.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/ghwjtssgo.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/giqsybfvj.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/gccbgsbzz.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/gjwumdhgd.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gnbjjxiuv.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/gmsvbrfvv.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/ghpfupqnl.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/ghjhhdfvh.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/givkszhxs.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.hesvh.cn/Article/details/gkyryxjez.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gifxyqzwc.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gzmaegjxw.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gplbwempz.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/glfmzijcl.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gbjcnpqzx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/gtysggesv.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gcfntkyag.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fehbvm.com/Article/details/ggbatekcc.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/gypfkhfpy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/ggglafknx.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/gfcxzbygj.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/gekwwwgrx.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gobjzlpvw.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/gvkowhopo.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/gpercmhbk.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/grcajjgbo.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/gfrnjsjcj.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/gpijwdgdf.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/grssyuxux.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/gofbjtbro.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/gxlwzfqvz.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/ggggpknjf.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/gmlrekien.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fehbvm.com/Article/details/grkzqwmau.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gkzpbuamw.sHtML

"值: $a"
来源：http://www.m.share.hesvh.cn/Article/details/gsstmzncv.sHtML

[T44] Perl：条件
来源：http://3g.hesvh.cn/Article/details/ghshddtsy.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fehbvm.com/Article/details/gdlwouthr.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/glpyxhwnp.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/gnfglnnch.sHtML

[T46] Perl：哈希操作
来源：http://m.share.zdbjq.cn/Article/details/golymyrih.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gvxvadkyb.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/gkjmgcien.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/gwbexzymi.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fehbvm.com/Article/details/grfojtviy.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/gmlsbxbvp.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/gqykltape.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gfojgdaqy.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/grljoomrp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fehbvm.com/Article/details/glxalyyks.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gtmgansqg.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gaaciczsw.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gfcbqsqfc.sHtML

[T52] Scala：变量
来源：http://www.share.hesvh.cn/Article/details/gtgvzymjc.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gbanzsvsm.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/geppefmwn.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gbphccqwb.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gqnmoanux.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.hesvh.cn/Article/details/gfepxikls.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gbmrresyr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/gjvkwcxqv.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/gnhrxydrr.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gzzdcnapa.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gixfnqhox.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/ghpsvbezo.sHtML

[T58] Scala：函数定义
来源：http://read.share.fehbvm.com/Article/details/gwmfncgly.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/ggcnmwefj.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gkcqduibi.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gbtknosmy.sHtML

[T60] Scala：折叠
来源：http://blog.zdbjq.cn/Article/details/gvdahxwgv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/gnrjydmeq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcwctkxil.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/gpumyhido.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbxxxjisb.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/gwjsjtqye.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/gkbjsmszz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fehbvm.com/Article/details/gvnkujfqo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.zdbjq.cn/Article/details/ghqwcvvjm.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fehbvm.com/Article/details/gugqwddtb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.zdbjq.cn/Article/details/gkugzsgcc.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/gewuhiwod.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gpfninfsg.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fehbvm.com/Article/details/gjjbynlse.sHtML

list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gucnajbzw.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/gvnihxzvx.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/ggmbvgynl.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.hesvh.cn/Article/details/guxumvimz.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/gggokjepe.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/gfftibglq.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/gieublufm.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.zdbjq.cn/Article/details/gvvimhxsx.sHtML

max(d, key=d.get)
来源：http://mobile.zdbjq.cn/Article/details/gavjollfl.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/gwosfwmkm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.zdbjq.cn/Article/details/gmdssodof.sHtML

[U11] Py：生成器表达式
来源：http://wap.fehbvm.com/Article/details/gifafwemo.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/ggmewmfqd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/ggmlvgsoz.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/gzfznoxwq.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/gdqetepkk.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/gauryktwg.sHtML

[U14] Py：分组收集到列表
来源：http://baike.zdbjq.cn/Article/details/ggvuvvdph.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/gztsophuw.sHtML

[U15] Py：高精度计时
来源：http://wap.zdbjq.cn/Article/details/goewiodwp.sHtML

t = time.perf_counter()
来源：http://m.share.zdbjq.cn/Article/details/gghmfyuzt.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/gpepqylmk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/gtocvgypk.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/gjhpvdmhy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gyxcexzfc.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/gpcstlhtv.sHtML

pat = re.compile(r"\d+")
来源：http://baike.zdbjq.cn/Article/details/goscaehkz.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fehbvm.com/Article/details/goapzbuzk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fehbvm.com/Article/details/gcdxqyxtk.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.hesvh.cn/Article/details/gkdedpkba.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/gspaxhypn.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.hesvh.cn/Article/details/grjoljnmd.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/gebsltmyb.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gvfjfzzjz.sHtML

list(zip(*m))
来源：http://mobile.fehbvm.com/Article/details/gxletejvd.sHtML

[U23] Py：分块读取大文件
来源：http://baike.hesvh.cn/Article/details/gfllcmxyg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fehbvm.com/Article/details/gvwzhhlug.sHtML

[U24] Py：路径操作
来源：http://blog.zdbjq.cn/Article/details/gjrsklkww.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gowxbupdf.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/gkevhtmaw.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/gkrcyljrn.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/gniyxtdjj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/gxdbbckaj.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gqtzdyuov.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/gionkwaty.sHtML

[U28] Py：类型别名
来源：http://3g.zdbjq.cn/Article/details/gmcbxfxjn.sHtML

UserId = int
来源：http://wap.fehbvm.com/Article/details/gzlyfajdl.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/gflrsoraq.sHtML

@property 与 @x.setter 配合
来源：http://3g.fehbvm.com/Article/details/gvhrybbfl.sHtML

[U30] Py：数据类
来源：http://www.blog.fehbvm.com/Article/details/gprifpbcj.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/ghlfklabq.sHtML

[U31] Py：单测
来源：http://mobile.zdbjq.cn/Article/details/gwzoidtpz.sHtML

python -m pytest -q
来源：http://baike.fehbvm.com/Article/details/gcwlsqggi.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gobtpbkfo.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/glzcyyexg.sHtML

[U33] Py：打包发布
来源：http://baike.zdbjq.cn/Article/details/goxjzqzks.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.hesvh.cn/Article/details/gkdmvzrym.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/gsfmkjwqr.sHtML

chardet.detect(raw)
来源：http://blog.hesvh.cn/Article/details/glyccdlyf.sHtML

[U35] Py：发送邮件
来源：http://read.share.zdbjq.cn/Article/details/gtpdchxzr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/gpetjqjdd.sHtML

[U36] Py：定时任务
来源：http://baike.hesvh.cn/Article/details/gwfsshfjg.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/grubejmcz.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fehbvm.com/Article/details/gxelemhhr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.hesvh.cn/Article/details/gqafsptwm.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.hesvh.cn/Article/details/gxwayilti.sHtML

Path(__file__).resolve().parent
来源：http://read.share.zdbjq.cn/Article/details/gqrhmglct.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/gqawsknvb.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/gxccehxnd.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gdwnhcnri.sHtML

print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gertnamma.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fehbvm.com/Article/details/gqbodwlro.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/gfzziwtlv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gubpeatuc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fehbvm.com/Article/details/goapmdxmw.sHtML

[U43] PHP：声明命名空间
来源：http://blog.hesvh.cn/Article/details/gudiiwzlp.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/gokamdomg.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gfruslsch.sHtML

declare(strict_types=1);
来源：http://wap.hesvh.cn/Article/details/gwjarfkad.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.hesvh.cn/Article/details/gpuingoqc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gpnszerkv.sHtML

[U46] PHP：可空类型
来源：http://www.share.fehbvm.com/Article/details/gxlcqnibu.sHtML

?string $name = null
来源：http://m.share.fehbvm.com/Article/details/gtdzifxsq.sHtML

[U47] PHP：联合类型
来源：http://wap.hesvh.cn/Article/details/getdvcorm.sHtML

int|string $id
来源：http://read.share.hesvh.cn/Article/details/ghltfyfgo.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/gawjdegeb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/gkvynzqov.sHtML

[U49] PHP：只读属性
来源：http://read.share.zdbjq.cn/Article/details/gmidfbyyd.sHtML

public readonly string $name
来源：http://mobile.hesvh.cn/Article/details/gfsgiqwtl.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.zdbjq.cn/Article/details/gbscxiuou.sHtML

public function __construct(private int $id) {}
来源：http://wap.hesvh.cn/Article/details/gbkzhbtgh.sHtML

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/geqzyhxdy.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/gmslncckx.sHtML

[U52] PHP：箭头函数
来源：http://baike.hesvh.cn/Article/details/gojdbjutj.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/gtlgzabsf.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/gtkwyeiwi.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.hesvh.cn/Article/details/gjeiaertt.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/gtwgwftjn.sHtML

$obj?->method()
来源：http://www.m.share.zdbjq.cn/Article/details/gxvzxswgm.sHtML

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/glkyqknrr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fehbvm.com/Article/details/geydizgil.sHtML

[U56] PHP：命名参数
来源：http://www.share.hesvh.cn/Article/details/gacnhwqkp.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gzabiamjh.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gxaitaadq.sHtML

"值: {$a}"
来源：http://www.share.fehbvm.com/Article/details/grtgiaekx.sHtML

[U58] PHP：数组三件套
来源：http://www.share.hesvh.cn/Article/details/ghhgsdqwv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fehbvm.com/Article/details/gnwwsibxd.sHtML

[U59] PHP：自定义排序
来源：http://www.share.hesvh.cn/Article/details/giyrrckao.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gdingrgrl.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fehbvm.com/Article/details/gapcetgar.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fehbvm.com/Article/details/gqctgnevo.sHtML

[U61] PHP：正则
来源：http://www.m.share.zdbjq.cn/Article/details/gkoiiseif.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gffaqokps.sHtML

[U62] PHP：日期对象
来源：http://www.blog.hesvh.cn/Article/details/gpflxgasd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.hesvh.cn/Article/details/gtiazqzhb.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fehbvm.com/Article/details/gybpvoyil.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.zdbjq.cn/Article/details/gclzijiax.sHtML

[U64] PHP：目录遍历
来源：http://www.share.zdbjq.cn/Article/details/gqegmhprz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fehbvm.com/Article/details/gcklpqgtb.sHtML

[U65] PHP：会话
来源：http://read.share.fehbvm.com/Article/details/gexgjiafj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gejxmqtln.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/gemtmihyz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.zdbjq.cn/Article/details/gjifjecgg.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.zdbjq.cn/Article/details/gahmcmcmk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fehbvm.com/Article/details/ggsdsyaqs.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fehbvm.com/Article/details/gwsnkwaaw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.hesvh.cn/Article/details/gsxiwsceu.sHtML


<!-- 参考信息 -->