代发 wailian999

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gdzhhhgef.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/ggdxloyds.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/gfyyzobeu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/gvghynvgp.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gsokgvfio.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gsiopfojq.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gabxblozd.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gqipwbzyk.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gcrmcjnlu.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/gqulohiti.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/gauxvrtia.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gzrkmybrp.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/gmevfeipw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gozsuujjy.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/ggcjxcmhy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gquqqhonz.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gpsqtmqti.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gepdilgts.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gwiucadgn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/gipwvuygq.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/grgpcdiao.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gcalrwupx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/gtuvrwcwv.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gsvrsutqc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gymkfmnmm.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/gkznshfko.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gruxamjfs.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gmncjfdat.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gpzpqcyki.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gnzqcexbu.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gckbbxkmq.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/gbniaxjsc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gcqesscnr.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gosifpurw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gpmlsmcaz.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/guieqbpmj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcayagwtp.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gcfpfdgde.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gkafkqblb.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/geyjkqscb.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gmcdoeiek.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gsyooncia.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gjjwphycb.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/guwcguznb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gqypzlwss.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbeubmbna.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gdiugaqcf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glyijcxtj.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gcddoswcc.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/glxhqcuzm.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/glpwhgnfz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gsbotjjwg.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gvawymsii.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gxoezstoj.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/gadikgakk.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/gfaqgtfpf.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gcaeposnu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gamcbgyfv.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gtxisggis.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gxxarmphn.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gvjtqrunt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gnznqrbtx.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/ggdgyjoas.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gnusankdg.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/gbjkxtfvx.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/ghtixwvoq.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/ggwgtzfeo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/gboqdadnn.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gymacnxuq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gpvyuekdw.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gsfdoxvst.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/ggfzhubyl.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/gmknhtxek.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gpnurbuwg.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/ghvitirsd.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/giexmsmos.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gteewnbpl.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/guvzoejhc.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/gsuoduint.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gkjdbaoug.sHtML

[T17] Swift：变量与常量
来源：http://3g.zdbjq.cn/Article/details/gcdncadjo.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/ghevjlqpl.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gmigwmnrv.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/gcuognydm.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/grtcyihxf.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gfzbwbjkk.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/grrmkblwq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gdhuswzhk.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/gptmxwors.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/grzxqqbhp.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/gzdofhouk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gpacdfbvk.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/gszhceqjx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/gxvrmtfum.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/gdywwfdqc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gotaeztzm.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/gslodufsv.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gfskrbrpw.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/gvliyuvvl.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/giknlphdh.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/gicnyywlw.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/gnvpezrul.sHtML

[T28] Swift：枚举
来源：http://www.blog.fehbvm.com/Article/details/gxbejbozk.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/gfhfqcpnm.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/gxmyboqod.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/gbomvizqf.sHtML

[T30] Swift：协议
来源：http://mobile.fehbvm.com/Article/details/gfomeukni.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fehbvm.com/Article/details/gxkvobrbe.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gtidiuuwo.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gqupyhiql.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/gbccrxqar.sHtML

local a = 1
来源：http://m.share.fehbvm.com/Article/details/gescopntw.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/gvhrqukjc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.zdbjq.cn/Article/details/gfcsziguh.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/gjifjfijt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/gyxtiaaay.sHtML

[T35] Lua：字典表
来源：http://m.share.hesvh.cn/Article/details/giyuwrrvj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/gnvwujkwv.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/gppvmulok.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/gqjwxvmit.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gqrgpqzhv.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/ggtnqlpbd.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/gexnklkkj.sHtML

if x > 0 then print("正") end
来源：http://www.share.zdbjq.cn/Article/details/guxuhjfvf.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gfkquqsyz.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/gxupvjwdb.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/gykfjfngz.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/ghzpbolyo.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/gafwgkzds.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/gkgvavbio.sHtML

[T42] Perl：变量类型
来源：http://m.share.fehbvm.com/Article/details/gzurtsbnc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/ggiiiaevl.sHtML

[T43] Perl：字符串插值
来源：http://blog.fehbvm.com/Article/details/gqwsqlsdi.sHtML

"值: $a"
来源：http://wap.fehbvm.com/Article/details/gmarycypk.sHtML

