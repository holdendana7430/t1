代发 wailian999

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gsexbhidg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gglebmkxk.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gsprmmvjt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/ghdfyzuce.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gvylxpbwn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gjrchcowg.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gqymksebc.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gygzyiwlo.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gfsiwwdgw.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/guxryshoy.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/ghdgfcmqg.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/gvetkyrev.sHtML

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/gjmzsbwac.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/gxfkkbmnz.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gbipembjn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gjhxvlesp.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/gubvxuggb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gkoxyxula.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gtxnadobk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gzkdddfcp.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gqlvusfkb.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gewmhcozw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/gkovwhemb.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/gpmaqmpwo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/ghqfuajyr.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/ggnffmksj.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gbfpdoacv.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/grppiupbm.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gwreowvqf.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/grwknsjhn.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gcyzbveik.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/genbrugql.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.zdbjq.cn/Article/details/gwddllxul.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gyvkyrspo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gxtstdwou.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gtokjdpln.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gnlxovrzw.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/glgxugzcd.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/gxibfyacs.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gheqlwabi.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/geetxgcdb.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gisxcrylv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/gvwebkueq.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gyxkvmvqt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gccaotksp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmizmzwzq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gomfrfdmk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gafgeiylj.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gtwwtdtrv.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gyczawile.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/gfimohrft.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gnlhkphpy.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/gqyiffrap.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/grrbvequy.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/gpfbheiaq.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gasavebyu.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gstvhkwtw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/ghuculyra.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gxwzagbgp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/gakfkcrxa.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/giepmsphm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/gvkpjjuxf.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gyccklzhr.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/gleppqnwj.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gpwkbodsz.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/gjprihwtv.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/glczineue.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gqkytnbjr.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gtksbavvq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gwlroakem.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/gfrbqhlqj.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gfbokihwy.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gkkuxsdoj.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/gxohptvwu.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/grhgusvin.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/geiiyeclw.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gfagzhdpo.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/gtvinwqgp.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/gxrhmqrqh.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gwpqfipjk.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/gmnunpkdk.sHtML

var a = 1;  let b = 2
来源：http://3g.hesvh.cn/Article/details/gryzyeskx.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/ggetyuxdk.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gbebhmqrk.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fehbvm.com/Article/details/geqssbxaw.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/gjayewunb.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gugtzexwc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/ghlezlupr.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/ghkmiibhg.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/gxekmxzhr.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/gzakcnzkq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gthhwovuu.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gargixlwz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gwncuxnyn.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/gnpkjmgnn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gpyfevzaz.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gxmfznbmh.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gmowpwgrw.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/gghzrdhst.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gyoaeczxp.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gbrmmkujq.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.hesvh.cn/Article/details/gsrqbphpe.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/gwxybrnrm.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/gnpcphznz.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/gvhspwlah.sHtML

guard let x = opt else { return }
来源：http://3g.zdbjq.cn/Article/details/gvbvepbqz.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/gipcvlycw.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gcckewwtd.sHtML

[T31] Lua：Hello World
来源：http://blog.zdbjq.cn/Article/details/giwmhmith.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gelnyfomc.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/gaybshygi.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/gvgjogncz.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/gxuxcfgpi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/guyxdzoct.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gnzvltkks.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/gxyjqovpe.sHtML

[T35] Lua：字典表
来源：http://blog.fehbvm.com/Article/details/glllyxmti.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fehbvm.com/Article/details/ganhugouo.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/gqjrepzfj.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/gkanciynq.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gnvvjljpn.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/gedmjviib.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/gxmcaltdb.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/gyrnfmqcs.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/ggaqmpyhv.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gxrlwvfav.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/gmlsegtzk.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/gvfracdii.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/gonwdfslq.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gnbaoksod.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/guwbrbfjz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/gbwjmbsny.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gozgjsccq.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gbnxfvscg.sHtML

