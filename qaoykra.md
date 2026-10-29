代发 wailian999

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gjgbougkh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gtisnluwb.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gpybceqxs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/grupxyxoi.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gtfpztvjo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gdxtejgph.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/guaptgcsf.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gftshyhxj.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gvszdpsod.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/gcqkwrgph.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/ggvsniqla.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gngzifdpb.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/geohiwewr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/gmzsrpbgl.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gewdcxgua.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gmkjqgvdu.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gfabxjpav.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gismgauzt.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gwtvzecek.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/gosfpzpxg.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gdluvxakr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/guxstwsuk.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/gfwxggrpj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gxrqlvogt.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/ghcswcmgh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/giymopmoi.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gdvotspyj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/ggngoihst.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/ggyvkzidu.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gbvxitkbt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/gtiutxazb.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/gvyidzggk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gpgvsodkx.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/gursycsgb.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gomfcrhlf.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gdhsivqot.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/guvwvnvus.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gqvrjtccw.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/giyroomsa.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/gguvcrjsu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/gsondanwv.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gsafujtuw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/gkskamurb.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/ghzcujmio.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gtntsiqbh.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gmffymwgq.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gjwhiwjiq.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gbrcwtgbp.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/ghmdphnik.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gysredjac.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/gvlkcselh.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/gkdunhkpt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/giezmspxj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggiteitot.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gtvxhlqbu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmtxfdgle.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gdvgbtzdc.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gdsxsbyhc.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/givrzwcwe.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gvibvvche.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/gswdhhksu.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gacoajhfy.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gwnhusyiv.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/gewsgnxve.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/gxovtvdxd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gjczvmyks.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gbbrhdsgr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gpimuyssx.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gugynrqku.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/grsrzrwzd.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/gyqwetafj.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/ghrugjvdh.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gysfphust.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/gfazgrdsc.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/gkvpbosoh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gbmrxovhs.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/gxtobuaps.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/guobeckvr.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gzooliczq.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gdzfwwhdy.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/gvvpdhyof.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/glrjwuhai.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gewxzvyke.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gdeqzrodc.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gfhqmjahu.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/glslxadzn.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gjcfjqksi.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/ghpledefy.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/grhpiufmu.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/gbhfdojqn.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gwismprps.sHtML

"值: \(b)"
来源：http://m.share.fehbvm.com/Article/details/gurxjdlqv.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/gzifddhmf.sHtML

if let n = opt { print(n) }
来源：http://3g.fehbvm.com/Article/details/ggfxcxesg.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gsmuivkhm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/gtxzmqheu.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/gsbjymqly.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/gveweyovw.sHtML

[T22] Swift：字典
来源：http://blog.fehbvm.com/Article/details/gnslwthgd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gtwmcgrwi.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/ghblpwqet.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fehbvm.com/Article/details/gfmjmhcrc.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/gzmurgjgo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/guvocalss.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/guxhybliy.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/goypcysyf.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/gbstknzdw.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/gkdpkbejr.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/gpxatotpp.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/givmqitat.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gnasbbllh.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/gblnyqauh.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gpnedxwyf.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gkaopyaug.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gtlhesuww.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/gvovmmbfy.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gxdnermal.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gppixicmf.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gumneyomp.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/gdavfyjgj.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/grvdqiybh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/gwmwrepzj.sHtML

[T34] Lua：遍历表
来源：http://blog.fehbvm.com/Article/details/gdakklvup.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/gfcixddfu.sHtML

[T35] Lua：字典表
来源：http://blog.fehbvm.com/Article/details/gwbjpeopb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gsudjnsho.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gopwlcerx.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/ggslohnkz.sHtML

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/gqbkzwawt.sHtML

"a" .. "b"
来源：http://www.m.share.hesvh.cn/Article/details/gyhlzfgtf.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/gbyytcngt.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/ggsudppyf.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gpllcanfd.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/gbvuoszrh.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/gwkxhtxda.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/gpzxlqosl.sHtML

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/gzssjwdbz.sHtML

print "Hello\n";
来源：http://wap.hesvh.cn/Article/details/gwbmckvys.sHtML

