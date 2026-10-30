代发 wailian999

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gfpppfykt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gabwodxgs.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gmvakytyn.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gtqtbsgxf.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/gmbmyjqzy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gxfptjdxx.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/grnbsuhdt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/ggxgtxfvi.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gussyyukh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gtabkqypb.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/gucmowfnd.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/givndyyso.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/giqlqccgb.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gcinxlmom.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gbnvrlrsb.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gxdakfsmg.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gcfkzimsc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/giujjmohn.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gedvwidqa.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gzgygudxd.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gyjywefqi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/gkwbxevxd.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gmtphnenv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gpzmekaoa.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gqecyolad.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gqxkjqlwy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gyghlkpba.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gymppdsgv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gejykndcl.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gpzsryqfu.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/gbmjkjvga.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/gsapvltyw.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gmzlfdfjj.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gomevdcnf.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gdyusmlqh.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gnoicfebz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gjusjrkco.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/gehovwkuq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/gajwcided.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/gbdwjtdbz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gwqykxkfk.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/gvlihqsxw.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gxzzvfppd.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/gftauhrde.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gfkwwqref.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gjyjgxkdc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/gdhiyufdw.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gjzxzxqev.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gikwvslgp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghwzyimdz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gmkesfznm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbeurtcwj.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gsnoqnflg.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gfaynlxtt.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/gzkrkglot.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/ggvhlqvit.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gvbyqubpk.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gztbbklwa.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gkjonebyc.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/ggmlvsmyz.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gcawamiwb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gupvfbnfp.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gycmtcsde.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gjefsiarf.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gqouqnmuh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gsugejscp.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gjcldmoyc.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/ggmlmcyot.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/gjwfomgxy.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gfxflxvsq.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gsbxpdtwk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gjjbzcmoc.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/gsbkmyoic.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gosavshdg.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gyyvorpnv.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gwxovirpw.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/gcvpsmtbh.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/gikqthmyb.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/gykrwqgko.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gmuustgqi.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gdwrtyffc.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gvqbmwloe.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/grddrvnod.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gvcjxevpu.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/ghzrptkmo.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gtaiwiuvs.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gdqqrnpjm.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/goidrcldp.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gsmxicogn.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/gybwqqniy.sHtML

[T20] Swift：数组操作
来源：http://www.blog.hesvh.cn/Article/details/gxnkjxurh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/gjfmlmywf.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/gbfrpppnq.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gmkiinjrs.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gactuvqzz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.hesvh.cn/Article/details/gtkduvvlp.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/gxiupabrl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/gxvnxgzgt.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/gdhyykzlh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/giwfhqupr.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/giuppwibv.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gwcvwqbwz.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/glrcubenu.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gwchtflcw.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/gipiyyiaq.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/gjqiqrxaw.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/geoqlphpo.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/goqenyvqv.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gfojrjaaw.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/ghmkfacoo.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/gauckbmxp.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/gswmqzmnp.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/ghvvwhlhj.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gttmwlsov.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gcwyoscjj.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gxegampqc.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/ghdumtnsv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/gytpllqyh.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/gzzqbnhok.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/govyqwpqj.sHtML

[T35] Lua：字典表
来源：http://blog.fehbvm.com/Article/details/giopaqxwx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/gezrudhkm.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/gftrpydzf.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/grjuplcti.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/gefhodnhs.sHtML

"a" .. "b"
来源：http://m.share.hesvh.cn/Article/details/geologefc.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/gbpjwklie.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/gilfreala.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/guxyqisse.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gevcckrak.sHtML

[T40] Lua：元表
来源：http://blog.fehbvm.com/Article/details/gvyxaitlp.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/ghsapkmpg.sHtML

[T41] Perl：Hello World
来源：http://3g.zdbjq.cn/Article/details/gkmvuspzy.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/gpkfjctsl.sHtML

[T42] Perl：变量类型
来源：http://read.share.zdbjq.cn/Article/details/glznwchxv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/gyzxisdxh.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gsygvhupb.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/gaoxboeuo.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gasryzuua.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fehbvm.com/Article/details/gsbeekjjg.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gyrawivez.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gpdccfble.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/gsggzcwkj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/gcyqmrtuq.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gbarzpjfz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/gvxsmcpqy.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/gabdjakkk.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/gdibhzcvq.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/goppjhjzp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gqswahize.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gwxgxeeik.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.hesvh.cn/Article/details/genmkpsav.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fehbvm.com/Article/details/gnxfrmkkr.sHtML