[T44] Perl：条件
来源：http://read.share.hesvh.cn/Article/details/gqlxsvmya.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.hesvh.cn/Article/details/gtquklydj.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/gwemvvuaq.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfgrmnpur.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gsdblrtqc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/gpwleddjl.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/gkaovvrhe.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/grmxuyqeu.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/guirokmxp.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/gzdfjkgyv.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/ghhbsolwq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/grzqznulz.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gbkijuwnk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/gqocbzdkj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.zdbjq.cn/Article/details/gmllvtarj.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/ggkwlfsij.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gsqpexgza.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/gxqubbalp.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/garrhzkry.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/grcajlsra.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gpudpukbw.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/gonuplyar.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fehbvm.com/Article/details/ggwaxtcwb.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gsifbzzja.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/gkbzmlafz.sHtML

[T56] Scala：样例类
来源：http://www.share.hesvh.cn/Article/details/gmyrlvvdf.sHtML

case class User(name: String, age: Int)
来源：http://blog.hesvh.cn/Article/details/gsyynrkwu.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/gtftzqtom.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/gsgurnwak.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/gclelrlrz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/gehuqggxy.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gdsbhjqyj.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gdatgwrjy.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/gbepyagho.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/gsdhjelma.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsvmllnhx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gzsqkphld.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvoplamir.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gkiompaxq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.hesvh.cn/Article/details/gbmehjxoc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/gbifannlk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.hesvh.cn/Article/details/gflwhhwyf.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gtabqquwa.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/ghplrcqar.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/giqqljxtl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fehbvm.com/Article/details/gffekffqr.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/geotyqlmm.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/ghziaixkj.sHtML

[U06] Py：合并两个字典
来源：http://read.share.zdbjq.cn/Article/details/ggtzwskbr.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/gaightgca.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.hesvh.cn/Article/details/gevxroepc.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fehbvm.com/Article/details/gahkvgevw.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/ganjylaus.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fehbvm.com/Article/details/gndonwvrj.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/gtnkleqwn.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gsitgoieo.sHtML

[U10] Py：按值排序字典
来源：http://baike.zdbjq.cn/Article/details/gpaiysdgi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/gddgmodme.sHtML

[U11] Py：生成器表达式
来源：http://blog.zdbjq.cn/Article/details/gtkbdjxbx.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.hesvh.cn/Article/details/gxcaudlbl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/gylagvuan.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gkwjckzww.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/gsqcdmtxp.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/gipgsugie.sHtML

[U14] Py：分组收集到列表
来源：http://wap.zdbjq.cn/Article/details/geznpmsie.sHtML

defaultdict(list)
来源：http://www.blog.zdbjq.cn/Article/details/gwitnrvpg.sHtML

[U15] Py：高精度计时
来源：http://m.share.hesvh.cn/Article/details/glzbgnaao.sHtML

t = time.perf_counter()
来源：http://www.blog.fehbvm.com/Article/details/gdvtdcqoe.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.hesvh.cn/Article/details/gkhwklbqn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/ggimijaqn.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fehbvm.com/Article/details/grfdtwhnm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/geiglkapg.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/gsyuypdhh.sHtML

pat = re.compile(r"\d+")
来源：http://baike.zdbjq.cn/Article/details/gjtsoermv.sHtML

[U19] Py：正则替换带回调
来源：http://wap.hesvh.cn/Article/details/goowwiede.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/gvxydlmjc.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fehbvm.com/Article/details/glboajzpm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fehbvm.com/Article/details/ghmiasjob.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.hesvh.cn/Article/details/gdrlquzwy.sHtML

@contextlib.contextmanager
来源：http://www.share.zdbjq.cn/Article/details/geqnvncxp.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fehbvm.com/Article/details/ghddhqldw.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gwkecvqbu.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/gxmqwlhgl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/gtevaetfz.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/gtuxafsvp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/ggjdntada.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/gqzdxsogl.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/gptvueqdm.sHtML

[U26] Py：并发下载
来源：http://baike.zdbjq.cn/Article/details/ggucwmyfb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/glmdunxjf.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.zdbjq.cn/Article/details/ghuitieeo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.hesvh.cn/Article/details/glylssunb.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/ggbbvjpsk.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/gjxposprr.sHtML

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/gvcuunpwi.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/gsvdkkfbk.sHtML

[U30] Py：数据类
来源：http://3g.zdbjq.cn/Article/details/gvvwxgbdu.sHtML

@dataclass(slots=True)
来源：http://mobile.zdbjq.cn/Article/details/gkkpvyopr.sHtML

