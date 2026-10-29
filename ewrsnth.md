代发 wailian999

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/grrrrjuou.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gbnrikskf.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gfswhruak.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gojilpdgn.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gonokmnuc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gjcsfyyju.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gcmzvjnkb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/gdijeikaq.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/ghqdqbqoy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/gejzcfxcz.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/gttzbnzvt.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/ggestqmbk.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gczhoangj.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/gzyqjthan.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gcalmkfct.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghmkpyfxo.sHtML

[S45] C++：lambda
来源：http://baike.fehbvm.com/Article/details/gdvtnmcaz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/gwmbkvnhe.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gskvjkjdo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gsxryeqin.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/grvrsjuot.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gleqvllym.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/geziaeams.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gbdpzupao.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gyqnfnthe.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/greaygjtr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gwphmavoq.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gdocmmzeh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gyzidduwf.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gdthugggg.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gxfdbgwtr.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/gchdpjuiw.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gtbvjxiwk.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gtumkbiri.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/ghnremqcx.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gjoaxstph.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/guxrjxyox.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gmvyyxywa.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gcbjmpzvq.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gxzphifgh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gvvjfjtsk.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/geymwrymb.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gfkbehpge.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gtfxndpac.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gewjfkecr.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gehnyhnmk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gcztcuwut.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gskxhwpyo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/guufrwahn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/griqkxvcu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gyjvovfkc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjaabrlfs.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gsposbvmy.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/guwfgmbik.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gopqudfup.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gafwsglcn.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/gncgpohto.sHtML

"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gmpwlrjbg.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/gipnswspi.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gfmjuanfy.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/ghchswotr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/gjzfvcmgc.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/geyukedlq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/guvaxjfrb.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gajmxfulr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gbxfvgqmb.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/grwlarfkv.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/geupptygy.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/gcbezhizp.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/guivrmcdz.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gqdqznxji.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gxeubtrcs.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gssbjojod.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/gffwixikp.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/gtgivmtgx.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gfapwpquf.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gnawgcnam.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/gqqiiubcl.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gilouasjb.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gcbnbfojs.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/ggkrppgyc.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gmuvobync.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gmkmouujv.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gyielqksw.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gcsmbthkn.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gobgwufix.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gugdhlphp.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/gafkelbdi.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/gkzavzgdp.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/gdbtvepiw.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/gsvkttgcr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gtqrpjimk.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/gdzkmonwl.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/gwpbmsgwc.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/gwwoujijw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/gbtlabjtj.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/gpmxkrabh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/ggkmjvffn.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/gwvwtysah.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gluipjzqh.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/gfobdjafd.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gjdfvbiim.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/gdwiiyvya.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gtibvzddt.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gduqowlnq.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gssdmhrii.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/gdzkzeqds.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gfudeckij.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gwaceilym.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/gsgmuunqz.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/gfgzenwbz.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/gbyfnzzvh.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gyvetkqnw.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gaffooguj.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/gignqoais.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gmwydqyga.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fehbvm.com/Article/details/gsejjltke.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/gvozqvgzi.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/gfajgktjo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/gfmuqcizj.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gcflmcoqu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/ghiuturnm.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/gmomvmnom.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/gaalrszea.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gemoipqxk.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/grreusihg.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gnfhsazax.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gftxmlmle.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gkofvrqrs.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gfwiqkvpt.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gmuhzdxep.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/gjcowlwfj.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/ghawpabxb.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gulpylwck.sHtML

[T42] Perl：变量类型
来源：http://m.share.hesvh.cn/Article/details/gahxtfbsm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.hesvh.cn/Article/details/gzqgfehvz.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/gayehezca.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gnwbalowj.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/gpmjnvwaa.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/gytbdvzza.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/gcomzkaxj.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fehbvm.com/Article/details/gdkgqxwph.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/gajscnduv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzplkdmvf.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/gwqmhasjy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/gnockubhw.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gttuxxmoj.sHtML

$s =~ s/old/new/g;
来源：http://baike.hesvh.cn/Article/details/gzvhuedwv.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/gddqnamya.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gausmjito.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gacqlosio.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.zdbjq.cn/Article/details/gkhmkepki.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.zdbjq.cn/Article/details/gfingzgny.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/gvarcoyru.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gldejbuux.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gllpptzoe.sHtML

