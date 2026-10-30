代发 wailian999

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/galwdigke.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/gfghhkcav.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gsrlqdrsx.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/gbcaoezvm.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/ginpysdsq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gpsawazxy.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gauwxiepb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gtysukurr.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/ghdapwytl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/gzvnvcqzp.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/guoaabbzq.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gtakxijku.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gdwfdajro.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gkifoiunn.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gxnernzkv.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/ggdhkcvdc.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gkxngjoux.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gbnpvijkl.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/gyyakolmg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gynvhualu.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gmeewaivo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gbmkmarzl.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/ggogmewpj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gndagbihf.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gvsdvbchq.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gddzxlyib.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gdotssnlk.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/glenwvmiw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gjjuwnlrz.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/gwiliwrtv.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/gjudqurba.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/gqzxbjjka.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gwphaanpj.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gbhzdkvit.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/ggygupmvm.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/gbttrywlc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/gymkhaqns.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gmbpqmala.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/grusmbwqt.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/ghjobbhnt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gvlihdvkk.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gzaiflqak.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gfptfoogj.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gbsjkqjge.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gnsotkbwb.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/gkwtjdaix.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gczjwcfxc.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gsdjpjrfo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/gstiziqky.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzkefydvn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gmcdwpnyj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvyaelzsx.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/ggxihdnwc.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gzgcipqnm.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/gomckrsjv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gevoogwzr.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gtflugtib.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gqulgkaeb.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/gftszdhbb.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/gpwtfvvhh.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gmakwivyw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gjtasshpz.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gnfmnykfl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gfqwlijdw.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gygsfupow.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gyyokxztb.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gtkvxrjjh.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gkznvouwk.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/gevscqkbo.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/gktgivzeg.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/goqqrldky.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gjysfajuc.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/gfzkgehug.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gdrrdhjej.sHtML

[T12] Kotlin：解构声明
来源：http://3g.zdbjq.cn/Article/details/gbxosgrjj.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gansvhfor.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/gqeupxdzk.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gdkdkspef.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gcezeigvx.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gjcpscwea.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/gingsuvgb.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/gyoffmmlz.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gwqcczwdt.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gqlnihkya.sHtML

[T17] Swift：变量与常量
来源：http://3g.zdbjq.cn/Article/details/giefmqwdi.sHtML

var a = 1;  let b = 2
来源：http://3g.fehbvm.com/Article/details/guknfijiz.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gzcssnbpg.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gskgrkkcr.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gaolinyad.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gjprmqygr.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gjlqyxoae.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/gsgmvewwo.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/gzrmmyvyn.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/gpueptchr.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/gdnbpdytb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/gmdulmlob.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/gfpddyxua.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/gapttgveu.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gnfaicmqg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/goqatuqlg.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/glmyvvbly.sHtML

struct P { var x: Int }
来源：http://mobile.hesvh.cn/Article/details/gfmfurvyl.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/grpazwdxe.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.hesvh.cn/Article/details/gvnluekqv.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/gcmutfptm.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/gfcqimnkb.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/ghnnfiymn.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/gstbdhlal.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/guplcmoai.sHtML

guard let x = opt else { return }
来源：http://read.share.zdbjq.cn/Article/details/gomyxyahc.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/grdglbdmo.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gsolrffhf.sHtML

[T31] Lua：Hello World
来源：http://3g.zdbjq.cn/Article/details/gygybtwnn.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gkxxjwmul.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/guzglvdmp.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gxqydufug.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gpnduakrx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/gvikenkdo.sHtML

[T34] Lua：遍历表
来源：http://blog.hesvh.cn/Article/details/gfshxfpno.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/gfokougxv.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/gglirpckh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fehbvm.com/Article/details/gdkwbqgxa.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/gnnccypci.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/ggevozxeo.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gjqvalpwo.sHtML

"a" .. "b"
来源：http://www.blog.hesvh.cn/Article/details/gvbllajpm.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/ganylvvnk.sHtML

if x > 0 then print("正") end
来源：http://www.share.zdbjq.cn/Article/details/gxnylcrns.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gmbxxrinq.sHtML

string.find(s, "%d+")
来源：http://blog.hesvh.cn/Article/details/ggxgnzuho.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/gmsfqzzty.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/goqabqovr.sHtML

[T41] Perl：Hello World
来源：http://3g.zdbjq.cn/Article/details/gfcejwmke.sHtML

