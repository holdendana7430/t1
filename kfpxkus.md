代发 wailian999

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gtlyvggyq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gocsqwqwc.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gbuwllint.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gxxepequf.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gzoyjlwzm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/giyyhbqdz.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/glnbhrpza.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gsqeeoojy.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gferjdral.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gsdybhdnz.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gcdnfuqpg.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/gbxdfsojy.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gcmdtrtmh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/gxabciuua.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/grqumhzzl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gfuvndtwd.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/guxfmwyjy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gsqqlpiki.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gdbnwutlc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gnszcosva.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/gfzvbyciy.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/grswfszfa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/gkslhwndf.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gyguothzc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gyjybawcr.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gmqfrcsus.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gksopwrkz.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/ghtwcxdqt.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gdzcyblbv.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/gkhdcqdkf.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/gcpcuznrm.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gokpvrjey.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gncqhudkm.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gvmaxbhfb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/gvdybemwj.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/gstirootr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/golrbfctn.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gjnmrbxvw.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/ghbsluflu.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gsbxopqmr.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fehbvm.com/Article/details/gknwilgmf.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gjeujmplb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/gcpysvdzw.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gvtgyqvux.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gvthzkmop.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gszlpdhnd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gbashiyhg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gazvstgzg.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/garxsqdoh.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/grpohabdy.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/ginbtflww.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gqzlnlxpi.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/goxhaaofl.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gugfqhdpy.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/glefvgxug.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/gfplttcgh.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gdhgddwzw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/gxjhsxbtp.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gqboaeolq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gyavuqbbj.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gifrcqkfq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gylrewhwt.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/gwrprvikz.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gdxqvmtye.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gypkdkrtf.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/gmqbzpduo.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/gfniijrui.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/geustwvhv.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gewsuoegh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/gjxlmghtv.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gjxgwbwsw.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gpojefyxq.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/gqnoivagq.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gucvbaixy.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gujzcxbcy.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gacgdivhx.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/ggbivjktf.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gvhljidah.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gbnbsctuj.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gyyqkzndi.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/gvmngjsab.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gvzewgphk.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gicbokhtr.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gvnbxonfn.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/gbqvxfhic.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/gfzgpghby.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/gnvqzwxcp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/gblshotpg.sHtML

[T21] Swift：遍历
来源：http://wap.hesvh.cn/Article/details/gwdyjhksl.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gesokxjmo.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/gkdnsylbf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gdjwhnzzs.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/gactfbnpi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.hesvh.cn/Article/details/gugzxzjku.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/gquzqhvwy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gjcpincer.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/gykbmtped.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gzzoykgzs.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/gxnbookux.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/gdfyyrktj.sHtML

[T27] Swift：错误处理
来源：http://baike.hesvh.cn/Article/details/gcwrxdceh.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/gpqflensq.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gmbppyfes.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gvqylfrfp.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gzgouwvee.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/gqvgorxmu.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gpcmsiouh.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/ghzmbhcea.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/gvvrivaxq.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gwnvqwunx.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/gcfhetwmn.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/grrbcqtps.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gvhxuabye.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.zdbjq.cn/Article/details/gbebvalvx.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/giieqfqji.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/grllwrecm.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/giowslhzr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/gjdiptpvd.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/gkwxmtvlb.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/gdgyfrmcq.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gyjsshejb.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gftuernsj.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/gwxcejryv.sHtML

if x > 0 then print("正") end
来源：http://mobile.hesvh.cn/Article/details/grjfcxmru.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/grsbtxcwa.sHtML

string.find(s, "%d+")
来源：http://wap.hesvh.cn/Article/details/gjmugwofb.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/gvayzjtlh.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.hesvh.cn/Article/details/gdxqiypbu.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/gjbsojpgh.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/gdxfrvtyo.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gqqxyldwo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/ggcxvzvul.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gzsjgidzx.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gvskwuaki.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/gzqakgnjk.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fehbvm.com/Article/details/gsysawdwc.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/gtygsfaqr.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/ghuhfhbio.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gieyabgyy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/gxvfbyefd.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/govfvfyqq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.zdbjq.cn/Article/details/gsvqzzpkk.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/ghbknmrwq.sHtML

