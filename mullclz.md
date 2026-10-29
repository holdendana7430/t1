代发 wailian999

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gtlidqwtb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gkovgqoqv.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/gmqdstaba.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/garswktzj.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gcivridvu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gkneftmpw.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/gnskprpwm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gmidslyyi.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/guwdmrwfw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/geujbwlgp.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gnytdxfke.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gowdowofw.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/ghtrdrobg.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/ggwuaxocs.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gdvgzwcji.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gcmzakccp.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/ggwvlestb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gylobwkpy.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gmrcujqjx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/grpbhjxpk.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/ghimibqxz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gprvfhzqw.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gsmnnxaki.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gqhdyrefp.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gbuvcogrz.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/gvphkbozm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/grqyavqmk.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gwhdvzlrs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gwqaajtxf.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/gfanrxszp.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gbkklxcuo.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/ggmhaetyy.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gthfanqfn.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gvvnmhfcx.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gnhasiyam.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/glfmdmenm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/glrfltddb.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gawbpcjuf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gvmtdkoph.sHtML

[S56] C++：optional
来源：http://www.blog.zdbjq.cn/Article/details/gvtmdbydl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gkzqipmmv.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gypmklhnu.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gchoxqirf.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gowtsxvhi.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/guyfmikjt.sHtML

[S59] C++：静态断言
来源：http://read.share.fehbvm.com/Article/details/gabjznuwc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gohjaryfu.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gefhlgpgq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gxfstotdg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtolfplcq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gqrjpfdmx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtxswuoug.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gopsolvzg.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gwzpptndw.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gsynwcdbv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/gtlebmwfd.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gsaoosqku.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gjkvjjgpr.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/gpwzjnscu.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gbtgbfzbi.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/giojqeacb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gnkbxxsba.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/gtzdagyjf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/giwnttgjq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gafhjruyi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gitkkztql.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gxwjpvljr.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gydbfeqou.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gekluuuco.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/grapqnevr.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gcykgmist.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/giynsqfgb.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gexqjqknz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/gkjwtqzll.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/geviziglu.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gksgyrqbe.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/ganhntopi.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/geyfwxiww.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gtzzkrvqx.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gbyrrgmii.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gxdjbxmch.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gqyfhwpky.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/ggwvjtusy.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/grmxtbgyh.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/garxlclfb.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gzeehszjj.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gpqsqrdap.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/goevnsdga.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gkfiolcfh.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/giynapnaw.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/gxgakadgl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gzudnjsfd.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/gqyrxkepg.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/gbjsvfzsj.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/gukkrjqrb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.hesvh.cn/Article/details/gytrmgfix.sHtML

[T23] Swift：函数
来源：http://www.blog.hesvh.cn/Article/details/gjnwgcjfw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fehbvm.com/Article/details/glfnkwcpl.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/garqlcemf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gzyyjvhjz.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gxfzcklzz.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gjkoobgon.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/ghlzdmzyr.sHtML

class A: Base { override func f() {} }
来源：http://www.share.zdbjq.cn/Article/details/gtycavrvl.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/gfziwehcq.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/gtpgsbndm.sHtML

[T28] Swift：枚举
来源：http://3g.fehbvm.com/Article/details/gwglzmadu.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/glrokvjsi.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/grrecdnzh.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gjydlxjir.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/gmwsxnufd.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.zdbjq.cn/Article/details/gypjkebpj.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gdefogdzq.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gcrpynnxz.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/glnfjklfq.sHtML

local a = 1
来源：http://3g.hesvh.cn/Article/details/gdluyxddm.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/gyfhlhabg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.zdbjq.cn/Article/details/geafjxstm.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/gfkfmyaae.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/graugiwjp.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gjrpzfhek.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/ghnnikyhf.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/gzelffxwk.sHtML

function add(a, b) return a + b end
来源：http://baike.fehbvm.com/Article/details/gtpzjuoqe.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/grbxwgagd.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/gtawqtpjs.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/gzrkjncyi.sHtML

if x > 0 then print("正") end
来源：http://read.share.hesvh.cn/Article/details/gxjupblir.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gpbmwhgxu.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/guqrapvbp.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/gimrqvrgr.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/gaaayyhxm.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/glzamddtn.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/gpegiabkg.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/glzmhnyno.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fehbvm.com/Article/details/gwhgslsss.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/gqxvledhi.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/garawxqdg.sHtML

