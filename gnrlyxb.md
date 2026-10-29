代发 wailian999

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gjgzmnimi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/gkppkugyc.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gvbocmjvm.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gdlvuwxrf.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gvmqsyvbs.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/goudmxnis.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gqqnanzul.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gnymdwovq.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gtrzkfnmi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gvrastozb.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gepegwfaj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gxzhjzpah.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gafhrowtt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/gnvypbylc.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gwefzxivy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gjewnkefu.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gzyjsxalt.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/gcvzaukpm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gdcoqdmii.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gudnxfnsl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/ggeksxvme.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gllqasxxb.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gpwuxkrwt.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gugsposcd.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gmdmglukq.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/gervbmdud.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/gwwexyxyd.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gujovxhss.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gcrmzkmyb.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/gyanmvhbj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/gqapitjua.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gexssjvdb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/gsdjnxfxm.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/ggiqrbias.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/getpjakhz.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gdhuqpoaa.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/gyntwgkye.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/glcvtwxwa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/ghhzkzgbo.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/glmbwuxms.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/gdxpgcpap.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvmnyksgj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gsghtoopm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghmbmytvr.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gvujljsdc.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gcdqnjdlt.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gcugtqcfw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gyrsbffyh.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/giknsuwmy.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gwbpqigng.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gqpemjxcc.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gxemybypt.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gmjgozpwf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gmhgbxcjs.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gwzdjqrxb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gzusebehv.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gwgnkgoys.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/gmztjeyrd.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gluyavvhi.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/ghrhpjobm.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gwhhgveao.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/gufwrujuq.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/gtlboinbw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gsrarpbnn.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gzfykzeba.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gnffqregm.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gnvitqvex.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/ggsicyrxm.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gxubomqcg.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/ggdtelwcp.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gloubrrmt.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gvuipayzo.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/gphexorbl.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gbojaxled.sHtML

[T16] Swift：Hello World
来源：http://wap.fehbvm.com/Article/details/ggsgirdes.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gzfddbqbi.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gtffkfawx.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gxzqefrpg.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/gaqsfieqk.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gwkdnzmhe.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gvzhgbhjv.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gpjhuyitg.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/gqjokyfsa.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/gnzihjhuu.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/gsnxazvjy.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gdfxeznfr.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/gzrxdhtow.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fehbvm.com/Article/details/gmxizptqu.sHtML

[T23] Swift：函数
来源：http://3g.hesvh.cn/Article/details/gnzzejvwh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gscqygqpq.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/gretjyxtu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gmvbvjjzb.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/gqrtxouih.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gwjwsowfv.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/gdzzzirqg.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gppnasplg.sHtML

[T27] Swift：错误处理
来源：http://read.share.hesvh.cn/Article/details/grorllaob.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fehbvm.com/Article/details/gewiuivxs.sHtML

[T28] Swift：枚举
来源：http://blog.fehbvm.com/Article/details/gsarzvxna.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/gzfppyyep.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/gprogyauo.sHtML

guard let x = opt else { return }
来源：http://www.share.zdbjq.cn/Article/details/gawwtbdsv.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/gnqijgdqp.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.hesvh.cn/Article/details/gautxcaru.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/gfmployxf.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gwynmaugg.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/gkybzztro.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/gmyiiyttw.sHtML

[T33] Lua：表（数组）
来源：http://blog.fehbvm.com/Article/details/gnftlflli.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/gugahvvvw.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/glrtdgpcu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gjsaihpat.sHtML

[T35] Lua：字典表
来源：http://m.share.fehbvm.com/Article/details/gfacdpgod.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fehbvm.com/Article/details/gqlmfyygd.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/gyxbuuzjo.sHtML

function add(a, b) return a + b end
来源：http://read.share.fehbvm.com/Article/details/gjymjqlep.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fehbvm.com/Article/details/gdobegobh.sHtML

"a" .. "b"
来源：http://www.m.share.hesvh.cn/Article/details/gjtznjurt.sHtML

[T38] Lua：条件
来源：http://wap.hesvh.cn/Article/details/gpjsfxlzz.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/gjzffjxot.sHtML

[T39] Lua：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gxnrxmqge.sHtML

string.find(s, "%d+")
来源：http://3g.fehbvm.com/Article/details/gqkzomyno.sHtML

[T40] Lua：元表
来源：http://wap.hesvh.cn/Article/details/ghpdmuhaj.sHtML

setmetatable({}, { __index = base })
来源：http://baike.zdbjq.cn/Article/details/gsasotowc.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/glgynoirs.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gqdbsvvpq.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gbwitsxat.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.hesvh.cn/Article/details/gsromyelb.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gekljcubo.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/grndqxifs.sHtML