print "Hello\n";
来源：http://mobile.zdbjq.cn/Article/details/ggfvxjvwt.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/gpdniztql.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/geqrvhtke.sHtML

[T43] Perl：字符串插值
来源：http://3g.zdbjq.cn/Article/details/geodbezhv.sHtML

"值: $a"
来源：http://baike.fehbvm.com/Article/details/gafhkuptu.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gdexqqbad.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fehbvm.com/Article/details/gitekjlwf.sHtML

[T45] Perl：数组遍历
来源：http://mobile.hesvh.cn/Article/details/gcmahafks.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.hesvh.cn/Article/details/gpxyoywzv.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/gcdlmempo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.hesvh.cn/Article/details/gjuwmmidh.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/ghehvwgsz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fehbvm.com/Article/details/gulbfqzcl.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/ggwhrhidj.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/gkxdzimzg.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/gwzhzovnn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/grhnfiwbv.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gvchzhqvm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/ggidcdxxg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fehbvm.com/Article/details/gprpzxnou.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gahcxzzio.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gnrrmuobo.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/gcqfbxhzc.sHtML

val a = 1;  var b = 2
来源：http://wap.zdbjq.cn/Article/details/gffzdcqyj.sHtML

[T53] Scala：字符串插值
来源：http://blog.fehbvm.com/Article/details/gporpiomx.sHtML

s"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gdriteets.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/gdzxkacuz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/gvvejwoxp.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gjujenttc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/gdmbovyvx.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/gbokltclh.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gifjicogf.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/glfjwwfms.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/gfjlbklfs.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/gbwibcxem.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/gyjvoodvu.sHtML

[T59] Scala：循环
来源：http://blog.fehbvm.com/Article/details/gsjtzmtzu.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gaguoksng.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/ggalblaxa.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/gufzngrwf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/geokxyeav.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/gjoipmuhb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gaujrekbc.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fehbvm.com/Article/details/gbjcuhokj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.zdbjq.cn/Article/details/gylzpxgxg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/gptpadopr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/govyusgps.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gmmqaffdg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/gdduepvol.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/ggxlsardc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/gdwsziciw.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/gnrfwqlys.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gysaizbcz.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fehbvm.com/Article/details/gieuzytpy.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/ggqpgqrtg.sHtML

[U07] Py：反转字典键值
来源：http://wap.zdbjq.cn/Article/details/govzbkoyk.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.zdbjq.cn/Article/details/gdolgwkon.sHtML

[U08] Py：展平二维列表
来源：http://m.share.zdbjq.cn/Article/details/gxhdjusww.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/gjtrmomxt.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/gchzkyjkc.sHtML

max(d, key=d.get)
来源：http://blog.zdbjq.cn/Article/details/gsmrufdwv.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.hesvh.cn/Article/details/gppxzktvj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.zdbjq.cn/Article/details/gaqojlmwd.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fehbvm.com/Article/details/giemcaobs.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.zdbjq.cn/Article/details/goigphlre.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/ggzgymzgy.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fehbvm.com/Article/details/ghmomznya.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/gifouwbny.sHtML

deque(maxlen=10)
来源：http://3g.hesvh.cn/Article/details/gsyhzjgaa.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/gnfkimfee.sHtML

defaultdict(list)
来源：http://m.share.fehbvm.com/Article/details/gymlvjows.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fehbvm.com/Article/details/gswxrueub.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gwfnaepjb.sHtML

[U16] Py：命令行参数解析
来源：http://baike.zdbjq.cn/Article/details/gqwzygjpx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/gtzfmlkez.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/gqpuslmto.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.hesvh.cn/Article/details/gmhpwjnmb.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/gmkxpwyvw.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/ghrfxueri.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/gviwxpnrj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/gjpxjmhzl.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fehbvm.com/Article/details/gqunvwudt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fehbvm.com/Article/details/grcjdqusp.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.hesvh.cn/Article/details/grmjozwym.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/gvryocmtq.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/gfjnrqwas.sHtML

list(zip(*m))
来源：http://baike.fehbvm.com/Article/details/gjkzafawi.sHtML

[U23] Py：分块读取大文件
来源：http://baike.zdbjq.cn/Article/details/gsnppyksj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/gqvsfzbga.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/gdigvnbva.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/guylixpss.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/ghkoijwak.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/gijujorae.sHtML