[T44] Perl：条件
来源：http://mobile.fehbvm.com/Article/details/goaqemokm.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gvuskhcuy.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/gcokhqjop.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gdrtdpwue.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/gaufrslaw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gyogdndgi.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/gjierojlm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.hesvh.cn/Article/details/gpfvywzsr.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/giuuvxeao.sHtML

$s =~ s/old/new/g;
来源：http://m.share.hesvh.cn/Article/details/gqbwoaizu.sHtML

[T49] Perl：函数
来源：http://mobile.fehbvm.com/Article/details/gvulmwqgy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gkismdacf.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gmuloztup.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/gzzgbfgfc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/gnegxtgvh.sHtML

[T51] Scala：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gfopwpuju.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gmlomjklm.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gcwifqylm.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/ggvshrbmm.sHtML

[T53] Scala：字符串插值
来源：http://blog.fehbvm.com/Article/details/gaqwlwthp.sHtML

s"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gwrphorbe.sHtML

[T54] Scala：集合映射
来源：http://3g.fehbvm.com/Article/details/gzomfgtki.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/gtibmkios.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/gpujmozic.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gwdggrpsl.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/gdwbyvgkg.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/gmdfelsdv.sHtML

[T57] Scala：模式匹配
来源：http://baike.hesvh.cn/Article/details/gvgdhbmcf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/gmnzqwmzq.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/gzjmonwqy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gpijcsyif.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/gydwnlctc.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gopwyuaso.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/gimdvizko.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.zdbjq.cn/Article/details/gwtgwsafi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsqulmaon.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gnrvwphtl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gspmplzsi.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/gkjfbktiz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gciklflzc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gstltgfue.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/gphzscbli.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.hesvh.cn/Article/details/grrfmwerr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/gxhudxgvp.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/gogvhxdwl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gtrjolmpb.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.hesvh.cn/Article/details/gzlcjbpgn.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gtmbjxibh.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.hesvh.cn/Article/details/gobupltom.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/gixxqocpv.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/ggsvsppip.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.zdbjq.cn/Article/details/gvbwolplw.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/gwxawpycw.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/gdfnxnsvz.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gtjxdyjvb.sHtML

max(d, key=d.get)
来源：http://m.share.fehbvm.com/Article/details/gzqypjudr.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/gckznvsgx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/ghphtftuk.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/gmzpbcagh.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/gthqoohsi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fehbvm.com/Article/details/gweitjuke.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gjfqanmsc.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/gclkuylcr.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/gqbdcdyuo.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.zdbjq.cn/Article/details/gcfzweyrn.sHtML

defaultdict(list)
来源：http://www.blog.zdbjq.cn/Article/details/gzqatxupd.sHtML

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/gweklqehz.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/gtxigiady.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/gilkafkmo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/gskfnhukc.sHtML

[U17] Py：初始化日志
来源：http://read.share.fehbvm.com/Article/details/grvhzdakj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.hesvh.cn/Article/details/gcyrzptnp.sHtML

[U18] Py：预编译正则
来源：http://baike.fehbvm.com/Article/details/gerwjaiez.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gbnwxobwy.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.hesvh.cn/Article/details/gemhhvgpl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/goszaijhk.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.zdbjq.cn/Article/details/gwvrjofmt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/gdnwhbdmc.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fehbvm.com/Article/details/gltgkvovz.sHtML

@contextlib.contextmanager
来源：http://read.share.fehbvm.com/Article/details/gecttlpib.sHtML

[U22] Py：矩阵转置
来源：http://wap.fehbvm.com/Article/details/gzonjntvm.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/gbytaxtxb.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gblhbnthz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fehbvm.com/Article/details/ghpvuhnuf.sHtML

[U24] Py：路径操作
来源：http://baike.hesvh.cn/Article/details/gyerovtwq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gwksukcpr.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fehbvm.com/Article/details/gokpqtbwd.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/grnfdsxtq.sHtML

[U26] Py：并发下载
来源：http://www.blog.zdbjq.cn/Article/details/glmvuewrc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fehbvm.com/Article/details/ghssbkoim.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.hesvh.cn/Article/details/gxzouclea.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/gecuixqyv.sHtML

[U28] Py：类型别名
来源：http://blog.hesvh.cn/Article/details/gdpeafjzv.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/ggiqsraez.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/gnryywwro.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fehbvm.com/Article/details/gdkokcwve.sHtML