[T44] Perl：条件
来源：http://m.share.fehbvm.com/Article/details/gfdfvpikz.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/ghltoxazy.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gqefociyr.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/gmtiioipv.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/gieiorvld.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fehbvm.com/Article/details/gtqwetsqw.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/gcuyqqwae.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/gpfayrzgy.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/ghxmcusmv.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/gqthrpmbu.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/gccplashg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gucglwlhx.sHtML

[T50] Perl：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gbmzzgyxe.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.hesvh.cn/Article/details/gkznbvicu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fehbvm.com/Article/details/gstseqjyd.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/gfqptmppe.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gxhvmspqo.sHtML

[T52] Scala：变量
来源：http://www.share.zdbjq.cn/Article/details/gqbvtvljk.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/gbiupvceb.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/ghzmzahex.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/gwexgwtjb.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/gtamifmry.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gxvfrtvqp.sHtML

[T55] Scala：集合过滤
来源：http://baike.fehbvm.com/Article/details/gfukjpjzk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/gwracznwm.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/gbjvhtrdw.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fehbvm.com/Article/details/givxusgba.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gyubucjur.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gicrgwwbq.sHtML

[T58] Scala：函数定义
来源：http://3g.hesvh.cn/Article/details/gcmkmexve.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gdseccjlo.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/grfvkgryw.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/geedhrlxh.sHtML

[T60] Scala：折叠
来源：http://3g.hesvh.cn/Article/details/goabplvse.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.zdbjq.cn/Article/details/gwnfegdnt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grvhjhkri.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/glaajohhn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggfednzgn.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/grgfstjtn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/gxwowcuyx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.zdbjq.cn/Article/details/gwfvxbirs.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.hesvh.cn/Article/details/gcpbgccje.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/gtevotgye.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/gqdunccdy.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/gncqobdcu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/girijalwd.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fehbvm.com/Article/details/gvufxnixy.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/glvgndzff.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.hesvh.cn/Article/details/gtrlureec.sHtML

{**a, **b}
来源：http://wap.zdbjq.cn/Article/details/gnpmjdagt.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/gzyeghyxp.sHtML

{v: k for k, v in d.items()}
来源：http://wap.hesvh.cn/Article/details/gilqgnikg.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fehbvm.com/Article/details/gtvrnyfdr.sHtML

[y for x in nested for y in x]
来源：http://www.share.zdbjq.cn/Article/details/gowrhgryc.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.zdbjq.cn/Article/details/ghloelzjq.sHtML

max(d, key=d.get)
来源：http://www.blog.fehbvm.com/Article/details/gezhyctzk.sHtML

[U10] Py：按值排序字典
来源：http://www.share.hesvh.cn/Article/details/gfzzimvrh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.hesvh.cn/Article/details/gwsvvouwq.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/gfkhfpcpi.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/gzpchweaz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.hesvh.cn/Article/details/gvwrkpxqx.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fehbvm.com/Article/details/grwapprvg.sHtML

[U13] Py：固定长度队列
来源：http://baike.zdbjq.cn/Article/details/gkwfsxdsl.sHtML

deque(maxlen=10)
来源：http://m.share.zdbjq.cn/Article/details/gmvfijjqs.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.hesvh.cn/Article/details/gnblvompm.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/gtmvutybj.sHtML

[U15] Py：高精度计时
来源：http://m.share.hesvh.cn/Article/details/gmuqbsemp.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/ghkknxgmp.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/gcahxjelu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/guvoesyer.sHtML

[U17] Py：初始化日志
来源：http://www.share.fehbvm.com/Article/details/grvlsamfr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.zdbjq.cn/Article/details/gbsrkfbpc.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/gmubrcsah.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gajqnncca.sHtML

[U19] Py：正则替换带回调
来源：http://3g.zdbjq.cn/Article/details/gungfllgv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/ggjgjxpta.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fehbvm.com/Article/details/gxjtytqcc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.zdbjq.cn/Article/details/gegwprozc.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/gixolqkcl.sHtML

@contextlib.contextmanager
来源：http://3g.zdbjq.cn/Article/details/gbhkojopg.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fehbvm.com/Article/details/gamnppvzj.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/gawbpgyax.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fehbvm.com/Article/details/gzracqxst.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.zdbjq.cn/Article/details/gxyqxjzkg.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/gkflpukmw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gczocobja.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gqfgletlv.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/gjesuzbgd.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/gsddrpwfe.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/gqhjysrbf.sHtML

[U27] Py：异步 HTTP
来源：http://blog.zdbjq.cn/Article/details/gqjhmksum.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fehbvm.com/Article/details/gqgmnjdsf.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fehbvm.com/Article/details/gvtxcydsh.sHtML

UserId = int
来源：http://www.share.zdbjq.cn/Article/details/gvbqhalfd.sHtML

[U29] Py：属性校验
来源：http://3g.hesvh.cn/Article/details/glemembln.sHtML

