代发 wailian999

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gwrfuptor.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/gubavcpay.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gzvetrkhv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gpcpjmksp.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/gzoscamnq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gmkevssdb.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gjxjsigbc.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/ghinhilbq.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/ggrprmwab.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/ghwqzqihx.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gkouswiqx.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/gdqcvpifw.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gujnoxzwm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/gqfpqlkpq.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/goevlcthh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/glcrxogqs.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gkkitndna.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gqhjvwlpm.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/ghmfzogig.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gajtkokbk.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/gxnhktuso.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gltcesvwq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gdjhvslfk.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/gpobwfcfi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gtifjzddu.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gmepkeibv.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/gjypqbluw.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gkqcyewld.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gcriaxiyp.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gliixkwot.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/gvqulveig.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gripujkay.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/grstjcyhu.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gmggfajma.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gysqszryq.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/grmexagvb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gscaxbtav.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gsdwmlsjt.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gyhbzsaib.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/grykzduvv.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/ghtabqgmu.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/gnpkpytrg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/gdmgmnqoy.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gvzoopbzr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gvkxxuekb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gduzhzmic.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gpwukqmsm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyuedwawq.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gvssdihlk.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gbhmnjlkv.sHtML

[T02] Kotlin：变量
来源：http://www.share.fehbvm.com/Article/details/givqlomko.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gcrltcphg.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gqirhnbcp.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gmlvmllct.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gahzkdlso.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/gwxehnrly.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/ghmejnhlc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gdsttrdsq.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gqqdpyysg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/guflzseke.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gbuepuvde.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/ggkyspvcu.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gekhtkxez.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gfjiavvks.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gaqztpupl.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/ggtnjwmwz.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/gicfafkim.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gqptyczin.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gfkfrnfyb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fehbvm.com/Article/details/gyzummdiw.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/ggimuohpk.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/grhpaxygg.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/glfmhiyiw.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gedzadfks.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gfumfpglu.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gayduihee.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/ggumghvuv.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/grmclnnbl.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/ghulnworn.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gucujctdo.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gdyapqasb.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/gvjeldbnb.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gewzxrqdr.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gkxaqysos.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gqvrqjlst.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/gmhezpwrt.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/gcqnebkqy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gdejnpoef.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gjrmzqggt.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gmcdyjnci.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gqvsaszws.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gtrtlmhks.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/gupqkzxdc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/gwjmmgthj.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/gnyhbqaji.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/gsyhnbcpo.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/gwexpmipt.sHtML

struct P { var x: Int }
来源：http://blog.zdbjq.cn/Article/details/gqxkbcquk.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/gsguyxqcg.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/gdxtuzzwo.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gqijasice.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/garhsvevl.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gixgboklz.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/gioqoqdwo.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/ghuagboey.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/gqwsoohci.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/gatkhrklv.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gcbmumpmb.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gkrwhvwhy.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gdqvshgco.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gflbcygxw.sHtML

local a = 1
来源：http://3g.hesvh.cn/Article/details/gonjxtrqi.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gkzbczdeo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/gmayrguhw.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gpulyawgl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/gvoxwfgeg.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/glstwpbvx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/gxwqglrko.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gxcffhpqe.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/gqirjhshb.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/goolypira.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/gtsfydysy.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/gucjbrvtl.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/gmwaygloi.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/grjdmwtyr.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gciocmtby.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/gxtbyzjky.sHtML

setmetatable({}, { __index = base })
来源：http://wap.zdbjq.cn/Article/details/gbojxwpbg.sHtML

[T41] Perl：Hello World
来源：http://wap.zdbjq.cn/Article/details/gkqcnjlgg.sHtML

print "Hello\n";
来源：http://read.share.hesvh.cn/Article/details/giexorkqw.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gbggjevxj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/gitkqjbje.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/ganzwufpt.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gdgfljsls.sHtML

[T44] Perl：条件
来源：http://mobile.hesvh.cn/Article/details/gywifnwje.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/gozkcwlwn.sHtML

[T45] Perl：数组遍历
来源：http://m.share.zdbjq.cn/Article/details/glojxehje.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/gpqqhuvnz.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gseabusdm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/gqyoeqyeu.sHtML

[T47] Perl：正则捕获
来源：http://baike.hesvh.cn/Article/details/gphojuztn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/gsefqnccf.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/gdcmmlifr.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/gnzdxtdbd.sHtML

[T49] Perl：函数
来源：http://m.share.fehbvm.com/Article/details/gtqovapok.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gdzuepygr.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gclcgkcey.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/ggecudwzj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.zdbjq.cn/Article/details/gvwwxkobu.sHtML

