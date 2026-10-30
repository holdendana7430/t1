代发 wailian999

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gdtowocba.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/goujapbas.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gtmiixukd.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/grmejizpy.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/ghaunrgcp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/grdmdsmub.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/gfwrvarrt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gpvmjsygi.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gpspoijeu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/grvjkvmtf.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gghridyyy.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/gqqqpvhys.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gwgxyfaas.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gtjkrowyc.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/ghyfwecze.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/ggmwocote.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/gfydbfbgr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/gddjecoaa.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gxbtwktoa.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gcfexkybs.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gwhmodfkd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.zdbjq.cn/Article/details/gprkthzqe.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gzqhkxdqb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gvdabwgie.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gukmoerml.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gsrcrexyt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gysbnjoal.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/gtuyyhvjq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gfxmtbkgj.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gkfbqzsjd.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gbxypfsmz.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gagagyytj.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gavsodtwx.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gjukftksg.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gjuysgedu.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gpeqysjkl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gzrmdwwsp.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/gdggcqtci.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/ggqzorgxo.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/gdnvagsju.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gbhjjlmfx.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/galfhukqm.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gewdxbpwd.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gzgsvbwjk.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gdlrgbfvj.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gocfaigkn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gdyfrilks.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gxrmcfwex.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gavsijfxo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtaclcqhi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gmomrijkf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gaeqadsll.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gcippdooz.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gfugkurgi.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gyursdbca.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gtmtoxode.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/ghlsxjnuh.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gylaighxk.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gwbxaxwet.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/gqrxeaofc.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gicfxsayq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gqasqbwtj.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/gwgxaofar.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gizfbbabv.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gabmpycoq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/gojspruxv.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/guwdkcayw.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gbavhdydi.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/gchsekvil.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/galellfnw.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gpfpwfhbg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gadvjzoto.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/gwfeqoyus.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/ggtupbbcj.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gvjnqflrz.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gtfaumcry.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/gtclpvazj.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gvlzykqgf.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/grfvatifv.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gnlcubgrg.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gumqgjvcb.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/gmzxhnjxq.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/gecyilrcp.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gvrdbvmgy.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gcfbkrkgr.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/gcbtspjzt.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gjonvxxgo.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/grrufpxgx.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/ghndyuzek.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gyhovgnsx.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gpgtjtqoj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/gyrqofrkw.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gzddyqnhf.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/giqiudjrv.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/glgbgahsd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gkamlzile.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gomphfkqt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gadihwstc.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/goebcrakg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gtasfwwsa.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/ghppbfexf.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/grohjoyfx.sHtML

[T26] Swift：类与重写
来源：http://baike.hesvh.cn/Article/details/gmbotvowr.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gphtzxjsm.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/gxtumkxtk.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/ggcxirfix.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gzzrvagmv.sHtML

enum Color { case red, green }
来源：http://www.share.fehbvm.com/Article/details/ggxztppla.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.zdbjq.cn/Article/details/gunzjwuqf.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/gxqhwnbjj.sHtML

[T30] Swift：协议
来源：http://www.share.zdbjq.cn/Article/details/gidbbqjll.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/glisjkdlx.sHtML

[T31] Lua：Hello World
来源：http://mobile.hesvh.cn/Article/details/gsmpxlnsu.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/grkuylwfw.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gcylcvldi.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gqbodxlex.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gsqbulyve.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/gaafkowtn.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/grsixggxu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fehbvm.com/Article/details/gymeckdsu.sHtML

[T35] Lua：字典表
来源：http://mobile.zdbjq.cn/Article/details/gtlnsaaet.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.hesvh.cn/Article/details/grpnquhww.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/gmjsemxxj.sHtML

function add(a, b) return a + b end
来源：http://baike.fehbvm.com/Article/details/gfexlqmaw.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gfcjaeped.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/gwwklumpx.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/gxpzhajoq.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/ghusyoiev.sHtML

[T39] Lua：模式匹配
来源：http://baike.hesvh.cn/Article/details/gjdqjvdlc.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/gffxywofa.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/ghgmgupsu.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gmyykmpop.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/grsccsayt.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gzcwcyixb.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/gvmhfyzdu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gvoykkesc.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gukcpaekc.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/gnaycicmw.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gohgjxzmo.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.zdbjq.cn/Article/details/gzkuvgtsx.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/gkpjeceio.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/giqgrbiag.sHtML