@property 与 @x.setter 配合
来源：http://read.share.zdbjq.cn/Article/details/gqtiuoyhd.sHtML

[U30] Py：数据类
来源：http://wap.zdbjq.cn/Article/details/gmkphspbb.sHtML

@dataclass(slots=True)
来源：http://m.share.zdbjq.cn/Article/details/gmvkmxoxv.sHtML

[U31] Py：单测
来源：http://www.share.hesvh.cn/Article/details/gkfpxvohh.sHtML

python -m pytest -q
来源：http://baike.hesvh.cn/Article/details/gkdpbwfpf.sHtML

[U32] Py：代码格式化
来源：http://wap.zdbjq.cn/Article/details/ghclxqovh.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.zdbjq.cn/Article/details/gbgffahhd.sHtML

[U33] Py：打包发布
来源：http://m.share.fehbvm.com/Article/details/gnpdpbhdu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/ghecpztfd.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/glviqojdg.sHtML

chardet.detect(raw)
来源：http://m.share.fehbvm.com/Article/details/gmvhqamnd.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/gnabxpozj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/gbkzpuhmu.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/gljfzovje.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.zdbjq.cn/Article/details/gstgvxyoo.sHtML

[U37] Py：读写 Excel
来源：http://baike.fehbvm.com/Article/details/glqpoomnp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.zdbjq.cn/Article/details/gykigcpxf.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/gdilvzikp.sHtML

Path(__file__).resolve().parent
来源：http://baike.hesvh.cn/Article/details/gvjcwaxwb.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.hesvh.cn/Article/details/gpwwssxlh.sHtML

sys.stdout.isatty()
来源：http://blog.fehbvm.com/Article/details/gufpqvhsp.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/glrizwqpc.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gefpdrivg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.zdbjq.cn/Article/details/gyiltgqfx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.zdbjq.cn/Article/details/gkwqqzwtj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.zdbjq.cn/Article/details/gswwoayif.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/ggurbdjlq.sHtML

[U43] PHP：声明命名空间
来源：http://3g.hesvh.cn/Article/details/gmkaebilh.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/gqwtgvqcw.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fehbvm.com/Article/details/ggwhgaatt.sHtML

declare(strict_types=1);
来源：http://read.share.fehbvm.com/Article/details/gsfzndluh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fehbvm.com/Article/details/gvzdjyrmm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/giehzwgur.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.hesvh.cn/Article/details/gacurjnwn.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/gtnyeyfft.sHtML

[U47] PHP：联合类型
来源：http://mobile.fehbvm.com/Article/details/gguidrgzt.sHtML

int|string $id
来源：http://wap.hesvh.cn/Article/details/gainyystu.sHtML

[U48] PHP：纯枚举
来源：http://blog.fehbvm.com/Article/details/gvhthaugt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.hesvh.cn/Article/details/gwdvecwmi.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fehbvm.com/Article/details/gjvlgwuzp.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/gpjkrsymz.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.zdbjq.cn/Article/details/gpsgqthen.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/gjkcrpwkm.sHtML

[U51] PHP：数组解构
来源：http://read.share.zdbjq.cn/Article/details/glxnrawjq.sHtML

[$a, $b] = $arr;
来源：http://3g.fehbvm.com/Article/details/gtoeopjzv.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gsprqlezo.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gkpixqgux.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/gwojaqiey.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gxoqwpmam.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fehbvm.com/Article/details/gurfogjaj.sHtML

$obj?->method()
来源：http://blog.hesvh.cn/Article/details/gbtetmhsd.sHtML

[U55] PHP：match 表达式
来源：http://baike.zdbjq.cn/Article/details/grrvqevph.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.zdbjq.cn/Article/details/gkgwwxqai.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/graweieqe.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/grwmmmcqn.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gyyoroedj.sHtML

"值: {$a}"
来源：http://baike.hesvh.cn/Article/details/ghvimkepd.sHtML

[U58] PHP：数组三件套
来源：http://mobile.zdbjq.cn/Article/details/gcdaxnrrw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.hesvh.cn/Article/details/gislbclhg.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/gwboaxuxt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gyrwadgqp.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.zdbjq.cn/Article/details/grhrkqxiu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.hesvh.cn/Article/details/gvxgbnfhk.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/gkrnzxikq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gngzcnmtv.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.hesvh.cn/Article/details/ghdhprvyy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/gldnpszxf.sHtML

[U63] PHP：文件读写
来源：http://mobile.fehbvm.com/Article/details/gypdizddn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fehbvm.com/Article/details/gnltsjrsh.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/gukcnfoxi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.hesvh.cn/Article/details/ghcndaogy.sHtML

[U65] PHP：会话
来源：http://www.m.share.fehbvm.com/Article/details/gdgyxfspp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gcrqlhsam.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/gnxbrohay.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.hesvh.cn/Article/details/gustkulls.sHtML


<!-- 参考信息 -->