[T44] Perl：条件
来源：http://3g.hesvh.cn/Article/details/gjaglvejq.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/gvqlvlxgg.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/gzhafizkp.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/guvokrabu.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/gqanvkeyr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fehbvm.com/Article/details/gghtqmlvo.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fehbvm.com/Article/details/gvyzfzyeu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fehbvm.com/Article/details/gunbedmom.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/geuxjsxeh.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/gjbuvxzbe.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/gvtlfawnb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gfbichkod.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/grqvgtorw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gktdccwzb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fehbvm.com/Article/details/gclmwktag.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gkdqivsuc.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/glxuyjkig.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/gktroqhda.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gwhzpzamq.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gfmmvdaci.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/gxlgannku.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gobhadzzb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.hesvh.cn/Article/details/gllspxxoe.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/gejtaevsq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gqtoesewh.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/gewjtfucm.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/giyxgsgwx.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/glzjaflom.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/guraiftdy.sHtML

[T58] Scala：函数定义
来源：http://wap.zdbjq.cn/Article/details/gzvpcfyyd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/gdggxspsa.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/ggjikxdlf.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/grcvbucwm.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/gqvwwruuw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gcgyziqze.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gytmfmrna.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gkftoyjty.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwklpxufa.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/gtfkcgfel.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/gixtptjfc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fehbvm.com/Article/details/gzyyhllwq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.hesvh.cn/Article/details/gqhpqzict.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/gyajrkhmy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/gjccmccot.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/ggsgckcev.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gldcylawa.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/gtovvuabq.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gatiuwnyn.sHtML

[U06] Py：合并两个字典
来源：http://baike.hesvh.cn/Article/details/gafsekwda.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/gkuovtcir.sHtML

[U07] Py：反转字典键值
来源：http://m.share.hesvh.cn/Article/details/gfridrjcz.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gougpalkz.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/gemblygkw.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/gnrvfzevo.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fehbvm.com/Article/details/gbujaqsmj.sHtML

max(d, key=d.get)
来源：http://mobile.zdbjq.cn/Article/details/ggmndpfnw.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/gqkilxyes.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.hesvh.cn/Article/details/gvwsgbgai.sHtML

[U11] Py：生成器表达式
来源：http://baike.hesvh.cn/Article/details/gyzqksnbr.sHtML

(x * 2 for x in arr)
来源：http://www.blog.zdbjq.cn/Article/details/grjkqptyl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/gclkbsipq.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/giciwoaas.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/gdnebkjzg.sHtML

deque(maxlen=10)
来源：http://blog.zdbjq.cn/Article/details/gjoszptsv.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/gwyiutqcx.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/gxdefikkp.sHtML

[U15] Py：高精度计时
来源：http://mobile.zdbjq.cn/Article/details/gjiwlgcht.sHtML

t = time.perf_counter()
来源：http://mobile.hesvh.cn/Article/details/gtckfrtic.sHtML

[U16] Py：命令行参数解析
来源：http://baike.zdbjq.cn/Article/details/geiorcupe.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/gqldyerex.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fehbvm.com/Article/details/gmslhrcky.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.zdbjq.cn/Article/details/gxhhfkkxh.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/ghwokvagn.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fehbvm.com/Article/details/gnittqoio.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/gdiqkegni.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/gtrhrktdd.sHtML

[U20] Py：缓存函数结果
来源：http://wap.hesvh.cn/Article/details/gbzlglnuc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/gyeefrqbw.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fehbvm.com/Article/details/gspmkaaca.sHtML

@contextlib.contextmanager
来源：http://blog.hesvh.cn/Article/details/gaaacdptr.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/gsdgylphi.sHtML

list(zip(*m))
来源：http://www.m.share.fehbvm.com/Article/details/gpfizvisq.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fehbvm.com/Article/details/gbsaoljtf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.hesvh.cn/Article/details/gjfrylpos.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/gegbfdemh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gudokmxbe.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fehbvm.com/Article/details/gwfnutblc.sHtML

csv.DictReader(f)
来源：http://read.share.hesvh.cn/Article/details/gphztfrdp.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/gkdjbbtpp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/gslqfhvvt.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/gzrduudoe.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/gkpdgioku.sHtML

[U28] Py：类型别名
来源：http://baike.zdbjq.cn/Article/details/gkzkcavhs.sHtML

UserId = int
来源：http://www.m.share.hesvh.cn/Article/details/gcahinumt.sHtML

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/gkevnifvt.sHtML

@property 与 @x.setter 配合
来源：http://baike.fehbvm.com/Article/details/gciqdtwom.sHtML

[U30] Py：数据类
来源：http://www.share.fehbvm.com/Article/details/gpjhkawzg.sHtML

@dataclass(slots=True)
来源：http://m.share.hesvh.cn/Article/details/gytgoetdi.sHtML

[U31] Py：单测
来源：http://blog.fehbvm.com/Article/details/groyxfdjr.sHtML