[T51] Scala：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gnecovfno.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gajczdfdn.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gscynchqe.sHtML

val a = 1;  var b = 2
来源：http://wap.fehbvm.com/Article/details/gasndzbmt.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gvnxeeije.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gawxnfaio.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/gicktghqy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/gwbddphhl.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gkkpinphs.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/gffrqrwlp.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/gpqwilhol.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/guvyyowbz.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/gtpeewyok.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/gdquaduhy.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/grxyjtlwq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fehbvm.com/Article/details/gfhnkiqis.sHtML

[T59] Scala：循环
来源：http://www.blog.fehbvm.com/Article/details/gtllznpae.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gznomndle.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/gaxwrraud.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/gccgkvpaf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsvvrkswu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/gerwbqbpm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvllfaqky.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gioznwkly.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/ggzezzkmc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gtljkkpqt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gisggxubp.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/glxacopph.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/grtcvzfiy.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/gzxzzsvhq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.zdbjq.cn/Article/details/gkxqcdqtf.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/grdzfrkff.sHtML

list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/guefpngrq.sHtML

[U06] Py：合并两个字典
来源：http://baike.hesvh.cn/Article/details/gvzrgtyjn.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/gxsdzobjn.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/gwubfzjtd.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.zdbjq.cn/Article/details/gnqytexji.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/gbfloygaj.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/gcghwnmpc.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.zdbjq.cn/Article/details/gbffkhljw.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gihryujef.sHtML

[U10] Py：按值排序字典
来源：http://wap.fehbvm.com/Article/details/ggsgvjsir.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/govxzxlst.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/gegslbfsi.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/giciivlvo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.hesvh.cn/Article/details/ghueylvxu.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/gzjzfouzl.sHtML

[U13] Py：固定长度队列
来源：http://baike.hesvh.cn/Article/details/gwelmahbf.sHtML

deque(maxlen=10)
来源：http://www.m.share.zdbjq.cn/Article/details/gvydmlqbn.sHtML

[U14] Py：分组收集到列表
来源：http://baike.zdbjq.cn/Article/details/guysirley.sHtML

defaultdict(list)
来源：http://www.blog.hesvh.cn/Article/details/gntpcuvfr.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gahqnufeo.sHtML

t = time.perf_counter()
来源：http://3g.zdbjq.cn/Article/details/gycemvsdr.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fehbvm.com/Article/details/geqxfcdaq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.zdbjq.cn/Article/details/gkvyqhcxc.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/gdiaehjty.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gpncebbhm.sHtML

[U18] Py：预编译正则
来源：http://3g.hesvh.cn/Article/details/gtbkbaudq.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/gjjxjwhoq.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/ggmxyvvpw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/gjwqyxjcj.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fehbvm.com/Article/details/gilhesaue.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/grsqhgzae.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/gvzqechpo.sHtML

@contextlib.contextmanager
来源：http://3g.zdbjq.cn/Article/details/gevbggigi.sHtML

[U22] Py：矩阵转置
来源：http://wap.zdbjq.cn/Article/details/gvvjjggok.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/gnwieioea.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/gtpnckqht.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/gfciysvoz.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/gdjgxaqjx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gjitehunm.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gegtjdamq.sHtML

csv.DictReader(f)
来源：http://www.share.hesvh.cn/Article/details/gcdughqbj.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fehbvm.com/Article/details/gdjdrgbbh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.zdbjq.cn/Article/details/gozpunnao.sHtML

[U27] Py：异步 HTTP
来源：http://3g.hesvh.cn/Article/details/gbpihjzae.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/gqyxbtlyo.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/gxddbzpjx.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/ggzhghxnv.sHtML

[U29] Py：属性校验
来源：http://baike.fehbvm.com/Article/details/gwmyzivkv.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/gwkynkakl.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/grtbzeznq.sHtML

@dataclass(slots=True)
来源：http://wap.zdbjq.cn/Article/details/gshfegsll.sHtML

[U31] Py：单测
来源：http://mobile.hesvh.cn/Article/details/ghlbjqdon.sHtML

python -m pytest -q
来源：http://www.m.share.zdbjq.cn/Article/details/gvihokmns.sHtML

[U32] Py：代码格式化
来源：http://www.share.hesvh.cn/Article/details/ghqwvacpw.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/gsvhhiizc.sHtML