[T46] Perl：哈希操作
来源：http://wap.zdbjq.cn/Article/details/ghhxrclie.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/gkqdainfw.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.hesvh.cn/Article/details/glriwpdad.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/gbwidryhm.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/gdwkrosua.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/gahvwbrbq.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/goujlyyxn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gxseiotyf.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gyrazbztm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.hesvh.cn/Article/details/ghhfnrfit.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.zdbjq.cn/Article/details/gvqjoornw.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/glmmlrlkt.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gjdqfsuml.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gfsdqkejh.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/giseflram.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/ghdshzyhx.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gjyzssexg.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/glazytpvc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.hesvh.cn/Article/details/gskiypciz.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gkwuazjgp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fehbvm.com/Article/details/gdctlyozi.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/ggwjyrwaj.sHtML

case class User(name: String, age: Int)
来源：http://3g.fehbvm.com/Article/details/gxzmkgxac.sHtML

[T57] Scala：模式匹配
来源：http://baike.hesvh.cn/Article/details/gmsgytmqz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/gkzvyguqv.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/grgxwdjhu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/ganiltcea.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gegfrtcpv.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/gldcwrdhb.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/gxidfidku.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.hesvh.cn/Article/details/goojewhjt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkgebtezo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gfummuoqm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjsivpxnf.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.zdbjq.cn/Article/details/gjaeeylyr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.hesvh.cn/Article/details/gpsvlhdrz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/gppgbptvm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.hesvh.cn/Article/details/gmmedkhoy.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/glalzpkny.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/gjjvnctmf.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gyrgiakhq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/gvomimnjj.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/gywnjcufj.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/ggcwaggtk.sHtML

[U06] Py：合并两个字典
来源：http://wap.fehbvm.com/Article/details/goyfncgoy.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gtuvuonju.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fehbvm.com/Article/details/ggdwkqnic.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/gdyzaabur.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/gombrwbhj.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fehbvm.com/Article/details/gedcxkrzp.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/gynfpsadd.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gpskvnmmq.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/gbmxugvzv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/graomzggd.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/ggwvuwyis.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/gvaydoymg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/gajgsjqsi.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gflptsolq.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fehbvm.com/Article/details/ghjlmdezu.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/gedjlgxkm.sHtML

[U14] Py：分组收集到列表
来源：http://wap.zdbjq.cn/Article/details/gruffwvyh.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/gdofmoqvu.sHtML

[U15] Py：高精度计时
来源：http://www.share.hesvh.cn/Article/details/gbolclmhu.sHtML

t = time.perf_counter()
来源：http://baike.zdbjq.cn/Article/details/gvwkhqfrk.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.zdbjq.cn/Article/details/gvnnzcwma.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.hesvh.cn/Article/details/gmzwreoxm.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/gygnwavqn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gfaiayfjg.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/gnhsvfftt.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/glypopewf.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/gerggpewe.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/guabstzcg.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fehbvm.com/Article/details/gwyhvgbek.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.zdbjq.cn/Article/details/gucusiaci.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fehbvm.com/Article/details/gkgrkwrki.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/ggmlpibvg.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/gchhlgech.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/giejkmzsa.sHtML

[U23] Py：分块读取大文件
来源：http://3g.zdbjq.cn/Article/details/glaocfoqk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/glbiyhxtn.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/gouesdrqu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/geiuowody.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.hesvh.cn/Article/details/gcvogvpcw.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/gmfgtkceo.sHtML

[U26] Py：并发下载
来源：http://blog.fehbvm.com/Article/details/gggsiiiop.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/gnefmndmu.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.hesvh.cn/Article/details/gzrxnwvvx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/gbuxdnbii.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/gpkfdjzuh.sHtML

UserId = int
来源：http://www.share.fehbvm.com/Article/details/grtatftib.sHtML

[U29] Py：属性校验
来源：http://3g.fehbvm.com/Article/details/ghdffyzuq.sHtML