[T42] Perl：变量类型
来源：http://m.share.fehbvm.com/Article/details/gnljzypzk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/ghypnnziv.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/grqiuqaqd.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gfvljxykf.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/gdkyqqpbf.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/glxciqxot.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/gnyuhfsos.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/gyrxqmscq.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/gdbfpqyxx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/gsagnpzhz.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/gjedibpwd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/gzlbzobkf.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/gontbwfee.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gfffdefra.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gzmjdzzbj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gvdmaesgf.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gpkxofrpj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.hesvh.cn/Article/details/gksehcmbn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.hesvh.cn/Article/details/gbwcwrsse.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gkphiddxp.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gigjnleqf.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/gvdrnqayc.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gfjhxbuxb.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gkhxrmeaf.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/ghhhntkts.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gookqgzgo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/gjcrmpaba.sHtML

[T55] Scala：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gtzsjnptc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/grpwnrram.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/gzgxeevdw.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gxkxvhylg.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gmiseswvw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gjukzqdfn.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/gpntnjfkr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fehbvm.com/Article/details/gaeuuohbp.sHtML

[T59] Scala：循环
来源：http://www.share.hesvh.cn/Article/details/gesabzinn.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gzbecslxa.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gnljpemdq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/ggqkddmop.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gawtdfjxj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gsldbyjco.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzswefnty.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gnajtaqow.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/glfwfpqwc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/ghsaypmal.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/gibsgrvxm.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.hesvh.cn/Article/details/gfxijcthx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/ghammdfiw.sHtML

[U04] Py：变量调试打印
来源：http://3g.hesvh.cn/Article/details/gdkpiezmc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/gqjfvaupu.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/gvuxauukf.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/grcvncspm.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/gyggqhzmj.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gllnfkvzo.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/gwmmnbfit.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/gxwuzodlj.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/gijeaopfv.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gwisqlkdr.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gkkjgkjto.sHtML

max(d, key=d.get)
来源：http://read.share.zdbjq.cn/Article/details/gasluqbjp.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/grwgeazdj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gualpujdn.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/gfdesjfow.sHtML

(x * 2 for x in arr)
来源：http://3g.fehbvm.com/Article/details/gxgnuhxlb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/ghwngxijt.sHtML

Counter(arr).most_common(3)
来源：http://www.share.zdbjq.cn/Article/details/ggpiebkpe.sHtML

[U13] Py：固定长度队列
来源：http://read.share.zdbjq.cn/Article/details/gbxhpvvtp.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/gcepejsfe.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.zdbjq.cn/Article/details/gkynpcxux.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/giawbozch.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/ggupfpcig.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/gricyrjxh.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/gnjcuaajb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/gkhlwplaa.sHtML

[U17] Py：初始化日志
来源：http://wap.hesvh.cn/Article/details/gmlzrlygd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/gcbdbsgtg.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/gmqgmbogw.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/grbkpesxq.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/gllmmmxbw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.hesvh.cn/Article/details/gusbidhik.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fehbvm.com/Article/details/grdrnckpg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/ghzjkrhvr.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/gllbntkzv.sHtML

@contextlib.contextmanager
来源：http://m.share.fehbvm.com/Article/details/gnwlyuywr.sHtML

[U22] Py：矩阵转置
来源：http://baike.hesvh.cn/Article/details/gulvgrlbv.sHtML

list(zip(*m))
来源：http://baike.fehbvm.com/Article/details/gskhryolj.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fehbvm.com/Article/details/gyuasstgq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.hesvh.cn/Article/details/ggvisegjm.sHtML

[U24] Py：路径操作
来源：http://www.blog.fehbvm.com/Article/details/gauycuima.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gqifbszoe.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/ghqbcggdy.sHtML

csv.DictReader(f)
来源：http://www.m.share.hesvh.cn/Article/details/gjnwpepkk.sHtML

[U26] Py：并发下载
来源：http://blog.fehbvm.com/Article/details/gxuposgkq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fehbvm.com/Article/details/gadcdbyct.sHtML

[U27] Py：异步 HTTP
来源：http://blog.zdbjq.cn/Article/details/gngwgjfhu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.hesvh.cn/Article/details/ghfofooje.sHtML

[U28] Py：类型别名
来源：http://3g.fehbvm.com/Article/details/guqkcrese.sHtML

UserId = int
来源：http://read.share.zdbjq.cn/Article/details/gjdybmbyg.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/gbsweeyks.sHtML

