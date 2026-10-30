代发 wailian999

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/gqzkrjate.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gykgnfwpu.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gfzzbkjrz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkyooupxo.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/glxruoirn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gdkmygkel.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gbdtjnzqn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gcmnwnnhk.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/gcbawqedo.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gcksahbxm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gxcujnalp.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gqcrqkosx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/giajaduyg.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gwzujalgu.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gxsmfxhfo.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gxonamyvv.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/gsumsance.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/gyzhaqpqk.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/gnuxidalr.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/gbedxxwjp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/gqbcxyqnu.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gsfrfseaw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gxleamtwr.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/grogdpiya.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gikaoaqca.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gflcsusvu.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/grggkuzpg.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gyncfbyaj.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/ghngqjklk.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/gbemjqzla.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gjsklypkn.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/gfruznjtk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gqqcaymzt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqteegdkg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gwrdkedcl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/giqybqtae.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gzuidhcbp.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gkdzfvils.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gauboeowd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gujzsrqpq.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/glzitkaup.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gibhudbev.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/gefsuqntg.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gwblvzhea.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/ggfrnupah.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gfcrgfbui.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gqkzxapub.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gmsbxkvim.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/giwakunci.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gfzotounc.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/galpjzwte.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gkwocoykk.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/glwdkwxib.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gzbgqninv.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gracentvp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gomrgdsyv.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/genjwncgj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gioecbvjp.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/gwyquzjzr.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gkzleuotr.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/gjaremgqr.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gkhcyhiln.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/grjjcibqk.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gquibdzse.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/ghnfpnnsc.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gibqnnlzh.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/gtmyezkwg.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gnnkbhxxn.sHtML

[T17] Swift：变量与常量
来源：http://read.share.zdbjq.cn/Article/details/gebvgvgiw.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/gsnicwwiv.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gqacqzckn.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gfatxqglg.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gnhpzknkw.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/gxeurxwqd.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/gutfgzczs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gnatpemja.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/gbcnkpmye.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/guqcwhmlh.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/gdkotsdiv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gkzvjwuli.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/ghxhfztzi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/gnzhdelvy.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/gklwksjbd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gbcrzsure.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/gczevamzm.sHtML

struct P { var x: Int }
来源：http://www.m.share.fehbvm.com/Article/details/ggozmzfxi.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gmltlkeoi.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gxfxgdpsi.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/gtinfihyp.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gocfzpate.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gxewncahh.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gtqfickjf.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/gxmqsuxwt.sHtML

guard let x = opt else { return }
来源：http://3g.fehbvm.com/Article/details/gggtomnbd.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/gsdphzoyi.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.zdbjq.cn/Article/details/gpklbijef.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/geqgthcwd.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/geexoatcw.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gvueshiiy.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gyrlqsfvi.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/gchmjorya.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/guamiutgv.sHtML

[T34] Lua：遍历表
来源：http://3g.hesvh.cn/Article/details/gffmnylsz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/gdyfurzvu.sHtML

[T35] Lua：字典表
来源：http://blog.fehbvm.com/Article/details/gyinzqdvc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/gojsocfrz.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/grfcgqfry.sHtML

function add(a, b) return a + b end
来源：http://baike.fehbvm.com/Article/details/gqqqkajtl.sHtML

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/gagygpppz.sHtML

"a" .. "b"
来源：http://3g.hesvh.cn/Article/details/gkdpurusv.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/gcdgfacoa.sHtML

if x > 0 then print("正") end
来源：http://read.share.hesvh.cn/Article/details/gldnofwli.sHtML

[T39] Lua：模式匹配
来源：http://baike.hesvh.cn/Article/details/gwjtwxdvr.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/gnitqvtgk.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/gzbgkyjaq.sHtML

setmetatable({}, { __index = base })
来源：http://wap.zdbjq.cn/Article/details/gzrtummbs.sHtML

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/guqvchykw.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/gxeocvhkl.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/gfreinhxa.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/gjtvqpduf.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gvzjukecv.sHtML

"值: $a"
来源：http://www.m.share.fehbvm.com/Article/details/gawvwsddq.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/ggtymdpgq.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/gkmjorpgr.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/gjvxmiaqz.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gwwbepcxk.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gmzbqyafi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gofzpkcon.sHtML

[T47] Perl：正则捕获
来源：http://baike.hesvh.cn/Article/details/gcriodfuw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fehbvm.com/Article/details/gopvvnymv.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/ghnbxvvbi.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gsdhiyrhv.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/giaazpjsv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gflcnymui.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/ghkfsmfmz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fehbvm.com/Article/details/gvlkqpafa.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.zdbjq.cn/Article/details/gkxpoizas.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gowvrxqtw.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gzrpvpemi.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gdxwmtbkp.sHtML