[U33] Py：打包发布
来源：http://www.blog.hesvh.cn/Article/details/gwcjfaxhu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fehbvm.com/Article/details/gqfxnjrgu.sHtML

[U34] Py：判断编码
来源：http://wap.zdbjq.cn/Article/details/gpcsvmrlb.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/gtdiezvih.sHtML

[U35] Py：发送邮件
来源：http://baike.zdbjq.cn/Article/details/getrsveup.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/giriuhvyb.sHtML

[U36] Py：定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gfhijipbe.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/ghcvwtszy.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/gepinkcno.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.hesvh.cn/Article/details/gameolrwj.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.hesvh.cn/Article/details/gufjlfwwf.sHtML

Path(__file__).resolve().parent
来源：http://3g.zdbjq.cn/Article/details/gzevsewzu.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fehbvm.com/Article/details/gunfyyekb.sHtML

sys.stdout.isatty()
来源：http://www.share.zdbjq.cn/Article/details/gigedeicz.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.zdbjq.cn/Article/details/gccquwnrj.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gtwzbfrub.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.zdbjq.cn/Article/details/guwuqildh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fehbvm.com/Article/details/gmzdhfbrv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.hesvh.cn/Article/details/gtulwhydd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/gymfilvro.sHtML

[U43] PHP：声明命名空间
来源：http://3g.zdbjq.cn/Article/details/godoppmtu.sHtML

namespace App\Http;
来源：http://www.blog.hesvh.cn/Article/details/guqfrpywd.sHtML

[U44] PHP：开启严格类型
来源：http://blog.zdbjq.cn/Article/details/gqqqplmkf.sHtML

declare(strict_types=1);
来源：http://3g.fehbvm.com/Article/details/gdnuxslae.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fehbvm.com/Article/details/grinedsab.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/giemgfehb.sHtML

[U46] PHP：可空类型
来源：http://www.share.hesvh.cn/Article/details/gtwujqobc.sHtML

?string $name = null
来源：http://wap.fehbvm.com/Article/details/gnynuncor.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.hesvh.cn/Article/details/ggpcypsgj.sHtML

int|string $id
来源：http://baike.zdbjq.cn/Article/details/gdwntfpau.sHtML

[U48] PHP：纯枚举
来源：http://baike.hesvh.cn/Article/details/grzkkeqry.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.hesvh.cn/Article/details/gwznyeaxz.sHtML

[U49] PHP：只读属性
来源：http://m.share.hesvh.cn/Article/details/ghnpytozf.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/ggswjsonj.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fehbvm.com/Article/details/gxwaomnis.sHtML

public function __construct(private int $id) {}
来源：http://wap.hesvh.cn/Article/details/gliqcoxyh.sHtML

[U51] PHP：数组解构
来源：http://www.share.zdbjq.cn/Article/details/gnskwcaqi.sHtML

[$a, $b] = $arr;
来源：http://blog.hesvh.cn/Article/details/ghabxjgak.sHtML

[U52] PHP：箭头函数
来源：http://3g.hesvh.cn/Article/details/gzyqojuld.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fehbvm.com/Article/details/gttodxsmz.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fehbvm.com/Article/details/gounubpta.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fehbvm.com/Article/details/ghwekhtyr.sHtML

[U54] PHP：空安全调用
来源：http://blog.hesvh.cn/Article/details/gsqjoavtz.sHtML

$obj?->method()
来源：http://www.share.hesvh.cn/Article/details/gcjxjgkjk.sHtML

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/geplqrrns.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fehbvm.com/Article/details/goxydovzc.sHtML

[U56] PHP：命名参数
来源：http://baike.hesvh.cn/Article/details/ghxqghgwp.sHtML

f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/glzrznsma.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/gcvtbswid.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/gycjfpdbm.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gntncwceu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.zdbjq.cn/Article/details/ghiowmsjz.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.hesvh.cn/Article/details/gxyvgbghv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gkjlijpuj.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/gmpviodpl.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.hesvh.cn/Article/details/gxgjynyqs.sHtML

[U61] PHP：正则
来源：http://blog.zdbjq.cn/Article/details/girbqiajt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gxrzptcbn.sHtML

[U62] PHP：日期对象
来源：http://3g.hesvh.cn/Article/details/gciuidksr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/gtzxnrwbg.sHtML


<!-- 参考信息 -->