$s =~ s/old/new/g;
来源：http://blog.fehbvm.com/Article/details/gwhnzzxbv.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/gotfxqqwv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/geyddmcai.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gswjqfeet.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fehbvm.com/Article/details/gsybkafye.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/grfzslrlm.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/gjytidfho.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gpkxhvxbn.sHtML

[T52] Scala：变量
来源：http://m.share.zdbjq.cn/Article/details/gwkztucxx.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gdzaqdnur.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gtanlcwqr.sHtML

s"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gxrklbqmn.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/ghjavlzif.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/gxpqggfgx.sHtML

[T55] Scala：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gslvrwper.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/gyzynafjq.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/gmxkkhfkz.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gteqlkmoh.sHtML

[T57] Scala：模式匹配
来源：http://3g.zdbjq.cn/Article/details/grxbthajx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.zdbjq.cn/Article/details/gjrwesrfr.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/gwsrapjut.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/gcmaxezhp.sHtML

[T59] Scala：循环
来源：http://baike.zdbjq.cn/Article/details/gwvizcdzb.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gggctckzt.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/gbffxzeqo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gfubjdzbw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gujtfhsoa.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gbzydcovs.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtazhhjxj.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/gsowytrbj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/gqiuzcfbx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/gvlcrwdii.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gszwnqjzy.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.zdbjq.cn/Article/details/gadxqxlkn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/gjqiufhrv.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/gyqucmkyo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gulplyood.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.hesvh.cn/Article/details/gwwlchezy.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gpfyxniwo.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gxgusdotd.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/gciojsnmr.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/gkanoxevz.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/gmehyqvwk.sHtML

[U08] Py：展平二维列表
来源：http://wap.zdbjq.cn/Article/details/gnjwuedxm.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/ghhfgnyqa.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.zdbjq.cn/Article/details/gumebteod.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/gidhdcdks.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.hesvh.cn/Article/details/gumbwixaj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/gqfqckunm.sHtML

[U11] Py：生成器表达式
来源：http://blog.zdbjq.cn/Article/details/grqipdior.sHtML

(x * 2 for x in arr)
来源：http://wap.fehbvm.com/Article/details/gzblxvctl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/glabcvzpm.sHtML

Counter(arr).most_common(3)
来源：http://mobile.hesvh.cn/Article/details/gzpkjwqbs.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/gbjqqcyza.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/gnpbgfsmg.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fehbvm.com/Article/details/gksxjwxjo.sHtML

defaultdict(list)
来源：http://www.blog.fehbvm.com/Article/details/gewambafw.sHtML

[U15] Py：高精度计时
来源：http://read.share.zdbjq.cn/Article/details/grvgnnxau.sHtML

t = time.perf_counter()
来源：http://3g.zdbjq.cn/Article/details/gltltkkuk.sHtML

[U16] Py：命令行参数解析
来源：http://baike.zdbjq.cn/Article/details/gijxbcwjv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/geukaxkbx.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/gxsollruy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/gthyvkwxq.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/gjczuhbuk.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gkmkrcxly.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/gwnrnuvbk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.hesvh.cn/Article/details/gnfrtrdir.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fehbvm.com/Article/details/gavhlcgvy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/gvapuivej.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gvwaybztx.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fehbvm.com/Article/details/gofzookue.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.hesvh.cn/Article/details/gnsfxxusf.sHtML

list(zip(*m))
来源：http://www.share.hesvh.cn/Article/details/gokptkcot.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/gikcqcxat.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fehbvm.com/Article/details/ggqjrfvna.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gpnbelrcr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gcncdpddh.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.zdbjq.cn/Article/details/gisimnicw.sHtML

csv.DictReader(f)
来源：http://blog.hesvh.cn/Article/details/gfbuwurhf.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/gzgvtegie.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/gqzwuqimq.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/gsrlcmzta.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/grpwjgdiv.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/gbskbnwzz.sHtML

UserId = int
来源：http://baike.hesvh.cn/Article/details/gjvaslyfl.sHtML

[U29] Py：属性校验
来源：http://read.share.hesvh.cn/Article/details/gdcvtpiac.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fehbvm.com/Article/details/grtsxnqgx.sHtML

[U30] Py：数据类
来源：http://read.share.zdbjq.cn/Article/details/ggtcphiou.sHtML