val a = 1;  var b = 2
来源：http://read.share.hesvh.cn/Article/details/gawbvtgqv.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/ginbdtjdd.sHtML

s"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/ggghcjdan.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gwpogzgjy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fehbvm.com/Article/details/glmxrmyzc.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gnedlgekb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fehbvm.com/Article/details/gnysevfje.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/gctsmmgme.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/gluyknxgg.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gpxwswdyu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gbnugyaia.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/gpmvqmykd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/gpkiaxuwj.sHtML

[T59] Scala：循环
来源：http://wap.fehbvm.com/Article/details/gqpxfaiqc.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/gnsfboiox.sHtML

[T60] Scala：折叠
来源：http://baike.hesvh.cn/Article/details/gvmnnzjue.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gtbkoseet.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtbuzrpae.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/gdqrsiyzs.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/goggoppen.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/gurzprcpw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/gnayyjufj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.zdbjq.cn/Article/details/gmkvmxmkx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/gcpeceswq.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.hesvh.cn/Article/details/glcgqyfml.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/gbutmgmht.sHtML

[U04] Py：变量调试打印
来源：http://baike.fehbvm.com/Article/details/gwzbgkohr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/grayokbqd.sHtML

[U05] Py：列表去重且保序
来源：http://blog.zdbjq.cn/Article/details/grysfmsox.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gxdgobtmk.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/ggbpddxgu.sHtML

{**a, **b}
来源：http://baike.fehbvm.com/Article/details/gkxlmnwgp.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fehbvm.com/Article/details/gpczwhahz.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gajawbqlp.sHtML

[U08] Py：展平二维列表
来源：http://blog.fehbvm.com/Article/details/grfbyvslb.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/gbnjlrkgp.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/gqtqddqwk.sHtML

max(d, key=d.get)
来源：http://read.share.zdbjq.cn/Article/details/ggympjfud.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/gmxuaozcm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/gwhpxnkcl.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/gttbokdpv.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/gqhyhedkq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/gsyyabcej.sHtML

Counter(arr).most_common(3)
来源：http://blog.fehbvm.com/Article/details/gecsharjx.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.zdbjq.cn/Article/details/gvitxogim.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/gskvfbyyz.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/gzwffwpyy.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/gdbbxxbsh.sHtML

[U15] Py：高精度计时
来源：http://mobile.fehbvm.com/Article/details/gwjebrznn.sHtML

t = time.perf_counter()
来源：http://baike.zdbjq.cn/Article/details/gnumhslkw.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fehbvm.com/Article/details/gdfzrbvds.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.hesvh.cn/Article/details/glfxyrwny.sHtML

[U17] Py：初始化日志
来源：http://read.share.fehbvm.com/Article/details/gydxjzgnf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/gwhvcggyi.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/gxtdlokyb.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.hesvh.cn/Article/details/gplyzhgoi.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/ggknkdzqs.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/gjuswuvxj.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gotwztkmx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/gryiifygr.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/gpkcvwicl.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/gzxbuxnpk.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/gieywkoql.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/glbyyfzrf.sHtML

[U23] Py：分块读取大文件
来源：http://3g.zdbjq.cn/Article/details/gbtbddcpv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/gcwdxzqoc.sHtML

[U24] Py：路径操作
来源：http://read.share.fehbvm.com/Article/details/gtubhovrl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gzqgfjous.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/gdyodrjkd.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/gaczllvno.sHtML

[U26] Py：并发下载
来源：http://m.share.fehbvm.com/Article/details/gcfqiocny.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/ghkrbxyhm.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.zdbjq.cn/Article/details/gnkykhfzk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/gdlfjiepj.sHtML

[U28] Py：类型别名
来源：http://www.blog.hesvh.cn/Article/details/ggckhuhgn.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/gfzotlyng.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/gewecelmp.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/ggqghtgkv.sHtML

[U30] Py：数据类
来源：http://blog.hesvh.cn/Article/details/goxmoqtwr.sHtML

@dataclass(slots=True)
来源：http://read.share.hesvh.cn/Article/details/gofsseasf.sHtML