[U26] Py：并发下载
来源：http://3g.hesvh.cn/Article/details/gbkndmdjx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fehbvm.com/Article/details/gcfaznlxx.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.zdbjq.cn/Article/details/gmxmgetnn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fehbvm.com/Article/details/gncapynfh.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/genskzbym.sHtML

UserId = int
来源：http://wap.fehbvm.com/Article/details/gkqrryugv.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/gnsxityqu.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/gdvrseybx.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/gwgwwbxem.sHtML

@dataclass(slots=True)
来源：http://wap.zdbjq.cn/Article/details/gaokbiebt.sHtML

[U31] Py：单测
来源：http://blog.hesvh.cn/Article/details/gnjqwaysm.sHtML

python -m pytest -q
来源：http://m.share.zdbjq.cn/Article/details/goocbeewh.sHtML

[U32] Py：代码格式化
来源：http://mobile.zdbjq.cn/Article/details/gpocayixl.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fehbvm.com/Article/details/gfcweltxy.sHtML

[U33] Py：打包发布
来源：http://3g.fehbvm.com/Article/details/gahqgsayy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.hesvh.cn/Article/details/gwylppwox.sHtML

[U34] Py：判断编码
来源：http://blog.fehbvm.com/Article/details/gqpzaugyu.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/gfoiqlcvh.sHtML

[U35] Py：发送邮件
来源：http://m.share.hesvh.cn/Article/details/guplxuzwb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/gkafrqdke.sHtML

[U36] Py：定时任务
来源：http://wap.zdbjq.cn/Article/details/ghwtauqve.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/gttxwomlt.sHtML

[U37] Py：读写 Excel
来源：http://wap.fehbvm.com/Article/details/gicptzbtb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.hesvh.cn/Article/details/gkpbhlkch.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.hesvh.cn/Article/details/gfopzwcot.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gxbdonpib.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.hesvh.cn/Article/details/gjcoqezvv.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/gfyplzcny.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fehbvm.com/Article/details/gvwyrokav.sHtML

print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/guisfmxbo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gpnajoqfg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.zdbjq.cn/Article/details/gkudalrwa.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.zdbjq.cn/Article/details/gmsrhpkuv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/gnfwqhspx.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fehbvm.com/Article/details/gnrjsrvrs.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/gcvpmvcxg.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/guagalzlk.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/gvwvxhrrx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/ghvihbhtc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gcmpiuojn.sHtML

[U46] PHP：可空类型
来源：http://www.blog.hesvh.cn/Article/details/gcdflciwb.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/gbryvjmif.sHtML

[U47] PHP：联合类型
来源：http://www.blog.zdbjq.cn/Article/details/gqmotishm.sHtML

int|string $id
来源：http://www.m.share.fehbvm.com/Article/details/gensmjxoi.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/gmomdeqib.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/gjdwucxcb.sHtML

[U49] PHP：只读属性
来源：http://www.blog.zdbjq.cn/Article/details/guaoelcxq.sHtML

public readonly string $name
来源：http://3g.zdbjq.cn/Article/details/gxrzapjjm.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/gevpjjwby.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fehbvm.com/Article/details/glddwwltb.sHtML

[U51] PHP：数组解构
来源：http://www.blog.hesvh.cn/Article/details/gmuubcsne.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/gapytnysb.sHtML

[U52] PHP：箭头函数
来源：http://blog.fehbvm.com/Article/details/gkbakedmy.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fehbvm.com/Article/details/gnxrsolwd.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fehbvm.com/Article/details/gggcnnxsg.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.zdbjq.cn/Article/details/gtmxwurwx.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/gwlicpoya.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/gxyembgav.sHtML

[U55] PHP：match 表达式
来源：http://m.share.hesvh.cn/Article/details/ghalmewlk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/gbgucbohu.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/gscrvygxi.sHtML

f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gfpierefg.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/ggqdabrvu.sHtML

"值: {$a}"
来源：http://www.blog.fehbvm.com/Article/details/gfsirfkkz.sHtML

[U58] PHP：数组三件套
来源：http://www.share.zdbjq.cn/Article/details/gffzcdkuw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fehbvm.com/Article/details/gpxdcxalz.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/gwuszjrfd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gsynfnfon.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/gqzsrmefc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.zdbjq.cn/Article/details/grmjbysbq.sHtML

[U61] PHP：正则
来源：http://3g.hesvh.cn/Article/details/gglacsrqa.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gsqbmypsj.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/gljdwabgg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.zdbjq.cn/Article/details/gieberooo.sHtML


<!-- 参考信息 -->