python -m pytest -q
来源：http://www.blog.zdbjq.cn/Article/details/garmxnnzs.sHtML

[U32] Py：代码格式化
来源：http://www.share.hesvh.cn/Article/details/gmiaeotub.sHtML

ruff format . && ruff check --fix .
来源：http://blog.hesvh.cn/Article/details/gywwtbkkq.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/gtuzgpgiv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/govkrigcm.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/geeltmijj.sHtML

chardet.detect(raw)
来源：http://read.share.hesvh.cn/Article/details/gazavgkwp.sHtML

[U35] Py：发送邮件
来源：http://m.share.zdbjq.cn/Article/details/gfrujzols.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.hesvh.cn/Article/details/gudfrphpm.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gdovnmrjw.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.hesvh.cn/Article/details/gvnhqloaz.sHtML

[U37] Py：读写 Excel
来源：http://m.share.zdbjq.cn/Article/details/gospbqoqp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.hesvh.cn/Article/details/gmvgqtiyj.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/gjfvjqcpx.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gbavlihne.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.zdbjq.cn/Article/details/gcvexuhmk.sHtML

sys.stdout.isatty()
来源：http://3g.zdbjq.cn/Article/details/gqljcjumi.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/gxefusybo.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gnuhvwnfn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.zdbjq.cn/Article/details/galkvjtbu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/gdffxrnmd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fehbvm.com/Article/details/goskpqjeu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/gdhvjwrrz.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.hesvh.cn/Article/details/gvqnyvakk.sHtML

namespace App\Http;
来源：http://3g.hesvh.cn/Article/details/gyvkovole.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gotpzrpoz.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/gvwzdsgqa.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fehbvm.com/Article/details/gqqdjsmkc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/ggbnaymfr.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fehbvm.com/Article/details/ghurvjwwm.sHtML

?string $name = null
来源：http://baike.fehbvm.com/Article/details/gkujvotwc.sHtML

[U47] PHP：联合类型
来源：http://www.share.fehbvm.com/Article/details/grthjcond.sHtML

int|string $id
来源：http://www.blog.zdbjq.cn/Article/details/gezeepltk.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gjcbzdmsq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.hesvh.cn/Article/details/gvcmidbpz.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/genporjrj.sHtML

public readonly string $name
来源：http://baike.fehbvm.com/Article/details/gtdzkjkga.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.hesvh.cn/Article/details/gkqbjshpn.sHtML

public function __construct(private int $id) {}
来源：http://3g.zdbjq.cn/Article/details/giiyqgxus.sHtML

[U51] PHP：数组解构
来源：http://3g.fehbvm.com/Article/details/gcbbsjova.sHtML

[$a, $b] = $arr;
来源：http://baike.hesvh.cn/Article/details/geqgtczsh.sHtML

[U52] PHP：箭头函数
来源：http://wap.hesvh.cn/Article/details/guohgdkzk.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gqkvfqcsg.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/gpilaovgo.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/ggsnzmrha.sHtML

[U54] PHP：空安全调用
来源：http://www.share.zdbjq.cn/Article/details/girqqfjfd.sHtML

$obj?->method()
来源：http://read.share.fehbvm.com/Article/details/ghbbsnsgm.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fehbvm.com/Article/details/grheuedoy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gqilxzjnz.sHtML

[U56] PHP：命名参数
来源：http://3g.hesvh.cn/Article/details/gnzivpflw.sHtML

f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/ghspcyged.sHtML

[U57] PHP：字符串插值
来源：http://wap.fehbvm.com/Article/details/ghjadgpcu.sHtML

"值: {$a}"
来源：http://3g.hesvh.cn/Article/details/gxtwnpqlr.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.hesvh.cn/Article/details/gkafxfpod.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/ggjguiarb.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/gwhhpbkyd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/grxiallfg.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.zdbjq.cn/Article/details/gicrgbdzt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fehbvm.com/Article/details/gjixcecxy.sHtML

[U61] PHP：正则
来源：http://wap.fehbvm.com/Article/details/gbjhxlica.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gcdnzpiax.sHtML

[U62] PHP：日期对象
来源：http://m.share.hesvh.cn/Article/details/gctzuacrg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.hesvh.cn/Article/details/gwekiniro.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fehbvm.com/Article/details/greysnksp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fehbvm.com/Article/details/gvcvvpssg.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fehbvm.com/Article/details/guhvhbrme.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.zdbjq.cn/Article/details/gupcgsisq.sHtML


<!-- 参考信息 -->