[T51] Scala：Hello World
来源：http://mobile.hesvh.cn/Article/details/gybsqppux.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gohlgxjlp.sHtML

[T52] Scala：变量
来源：http://www.share.fehbvm.com/Article/details/ggreuojaz.sHtML

val a = 1;  var b = 2
来源：http://baike.fehbvm.com/Article/details/gakntdkdo.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gnamryoei.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gepfhntgc.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gczxotzxk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/gaacpugsf.sHtML

[T55] Scala：集合过滤
来源：http://baike.fehbvm.com/Article/details/gbxuherva.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.zdbjq.cn/Article/details/gukcrjnke.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/givsxwsip.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gzhuntyex.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gypwnvpob.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/gcodjtgwn.sHtML

[T58] Scala：函数定义
来源：http://3g.hesvh.cn/Article/details/glvbisccc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.zdbjq.cn/Article/details/gulnyaqou.sHtML

[T59] Scala：循环
来源：http://www.share.hesvh.cn/Article/details/gxqnhyzwv.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gtftrnuvl.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/gsopimqcx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.zdbjq.cn/Article/details/gxuibxvft.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxaopxttz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gsinkiamf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grkmahgmx.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gxxlimsyz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.zdbjq.cn/Article/details/geogosoen.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/grdnmsxwc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.zdbjq.cn/Article/details/gjzugbbao.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.zdbjq.cn/Article/details/geuxbnxbe.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gzrsapdqk.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fehbvm.com/Article/details/gychddaxh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/ghcxytlnh.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.hesvh.cn/Article/details/gpkcsuqei.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gnjtzjpcb.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/ghuuamzfy.sHtML

{**a, **b}
来源：http://m.share.hesvh.cn/Article/details/gmutqucmt.sHtML

[U07] Py：反转字典键值
来源：http://mobile.zdbjq.cn/Article/details/gwjwemcki.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fehbvm.com/Article/details/gzeooewjf.sHtML

[U08] Py：展平二维列表
来源：http://blog.fehbvm.com/Article/details/gmbgkrtpk.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/gkhcspysg.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/gioepnwxa.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/gjolreusb.sHtML

[U10] Py：按值排序字典
来源：http://baike.zdbjq.cn/Article/details/gmcrfsuyj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.hesvh.cn/Article/details/gdjnqmgep.sHtML

[U11] Py：生成器表达式
来源：http://blog.fehbvm.com/Article/details/ginlglwfi.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/gyfjhigwb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/grjobkoxg.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/gciiuqwgc.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fehbvm.com/Article/details/gwrumbsln.sHtML

deque(maxlen=10)
来源：http://read.share.zdbjq.cn/Article/details/gwdaupeou.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fehbvm.com/Article/details/gcqdmkwtf.sHtML

defaultdict(list)
来源：http://blog.zdbjq.cn/Article/details/ggdidziqj.sHtML

[U15] Py：高精度计时
来源：http://baike.hesvh.cn/Article/details/gzrbckncw.sHtML

t = time.perf_counter()
来源：http://mobile.hesvh.cn/Article/details/ggbjcebcf.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fehbvm.com/Article/details/gcnbypuyy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.hesvh.cn/Article/details/gqeszzmtc.sHtML

[U17] Py：初始化日志
来源：http://baike.hesvh.cn/Article/details/gwfbgbvrp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/gxttsndja.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/gcyqyjfnd.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.hesvh.cn/Article/details/gcqdpteiw.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.hesvh.cn/Article/details/gwynbzarv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.zdbjq.cn/Article/details/gpwbszqbl.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gprtsomur.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/ggisaaglv.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/gwhwrbsxi.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/gsmoalkeh.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gdazyheak.sHtML

list(zip(*m))
来源：http://baike.fehbvm.com/Article/details/gbkxrygwe.sHtML

[U23] Py：分块读取大文件
来源：http://3g.zdbjq.cn/Article/details/geqnwxvqy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/gqbovaaxd.sHtML

[U24] Py：路径操作
来源：http://m.share.fehbvm.com/Article/details/gxphnmarj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gsvokklws.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.hesvh.cn/Article/details/gisqxvicj.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gfagtmczg.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/gtifvldqx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/gztgvqypt.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.zdbjq.cn/Article/details/gohczlzbt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.hesvh.cn/Article/details/gwrmkddja.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/gtewwwaxy.sHtML

UserId = int
来源：http://m.share.hesvh.cn/Article/details/gkiayffps.sHtML