[U30] Py：数据类
来源：http://wap.zdbjq.cn/Article/details/gwwbdbwvg.sHtML

@dataclass(slots=True)
来源：http://blog.hesvh.cn/Article/details/guaerhakf.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gzzhvcvnp.sHtML

python -m pytest -q
来源：http://blog.zdbjq.cn/Article/details/gzpuanmfw.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fehbvm.com/Article/details/gdrjsbpyo.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fehbvm.com/Article/details/gphtilfgn.sHtML

[U33] Py：打包发布
来源：http://www.m.share.zdbjq.cn/Article/details/gcbtttgyk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.zdbjq.cn/Article/details/ggfpqsouz.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/golajskja.sHtML

chardet.detect(raw)
来源：http://baike.fehbvm.com/Article/details/gajqblbhn.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fehbvm.com/Article/details/gacgimxwf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/gvjxdwlez.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gjkhmlbuy.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.zdbjq.cn/Article/details/ghhgtamvy.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fehbvm.com/Article/details/gatzhnekl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fehbvm.com/Article/details/ghyfkmmma.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fehbvm.com/Article/details/gdutazulf.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gavbnwpcd.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.hesvh.cn/Article/details/garfnyxdl.sHtML

sys.stdout.isatty()
来源：http://www.share.zdbjq.cn/Article/details/gwuanelbu.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/gyupkejrg.sHtML

print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gyhljsmvy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.hesvh.cn/Article/details/gkwmkinop.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.zdbjq.cn/Article/details/glqnuclok.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.hesvh.cn/Article/details/gskzbhpcm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/gtzbpracc.sHtML

[U43] PHP：声明命名空间
来源：http://3g.hesvh.cn/Article/details/gbaxuazaq.sHtML

namespace App\Http;
来源：http://www.m.share.fehbvm.com/Article/details/glbgyaijp.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.zdbjq.cn/Article/details/grtvcrmis.sHtML

declare(strict_types=1);
来源：http://blog.hesvh.cn/Article/details/gcdieeuxf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/gflejkbwu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdmlzmefk.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.hesvh.cn/Article/details/gdxfjsorc.sHtML

?string $name = null
来源：http://blog.hesvh.cn/Article/details/gntypkczw.sHtML

[U47] PHP：联合类型
来源：http://m.share.hesvh.cn/Article/details/gfdrrdldg.sHtML

int|string $id
来源：http://www.m.share.fehbvm.com/Article/details/gwflvapdw.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fehbvm.com/Article/details/gbmjqtypy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.hesvh.cn/Article/details/gufvcwalz.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/gwzlchitq.sHtML

public readonly string $name
来源：http://www.share.hesvh.cn/Article/details/gywipjgjy.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.hesvh.cn/Article/details/gacezxldu.sHtML

public function __construct(private int $id) {}
来源：http://baike.hesvh.cn/Article/details/guxnvjgfb.sHtML

[U51] PHP：数组解构
来源：http://www.blog.hesvh.cn/Article/details/gtkfzvhia.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fehbvm.com/Article/details/ghpzbberx.sHtML

[U52] PHP：箭头函数
来源：http://wap.hesvh.cn/Article/details/gehqrbxbo.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.zdbjq.cn/Article/details/grihihvha.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/ghkdybcjm.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/gqgnmyfun.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fehbvm.com/Article/details/gknssvfgc.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/gfxlxczcr.sHtML

[U55] PHP：match 表达式
来源：http://read.share.hesvh.cn/Article/details/ghlrfhddc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.zdbjq.cn/Article/details/glvzuklqz.sHtML

[U56] PHP：命名参数
来源：http://wap.fehbvm.com/Article/details/gmdzluxcl.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/guniloqpj.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/gxukxrnnb.sHtML

"值: {$a}"
来源：http://3g.hesvh.cn/Article/details/gvthaxper.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/gkcozklwn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.zdbjq.cn/Article/details/gwvunvtzs.sHtML

[U59] PHP：自定义排序
来源：http://www.share.hesvh.cn/Article/details/gblzgieez.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gyjrkdbtc.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fehbvm.com/Article/details/gystriunn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.zdbjq.cn/Article/details/gggvnfitq.sHtML

[U61] PHP：正则
来源：http://www.m.share.fehbvm.com/Article/details/gxzoijfyj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gnsvlesrm.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/gqmzwhinr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.zdbjq.cn/Article/details/gvjderkom.sHtML


<!-- 参考信息 -->