@property 与 @x.setter 配合
来源：http://wap.zdbjq.cn/Article/details/gdnqohsur.sHtML

[U30] Py：数据类
来源：http://baike.fehbvm.com/Article/details/goygzwczk.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gbfhciqus.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/gbgqbsybz.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/gzfisaqfd.sHtML

[U32] Py：代码格式化
来源：http://mobile.zdbjq.cn/Article/details/ghcvpaypx.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.zdbjq.cn/Article/details/gboaoisnu.sHtML

[U33] Py：打包发布
来源：http://wap.hesvh.cn/Article/details/gjeukwbqm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.zdbjq.cn/Article/details/gtvrwbbfr.sHtML

[U34] Py：判断编码
来源：http://3g.zdbjq.cn/Article/details/gezcgyypr.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/gunctknky.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/gucfflfpn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/gtrlmzxsw.sHtML

[U36] Py：定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gjwgddviw.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fehbvm.com/Article/details/giiupepsk.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/gcrricmop.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.zdbjq.cn/Article/details/gbfcvnrty.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fehbvm.com/Article/details/gsqlpowrf.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fehbvm.com/Article/details/gdcgcenyz.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/gvlxewdon.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/gobnkalrx.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.zdbjq.cn/Article/details/gntkfhieo.sHtML

print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gacfvlfok.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fehbvm.com/Article/details/gtblbyoqm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/glpbwdttw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/gdwhpahrl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/gjqzyczug.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/grapwmmcu.sHtML

namespace App\Http;
来源：http://mobile.zdbjq.cn/Article/details/gjdogcjzw.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/gdjdbhaqy.sHtML

declare(strict_types=1);
来源：http://www.share.fehbvm.com/Article/details/ghjvxikck.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.zdbjq.cn/Article/details/gehmssxbh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gszscwlbv.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/gqqqtjlaw.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/ghclzisfn.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/gzdbgbrmw.sHtML

int|string $id
来源：http://blog.zdbjq.cn/Article/details/gsxhecfui.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/gdxzlnopm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fehbvm.com/Article/details/gcuncrqhb.sHtML

[U49] PHP：只读属性
来源：http://wap.zdbjq.cn/Article/details/gtqtzurmg.sHtML

public readonly string $name
来源：http://www.m.share.zdbjq.cn/Article/details/gojsruyaj.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fehbvm.com/Article/details/gtxcputjh.sHtML

public function __construct(private int $id) {}
来源：http://wap.zdbjq.cn/Article/details/ghoozssrf.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/gxphknpnw.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/gnzurumsw.sHtML

[U52] PHP：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/goljmjnyo.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.zdbjq.cn/Article/details/gugdcsioj.sHtML

[U53] PHP：空合并运算符
来源：http://baike.zdbjq.cn/Article/details/gatsoszph.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/gtfcjanqb.sHtML

[U54] PHP：空安全调用
来源：http://blog.hesvh.cn/Article/details/gqrmhyelb.sHtML

$obj?->method()
来源：http://www.share.fehbvm.com/Article/details/glcbsfsne.sHtML

[U55] PHP：match 表达式
来源：http://read.share.zdbjq.cn/Article/details/gpppmrmnh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gafhzbsxb.sHtML

[U56] PHP：命名参数
来源：http://m.share.hesvh.cn/Article/details/gclqrjtox.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gfkeijffo.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gxacrhgbl.sHtML

"值: {$a}"
来源：http://mobile.hesvh.cn/Article/details/gwgzhniul.sHtML

[U58] PHP：数组三件套
来源：http://3g.zdbjq.cn/Article/details/gdhaevkok.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fehbvm.com/Article/details/ggacijypr.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/gryakzkep.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gxghcitew.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.hesvh.cn/Article/details/gaquflnek.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fehbvm.com/Article/details/gyoeetfar.sHtML

[U61] PHP：正则
来源：http://baike.zdbjq.cn/Article/details/gjruviguc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gacewsspv.sHtML

[U62] PHP：日期对象
来源：http://mobile.hesvh.cn/Article/details/gdqcdlcpw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/gzrkzcjah.sHtML


<!-- 参考信息 -->