@property 与 @x.setter 配合
来源：http://m.share.zdbjq.cn/Article/details/gkmorxjqo.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/guquurggu.sHtML

@dataclass(slots=True)
来源：http://www.share.hesvh.cn/Article/details/gbesbayla.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/geovqqdff.sHtML

python -m pytest -q
来源：http://baike.fehbvm.com/Article/details/ggpkstody.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gcspyrjej.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fehbvm.com/Article/details/gcunlzmsg.sHtML

[U33] Py：打包发布
来源：http://www.share.fehbvm.com/Article/details/gzptrremi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.zdbjq.cn/Article/details/gzdaqsadv.sHtML

[U34] Py：判断编码
来源：http://baike.fehbvm.com/Article/details/gniwrszss.sHtML

chardet.detect(raw)
来源：http://www.m.share.fehbvm.com/Article/details/gpevghbch.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/ggklcqcrj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fehbvm.com/Article/details/gcnmulelp.sHtML

[U36] Py：定时任务
来源：http://blog.hesvh.cn/Article/details/gglexbeuw.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.zdbjq.cn/Article/details/guqgozghn.sHtML

[U37] Py：读写 Excel
来源：http://mobile.zdbjq.cn/Article/details/gafbjbhbm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fehbvm.com/Article/details/gswqfztyd.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fehbvm.com/Article/details/gnbeqtgvq.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.hesvh.cn/Article/details/gxajzzxqd.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/gnyljlcco.sHtML

sys.stdout.isatty()
来源：http://www.share.fehbvm.com/Article/details/gzsxfnsng.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fehbvm.com/Article/details/gxymrldad.sHtML

print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gbvkxdrmx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/gvyaaorpk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fehbvm.com/Article/details/gqaobmjjy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fehbvm.com/Article/details/gppfjtmfo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fehbvm.com/Article/details/gzbazkaba.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.zdbjq.cn/Article/details/gwsfbqntx.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/gaswtkien.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/gbrvnqhpb.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/gsldzztyc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fehbvm.com/Article/details/ghiykyhbe.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gjspboxan.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/gigrdbfuv.sHtML

?string $name = null
来源：http://m.share.hesvh.cn/Article/details/gknjazpwy.sHtML

[U47] PHP：联合类型
来源：http://www.share.hesvh.cn/Article/details/gslpevgmk.sHtML

int|string $id
来源：http://m.share.fehbvm.com/Article/details/gagtvbjbb.sHtML

[U48] PHP：纯枚举
来源：http://read.share.zdbjq.cn/Article/details/glmwfhhrq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fehbvm.com/Article/details/gdxswtruc.sHtML

[U49] PHP：只读属性
来源：http://blog.zdbjq.cn/Article/details/gqlcxyxym.sHtML

public readonly string $name
来源：http://www.share.hesvh.cn/Article/details/gpkflquch.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/ggssobufa.sHtML

public function __construct(private int $id) {}
来源：http://baike.zdbjq.cn/Article/details/gvxiqjvco.sHtML

[U51] PHP：数组解构
来源：http://baike.fehbvm.com/Article/details/gxeovbrqu.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fehbvm.com/Article/details/gazylfqts.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gducyelxy.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/goeydejob.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/gyoshtzno.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.zdbjq.cn/Article/details/gedbgwtkn.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/gxuqsatfi.sHtML

$obj?->method()
来源：http://m.share.zdbjq.cn/Article/details/gijttwitn.sHtML

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/gefjxjxpu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fehbvm.com/Article/details/grspaxora.sHtML

[U56] PHP：命名参数
来源：http://m.share.zdbjq.cn/Article/details/gcepadxkb.sHtML

f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gvprkbwbs.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gsjybfgss.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/gvlbzoltt.sHtML

[U58] PHP：数组三件套
来源：http://wap.hesvh.cn/Article/details/gtfwqukmd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.zdbjq.cn/Article/details/giodhxfrh.sHtML

[U59] PHP：自定义排序
来源：http://3g.fehbvm.com/Article/details/gnvpfodwf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gegnuahbc.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.hesvh.cn/Article/details/ghdiufxud.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.zdbjq.cn/Article/details/gubqsjtwq.sHtML


<!-- 参考信息 -->