val a = 1;  var b = 2
来源：http://read.share.hesvh.cn/Article/details/gvyjpoizq.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gspjvzrre.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gllrvgbbi.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gbrsbimtf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/gcaqxrtba.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gvblausqq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqbumsxfh.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/gxocglnoi.sHtML

case class User(name: String, age: Int)
来源：http://www.share.hesvh.cn/Article/details/gxszsgmqq.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gikhzpknz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/gsmmsourl.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/gobhkqqdq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/gqvulowdl.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/gzvpnmdui.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/gujmvzhng.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/gdrkkcbcs.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.hesvh.cn/Article/details/glcxvaahk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gppyjvkax.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gtrgbmldx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ganqgbrpq.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/gpreduuco.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/gzptarolf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/geuizinqb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.zdbjq.cn/Article/details/gglsztlhq.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/glnqbcqey.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/gpiujjzug.sHtML

[U04] Py：变量调试打印
来源：http://mobile.hesvh.cn/Article/details/gadmpicjs.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gedondukb.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fehbvm.com/Article/details/gmjtyiolo.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/goaqweuiq.sHtML

[U06] Py：合并两个字典
来源：http://read.share.zdbjq.cn/Article/details/gtekzyoer.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gfruswpej.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fehbvm.com/Article/details/gsccqgjah.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/gpcfzeuic.sHtML

[U08] Py：展平二维列表
来源：http://www.share.hesvh.cn/Article/details/gzgawvbwv.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/gehwaxisf.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/gpdfydsol.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/gnsktoadu.sHtML

[U10] Py：按值排序字典
来源：http://baike.hesvh.cn/Article/details/gfvxtgyfg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/gxydcbvxf.sHtML

[U11] Py：生成器表达式
来源：http://blog.fehbvm.com/Article/details/gahztgoay.sHtML

(x * 2 for x in arr)
来源：http://www.blog.zdbjq.cn/Article/details/gawyberoa.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/giucpqydh.sHtML

Counter(arr).most_common(3)
来源：http://blog.zdbjq.cn/Article/details/gostufzyt.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fehbvm.com/Article/details/gwwtemdap.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gkgssctxv.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/goempdkag.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/gyhwhbzwv.sHtML

[U15] Py：高精度计时
来源：http://m.share.hesvh.cn/Article/details/grmqdlqjl.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/gbmquafae.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.zdbjq.cn/Article/details/gpgmthgha.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/gkvwodmpk.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/gijingwzb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/gracxkssj.sHtML

[U18] Py：预编译正则
来源：http://mobile.zdbjq.cn/Article/details/gvkgjdydf.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/grntjkcco.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/gymfhxfgv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.zdbjq.cn/Article/details/gfcmyqomn.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/guketrezp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/gevsikjnc.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fehbvm.com/Article/details/gexlilajt.sHtML

@contextlib.contextmanager
来源：http://3g.fehbvm.com/Article/details/gjoppvvvt.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/gtfjasnpv.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/ghzugjria.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fehbvm.com/Article/details/gbjasxhlx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/gutylkbhr.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/gxrvlbwjq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gseycusie.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.hesvh.cn/Article/details/grikifyac.sHtML

csv.DictReader(f)
来源：http://read.share.zdbjq.cn/Article/details/gtubirmnq.sHtML

[U26] Py：并发下载
来源：http://baike.zdbjq.cn/Article/details/gxjcxigkr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/gkjavkeej.sHtML

[U27] Py：异步 HTTP
来源：http://baike.hesvh.cn/Article/details/gmunseqsw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.zdbjq.cn/Article/details/gmlbgtvly.sHtML

[U28] Py：类型别名
来源：http://www.blog.fehbvm.com/Article/details/ggdhymdua.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/grqtwilha.sHtML

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/ggqzmqjvw.sHtML

@property 与 @x.setter 配合
来源：http://read.share.zdbjq.cn/Article/details/gqnimsotn.sHtML

[U30] Py：数据类
来源：http://m.share.zdbjq.cn/Article/details/gxsgoszyt.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/glhelntmq.sHtML

[U31] Py：单测
来源：http://blog.fehbvm.com/Article/details/guasiiiaq.sHtML

python -m pytest -q
来源：http://wap.fehbvm.com/Article/details/gepbolmhd.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gcmteypni.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gilpwclfb.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/gjjqsqhis.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.zdbjq.cn/Article/details/giqdweick.sHtML

[U34] Py：判断编码
来源：http://www.m.share.zdbjq.cn/Article/details/gymmgnchc.sHtML

chardet.detect(raw)
来源：http://blog.hesvh.cn/Article/details/gkoefrdva.sHtML