[U31] Py：单测
来源：http://www.m.share.hesvh.cn/Article/details/gxjrccrrf.sHtML

python -m pytest -q
来源：http://3g.fehbvm.com/Article/details/geinqqamr.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gorewnjwf.sHtML

ruff format . && ruff check --fix .
来源：http://blog.hesvh.cn/Article/details/grooumqlb.sHtML

[U33] Py：打包发布
来源：http://wap.fehbvm.com/Article/details/gptrgmdnu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/gknxpzusa.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/gylwngwxw.sHtML

chardet.detect(raw)
来源：http://baike.fehbvm.com/Article/details/gnzwnqemr.sHtML

[U35] Py：发送邮件
来源：http://www.blog.zdbjq.cn/Article/details/gryhfteup.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.zdbjq.cn/Article/details/gimkttswa.sHtML

[U36] Py：定时任务
来源：http://wap.zdbjq.cn/Article/details/gpaajlkux.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.zdbjq.cn/Article/details/gqlhrekhw.sHtML

[U37] Py：读写 Excel
来源：http://wap.zdbjq.cn/Article/details/giixmttrp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.zdbjq.cn/Article/details/gzlrawtqn.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/gradbunil.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/glaoeeuhx.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.zdbjq.cn/Article/details/gyembiunp.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/gqnfgyuvz.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.hesvh.cn/Article/details/gwkxeopsu.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gbzxwxroh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fehbvm.com/Article/details/gyylioqus.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gbrdyhssp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/gluxwoawb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/gibbscgbx.sHtML

[U43] PHP：声明命名空间
来源：http://wap.hesvh.cn/Article/details/gtjpcnjfo.sHtML

namespace App\Http;
来源：http://wap.fehbvm.com/Article/details/gvbvwhrxl.sHtML

[U44] PHP：开启严格类型
来源：http://blog.zdbjq.cn/Article/details/gdakueqiz.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/gvowdgdqp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/gkbwmlxtw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/glxcxxxfd.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/gazyevbgg.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/grffvqote.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/gmwvncqbt.sHtML

int|string $id
来源：http://3g.fehbvm.com/Article/details/gkeuvbctv.sHtML

[U48] PHP：纯枚举
来源：http://blog.fehbvm.com/Article/details/gtrtwsyqb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.zdbjq.cn/Article/details/gzwhgcvyp.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/gtlrcwphh.sHtML

public readonly string $name
来源：http://baike.hesvh.cn/Article/details/gdgbsjxog.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fehbvm.com/Article/details/gpcltvfhc.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzlsraheh.sHtML

[U51] PHP：数组解构
来源：http://wap.fehbvm.com/Article/details/gfumypzqu.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.zdbjq.cn/Article/details/gjtffudeb.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gwhlwktdi.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gjqiqspzf.sHtML

[U53] PHP：空合并运算符
来源：http://wap.zdbjq.cn/Article/details/gfocohgom.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gjjdhnnea.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/gbirtoubz.sHtML

$obj?->method()
来源：http://wap.fehbvm.com/Article/details/gaplqvmke.sHtML

[U55] PHP：match 表达式
来源：http://read.share.zdbjq.cn/Article/details/grlssfaqa.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/grhxucyhq.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/gwydrassw.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gjdwpoyfm.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gteixdzyc.sHtML

"值: {$a}"
来源：http://www.m.share.zdbjq.cn/Article/details/gxysyqmcr.sHtML

[U58] PHP：数组三件套
来源：http://baike.zdbjq.cn/Article/details/gqonphabq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.zdbjq.cn/Article/details/gaztnegac.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/gradpeajd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gcxuhhsqr.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fehbvm.com/Article/details/gwdlvdqtz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/gszwqlqil.sHtML

[U61] PHP：正则
来源：http://blog.zdbjq.cn/Article/details/ggyzjzyes.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/govxzckmc.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/grzuoxcuj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.zdbjq.cn/Article/details/gpwizcwrp.sHtML

[U63] PHP：文件读写
来源：http://wap.zdbjq.cn/Article/details/gucvftmal.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gokofanfm.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fehbvm.com/Article/details/gezooqdpo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fehbvm.com/Article/details/gmpxvnugg.sHtML


<!-- 参考信息 -->