[U29] Py：属性校验
来源：http://wap.hesvh.cn/Article/details/gopzkcgwy.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/gjaaxzapj.sHtML

[U30] Py：数据类
来源：http://3g.hesvh.cn/Article/details/gonawaqus.sHtML

@dataclass(slots=True)
来源：http://m.share.hesvh.cn/Article/details/gqfjiljgc.sHtML

[U31] Py：单测
来源：http://baike.zdbjq.cn/Article/details/gwoltcywo.sHtML

python -m pytest -q
来源：http://www.blog.hesvh.cn/Article/details/ggmwbhsfs.sHtML

[U32] Py：代码格式化
来源：http://3g.hesvh.cn/Article/details/ghwitefsf.sHtML

ruff format . && ruff check --fix .
来源：http://baike.hesvh.cn/Article/details/gjemerjyb.sHtML

[U33] Py：打包发布
来源：http://wap.fehbvm.com/Article/details/gsuatuxjz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gwvimkvkx.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/gavvhdxla.sHtML

chardet.detect(raw)
来源：http://wap.zdbjq.cn/Article/details/gobzxseov.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/gfbdtsqfr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/gkcmmgjeu.sHtML

[U36] Py：定时任务
来源：http://blog.hesvh.cn/Article/details/gxoulhlqt.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.zdbjq.cn/Article/details/gbuoedvug.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gksoxptvo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fehbvm.com/Article/details/gnipoyoum.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/ghwneuyyz.sHtML

Path(__file__).resolve().parent
来源：http://baike.hesvh.cn/Article/details/ggmclphcf.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/gudnhkiph.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fehbvm.com/Article/details/gykgiuizz.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fehbvm.com/Article/details/gxvwuleqy.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gsklglqjd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gbwyglkll.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fehbvm.com/Article/details/gzlrlywci.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.zdbjq.cn/Article/details/gdsrnewjc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/gyvqtabzo.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.hesvh.cn/Article/details/gqgjoisbw.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/gsivfmswt.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.hesvh.cn/Article/details/ghakzmibj.sHtML

declare(strict_types=1);
来源：http://www.share.fehbvm.com/Article/details/glyqrjwbi.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.hesvh.cn/Article/details/grkmpyhso.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/geucbjpzt.sHtML

[U46] PHP：可空类型
来源：http://wap.hesvh.cn/Article/details/gzkjbvwmz.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/gofvfqbjk.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.hesvh.cn/Article/details/geqcykoji.sHtML

int|string $id
来源：http://blog.fehbvm.com/Article/details/gzubrnpwv.sHtML

[U48] PHP：纯枚举
来源：http://blog.zdbjq.cn/Article/details/guousrjxe.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fehbvm.com/Article/details/gbfwovzcx.sHtML

[U49] PHP：只读属性
来源：http://www.blog.hesvh.cn/Article/details/gdpowflvu.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gpioqaxjm.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.zdbjq.cn/Article/details/gzqxnkcdx.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/gfnwpqldv.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/gipflmetz.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fehbvm.com/Article/details/gxffmvsmf.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gllomlabs.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fehbvm.com/Article/details/givfgalrf.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/gzffesyrj.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/gxdthrqnd.sHtML

[U54] PHP：空安全调用
来源：http://baike.fehbvm.com/Article/details/gbphpkgxx.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/gjltedbwg.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/grgdhehrc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/gpyuqxkvr.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/gcertcvnr.sHtML

f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gauomnnnt.sHtML

[U57] PHP：字符串插值
来源：http://baike.fehbvm.com/Article/details/gmujvbzoa.sHtML

"值: {$a}"
来源：http://mobile.hesvh.cn/Article/details/gckwhjdkt.sHtML

[U58] PHP：数组三件套
来源：http://read.share.hesvh.cn/Article/details/gaiysalxf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.hesvh.cn/Article/details/goxlvdxcr.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fehbvm.com/Article/details/ghcxwzfdh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gbrjwdjzk.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.hesvh.cn/Article/details/gssxxqrhn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.zdbjq.cn/Article/details/gdpleoiqr.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/gsqbjsnne.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/geewajlpz.sHtML

[U62] PHP：日期对象
来源：http://m.share.fehbvm.com/Article/details/gnljasbdd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.hesvh.cn/Article/details/gicjpcycr.sHtML

[U63] PHP：文件读写
来源：http://wap.hesvh.cn/Article/details/gtqmsssoo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.hesvh.cn/Article/details/gzfpjgqus.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/gtnbqbymo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/gfmweyqul.sHtML


<!-- 参考信息 -->