@dataclass(slots=True)
来源：http://www.share.hesvh.cn/Article/details/gsmponnjw.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/giuwijhzu.sHtML

python -m pytest -q
来源：http://baike.fehbvm.com/Article/details/gbgsjpmmu.sHtML

[U32] Py：代码格式化
来源：http://m.share.zdbjq.cn/Article/details/gdhheyijr.sHtML

ruff format . && ruff check --fix .
来源：http://baike.hesvh.cn/Article/details/gaxekabpw.sHtML

[U33] Py：打包发布
来源：http://read.share.zdbjq.cn/Article/details/giuvcbrsx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fehbvm.com/Article/details/geneivgpy.sHtML

[U34] Py：判断编码
来源：http://blog.fehbvm.com/Article/details/gfagtrldf.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/gndojfahi.sHtML

[U35] Py：发送邮件
来源：http://baike.fehbvm.com/Article/details/gshdghshs.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fehbvm.com/Article/details/gjvzjidfp.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/guxqwjlrf.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/gazhgmrgn.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fehbvm.com/Article/details/gkgahvtxi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fehbvm.com/Article/details/grlptvyjt.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gnbfbwbis.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gngqzyhul.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fehbvm.com/Article/details/gdqbexafx.sHtML

sys.stdout.isatty()
来源：http://3g.fehbvm.com/Article/details/gihrylapj.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.zdbjq.cn/Article/details/gutvcsviq.sHtML

print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gietduuyw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.hesvh.cn/Article/details/gshzsujgn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.hesvh.cn/Article/details/gjfcgbjln.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/gjdlazrjy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fehbvm.com/Article/details/gjdcoiedf.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.hesvh.cn/Article/details/gardawdjm.sHtML

namespace App\Http;
来源：http://www.m.share.zdbjq.cn/Article/details/grcopmpit.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fehbvm.com/Article/details/gyvwfhqsa.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/gdhqopszh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/girmytcrd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gyexusszv.sHtML

[U46] PHP：可空类型
来源：http://blog.fehbvm.com/Article/details/gfuotvxbx.sHtML

?string $name = null
来源：http://www.blog.hesvh.cn/Article/details/gdzdcsinj.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/gyuudfmeg.sHtML

int|string $id
来源：http://read.share.hesvh.cn/Article/details/gdjnfbdag.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/gitexuwob.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.hesvh.cn/Article/details/gokdxjlnr.sHtML

[U49] PHP：只读属性
来源：http://read.share.zdbjq.cn/Article/details/glwlejqoo.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gxhvunnro.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/gnlanyaqi.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/gdzdlvcva.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.hesvh.cn/Article/details/gfrkddohz.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/gtbibjlqv.sHtML

[U52] PHP：箭头函数
来源：http://blog.fehbvm.com/Article/details/gjqfriqve.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fehbvm.com/Article/details/gvzafdzdu.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/grvolvsmf.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.hesvh.cn/Article/details/gqzvrvrnu.sHtML

[U54] PHP：空安全调用
来源：http://read.share.hesvh.cn/Article/details/gyvyattkm.sHtML

$obj?->method()
来源：http://wap.fehbvm.com/Article/details/gvxzfijcr.sHtML

[U55] PHP：match 表达式
来源：http://baike.zdbjq.cn/Article/details/gfjkbsvgu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gxfcmjyhh.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/gyhgihuig.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gsyqkwesy.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/grmzceyje.sHtML

"值: {$a}"
来源：http://m.share.zdbjq.cn/Article/details/gerhivmyi.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fehbvm.com/Article/details/gmykelffo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.zdbjq.cn/Article/details/gqzxmoavh.sHtML

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/gbivvcics.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gpanntkns.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/grnfzubtd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/gfhrfavge.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/gtxduswbj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gogvkruxq.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.zdbjq.cn/Article/details/gckhwsddh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fehbvm.com/Article/details/gkdqckpoe.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/gmnsllsks.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.zdbjq.cn/Article/details/ghftebhvk.sHtML

[U64] PHP：目录遍历
来源：http://www.share.zdbjq.cn/Article/details/gbjmgpuqy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.hesvh.cn/Article/details/gpebbcyan.sHtML


<!-- 参考信息 -->