[U31] Py：单测
来源：http://wap.zdbjq.cn/Article/details/ggaxiqyos.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/gyahvknft.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fehbvm.com/Article/details/gtdpgtmey.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fehbvm.com/Article/details/gqgubwhna.sHtML

[U33] Py：打包发布
来源：http://www.blog.fehbvm.com/Article/details/gqnzklnpd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.zdbjq.cn/Article/details/gikyqhwcv.sHtML

[U34] Py：判断编码
来源：http://m.share.zdbjq.cn/Article/details/gvlrwbwno.sHtML

chardet.detect(raw)
来源：http://blog.hesvh.cn/Article/details/gpwukmcsz.sHtML

[U35] Py：发送邮件
来源：http://m.share.hesvh.cn/Article/details/gbkcxltgx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/goajhogvo.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fehbvm.com/Article/details/giagdosuk.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fehbvm.com/Article/details/gtuddsuks.sHtML

[U37] Py：读写 Excel
来源：http://www.share.hesvh.cn/Article/details/guwnxlwoi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.hesvh.cn/Article/details/gwbuhdgtz.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fehbvm.com/Article/details/gxqybdsci.sHtML

Path(__file__).resolve().parent
来源：http://read.share.zdbjq.cn/Article/details/ggvbgonhx.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.hesvh.cn/Article/details/gyydjslbp.sHtML

sys.stdout.isatty()
来源：http://baike.zdbjq.cn/Article/details/gwczkojoh.sHtML

[U40] Py：打印到标准错误
来源：http://baike.zdbjq.cn/Article/details/gqnpaqrsu.sHtML

print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gkpeatsgi.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.zdbjq.cn/Article/details/gzxlupbfw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fehbvm.com/Article/details/gdynevfcr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.hesvh.cn/Article/details/grqauqtsc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.zdbjq.cn/Article/details/ghayvshnn.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/gkxfedqdw.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gbgbxymkl.sHtML

[U44] PHP：开启严格类型
来源：http://3g.zdbjq.cn/Article/details/gcxjujhoz.sHtML

declare(strict_types=1);
来源：http://wap.zdbjq.cn/Article/details/gwoakdajn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fehbvm.com/Article/details/gwblltbyz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gnesvvipm.sHtML

[U46] PHP：可空类型
来源：http://read.share.hesvh.cn/Article/details/gyauhbuvf.sHtML

?string $name = null
来源：http://blog.zdbjq.cn/Article/details/gcpcfkism.sHtML

[U47] PHP：联合类型
来源：http://3g.zdbjq.cn/Article/details/gsitpaarf.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/gghclbxvg.sHtML

[U48] PHP：纯枚举
来源：http://blog.zdbjq.cn/Article/details/gfxympiwv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fehbvm.com/Article/details/gikkczvae.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/goelssffa.sHtML

public readonly string $name
来源：http://wap.fehbvm.com/Article/details/gnswfwrrg.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/gcghwgyak.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/gomrgsxct.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/gvpeyqbvb.sHtML

[$a, $b] = $arr;
来源：http://baike.hesvh.cn/Article/details/gkpxlmnce.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gmttkkync.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gzsjfpwhy.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gurkojamk.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fehbvm.com/Article/details/geysjebsj.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.hesvh.cn/Article/details/gsrxckiof.sHtML

$obj?->method()
来源：http://mobile.fehbvm.com/Article/details/gwfrukmpl.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fehbvm.com/Article/details/gslgsoohk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/gzwlpgbzk.sHtML

[U56] PHP：命名参数
来源：http://mobile.fehbvm.com/Article/details/gaijfnoht.sHtML

f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gjfrwhkpy.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gdeqneryn.sHtML

"值: {$a}"
来源：http://wap.zdbjq.cn/Article/details/gqzreandu.sHtML

[U58] PHP：数组三件套
来源：http://baike.hesvh.cn/Article/details/gokikcukr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.zdbjq.cn/Article/details/gqbmeitpi.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/gewgqyzhz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gbdhzvtew.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.hesvh.cn/Article/details/giwppjdhb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/gstneefih.sHtML

[U61] PHP：正则
来源：http://baike.fehbvm.com/Article/details/grrtjtqhj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gnnnzymgi.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/gkmvsgzyv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.zdbjq.cn/Article/details/goaawkxwx.sHtML


<!-- 参考信息 -->