[U35] Py：发送邮件
来源：http://blog.fehbvm.com/Article/details/gpqwslqmo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fehbvm.com/Article/details/gtxwanriy.sHtML

[U36] Py：定时任务
来源：http://baike.fehbvm.com/Article/details/gdsxhwofh.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fehbvm.com/Article/details/gsomatdfb.sHtML

[U37] Py：读写 Excel
来源：http://blog.zdbjq.cn/Article/details/gvuyujvix.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.zdbjq.cn/Article/details/gqxhctvxr.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.zdbjq.cn/Article/details/gcpccrvyn.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fehbvm.com/Article/details/gdpipcoob.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fehbvm.com/Article/details/ghlpymnto.sHtML

sys.stdout.isatty()
来源：http://3g.fehbvm.com/Article/details/glsgqqmed.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gusfyegbr.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gkljyhkso.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.zdbjq.cn/Article/details/gqasojxpe.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/ggvuupdyw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/ggcbgezyu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/gnsmxwlzk.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/gpmvzvsbx.sHtML

namespace App\Http;
来源：http://wap.hesvh.cn/Article/details/ggjfgfrhm.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.zdbjq.cn/Article/details/gkgwonifi.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/gmbyigjrn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fehbvm.com/Article/details/gbxacdpcl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gwjomseta.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/gtezdqeny.sHtML

?string $name = null
来源：http://wap.fehbvm.com/Article/details/gwlgnkuln.sHtML

[U47] PHP：联合类型
来源：http://m.share.fehbvm.com/Article/details/gyetgbunt.sHtML

int|string $id
来源：http://www.share.fehbvm.com/Article/details/gmlhvcphz.sHtML

[U48] PHP：纯枚举
来源：http://read.share.hesvh.cn/Article/details/gadaqqdjv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/gnhyrjqlu.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.hesvh.cn/Article/details/gnmpgtbhb.sHtML

public readonly string $name
来源：http://wap.zdbjq.cn/Article/details/gysxvysho.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fehbvm.com/Article/details/grpinswnz.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqwehkbnm.sHtML

[U51] PHP：数组解构
来源：http://blog.fehbvm.com/Article/details/gnyvumert.sHtML

[$a, $b] = $arr;
来源：http://read.share.zdbjq.cn/Article/details/gjcefnigi.sHtML

[U52] PHP：箭头函数
来源：http://baike.fehbvm.com/Article/details/gkwqlbqyk.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gnjmpanaa.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/gulyloxce.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.hesvh.cn/Article/details/gbpdtwblk.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.zdbjq.cn/Article/details/grcudmuru.sHtML

$obj?->method()
来源：http://www.share.zdbjq.cn/Article/details/gsmdmdcjq.sHtML

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/godqbzllj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/guezagohj.sHtML

[U56] PHP：命名参数
来源：http://m.share.zdbjq.cn/Article/details/gzibassmf.sHtML

f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gicjwmujw.sHtML

[U57] PHP：字符串插值
来源：http://wap.hesvh.cn/Article/details/gupizbgvj.sHtML

"值: {$a}"
来源：http://m.share.hesvh.cn/Article/details/gsywlcccm.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/ghhigonzm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.zdbjq.cn/Article/details/gawojdubo.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fehbvm.com/Article/details/gynkvircn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/ggcubopzl.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.zdbjq.cn/Article/details/gqeujyzbs.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fehbvm.com/Article/details/gfyjfsvaa.sHtML

[U61] PHP：正则
来源：http://3g.zdbjq.cn/Article/details/gsidcypxr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gbsuviwzb.sHtML

[U62] PHP：日期对象
来源：http://mobile.fehbvm.com/Article/details/gbixzwcjt.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fehbvm.com/Article/details/gonydxhjh.sHtML

[U63] PHP：文件读写
来源：http://wap.zdbjq.cn/Article/details/gqzxvszxi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fehbvm.com/Article/details/gzjntukqx.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fehbvm.com/Article/details/gixmeqpom.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fehbvm.com/Article/details/ghtkxkqix.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/gapnwhepk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gqenjzfww.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/glgriixhh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.zdbjq.cn/Article/details/grtwclszt.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fehbvm.com/Article/details/gttratqhx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/glcympynv.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/glxangppm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.hesvh.cn/Article/details/gndgctxuj.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.hesvh.cn/Article/details/ghmfcunuv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fehbvm.com/Article/details/geywbdvkj.sHtML

[U70] PHP：PDO 事务
来源：http://baike.hesvh.cn/Article/details/gnvvlpujy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.hesvh.cn/Article/details/gfkakcney.sHtML


<!-- 参考信息 -->