代发 wailian999

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/gvuoqcaja.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/gmupjbrex.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gdxcmbvyd.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/golqjswrx.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/gfllvuvcc.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/gbwfxbojw.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/gvqzfnyqf.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gbhjjmiho.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gzgxqcigl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gnmvzopgi.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gousrxtsl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/ghyyistvh.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/ggshjvcpc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/gmctonsmn.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gsoutrfnr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gpjvichpt.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gxxzzpfvt.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/guxfizwuk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/gzmduevzh.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gxitzrlco.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gonueynkk.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gvsnvmrhy.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/givbchkqc.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gflgssmyi.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gpopnkpmv.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gjulknpsf.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gslwwoujf.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/gestrmbtc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gvovahpdu.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/gzjqyumkg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gzkizrfon.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gxjqdwyfk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/ggkzedpwh.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gkcfwjpkg.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/glxctwiiv.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gbqjzjopb.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/giubcdlfx.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gvqizomgw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gyessdjkp.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gmwozmrfb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gpoosiqkp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwrumhfsj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gmmdytrsh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/glygcjktt.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gipwcbqwl.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gnlnwrlde.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/ggtfojdqk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gbecdcetl.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/gqrcijmjr.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gaodqtztg.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gctkitfah.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gvqgqzqsk.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gdriqdoav.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gxklqpews.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/gnrlzpkrt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gnmizfpqb.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/grpnosful.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/gtbfxelen.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gmjanmewr.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gttdqrwbx.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/guqbhscfo.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gsbyrdtfp.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gaomueiuh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gavjqfjzf.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/gbadhlcpi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gtyfqtgzm.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/ghlztcslx.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/goncqbour.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/gsxvutwcl.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/gzvgqkyex.sHtML

[T14] Kotlin：循环
来源：http://read.share.fehbvm.com/Article/details/gpzvvbjns.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gynumywbj.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/gjytntsib.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/giycyjpjp.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/gdmbmgbha.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/glcmncakk.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gqbjhtbln.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gosrhwdpo.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gjaqtsnad.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/gufjufwtl.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gyuadazau.sHtML

if let n = opt { print(n) }
来源：http://blog.fehbvm.com/Article/details/ghbpzpajt.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gefovrdgz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gnsgnoydt.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/gntuhnxfo.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/gipnrwpug.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/ggtkctkpp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/gatnlebpf.sHtML

[T23] Swift：函数
来源：http://m.share.fehbvm.com/Article/details/gfqyggtbp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/glphlnxzi.sHtML

[T24] Swift：闭包
来源：http://wap.hesvh.cn/Article/details/gtzdsbild.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gslvwiyts.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gywkchoqw.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gewbuvfzu.sHtML

[T26] Swift：类与重写
来源：http://baike.hesvh.cn/Article/details/gfeaewlsc.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/gylekwtrt.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/gyoxwbfkg.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/ggzvusbrs.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/gsarsziez.sHtML

enum Color { case red, green }
来源：http://m.share.zdbjq.cn/Article/details/gotvwosgh.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/gwknwjbzj.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/gkmuklnpa.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/gmzcjsfwd.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/gpuavaqlz.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gjgqzeseo.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gatfbdxac.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gwrkmxiae.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/ggcfnqfzi.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gqcroffkd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/gmkxawfqs.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/gibhfzxbv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/gidxsubxp.sHtML

[T35] Lua：字典表
来源：http://read.share.fehbvm.com/Article/details/guvwckyct.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gsgjuempu.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/gbftriicf.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/glxfihysl.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/gzziamgdi.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gxhdbvffy.sHtML

[T38] Lua：条件
来源：http://www.blog.zdbjq.cn/Article/details/gcizmwnhw.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/gsrqilqsb.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/gczcgrkwm.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gdlvcredc.sHtML

[T40] Lua：元表
来源：http://www.blog.fehbvm.com/Article/details/gyyxoohar.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/gsebadwvs.sHtML

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/ggprfobgp.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/gwigldtyz.sHtML

[T42] Perl：变量类型
来源：http://mobile.zdbjq.cn/Article/details/gihkpuaag.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/gbkqtjgpa.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gyzofdbno.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gerocbzes.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/gvqvphzfi.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gkdmcoccl.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/gdujqivmg.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.zdbjq.cn/Article/details/gmfjyltwt.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/gcdjdrugk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/gyxirclgx.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/gyfacjfkq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/gvtgyfdha.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gjuvwxgem.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/gwdarktgd.sHtML

[T49] Perl：函数
来源：http://www.share.fehbvm.com/Article/details/gtdjhbmar.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/geddezqhd.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gbhpprklm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/gudzjzljl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gdcgsqpru.sHtML

[T51] Scala：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gvbecgvnh.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gxsgxxqhx.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gcgkabwza.sHtML

val a = 1;  var b = 2
来源：http://www.share.fehbvm.com/Article/details/groshlsnx.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gowcawoxb.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/gpwjmhlzk.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gmbvjqmqw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/gvhbbmnto.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/gjkbjwjbz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gnpjvsvkp.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gleaxgiwd.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gkidfebhj.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/ghdrziajq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gmqbyigec.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/gpeqlvbnw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/ggkbikenz.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/gtckcpzhi.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.zdbjq.cn/Article/details/guntxdayc.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/gcedusvyx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.hesvh.cn/Article/details/gpaioyvle.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gacberazj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/gldynxmad.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfzfbxklz.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/gftsfgrbf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/graswmwfx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/gnyxrkdcx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/gifkorkab.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fehbvm.com/Article/details/gmuntwjut.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/giazfpiml.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gjidrpyyx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gnrupccdx.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gvsgeobuf.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gsoratcca.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/giljjjwbx.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/gpejmizpo.sHtML

[U07] Py：反转字典键值
来源：http://baike.zdbjq.cn/Article/details/gapdzqfws.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/gjqdlyltq.sHtML

[U08] Py：展平二维列表
来源：http://3g.zdbjq.cn/Article/details/gjcyogopn.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/gjiohfucd.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/guiswsppc.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gjgddgzig.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gxuybfsog.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/gsiwejazg.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/gogvwvtqy.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/gmnlzrnkr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gsbtfpoyy.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/gmaomfalj.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/gqfrsssoc.sHtML

deque(maxlen=10)
来源：http://baike.hesvh.cn/Article/details/gjedzkbrn.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/gfiaggamv.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/gwddfkfly.sHtML

[U15] Py：高精度计时
来源：http://read.share.zdbjq.cn/Article/details/gssvegmta.sHtML

t = time.perf_counter()
来源：http://3g.zdbjq.cn/Article/details/gzkmnzbpe.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/goieruiul.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fehbvm.com/Article/details/gbkkoshuk.sHtML

[U17] Py：初始化日志
来源：http://baike.zdbjq.cn/Article/details/gxzzpvpli.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gjbukixqp.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.zdbjq.cn/Article/details/gtmwsmcdd.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gxkvlisjn.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/gqwjugymf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/gzovriwuy.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fehbvm.com/Article/details/gdwinvzit.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/gggjykpwm.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fehbvm.com/Article/details/gdzpczzfp.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/gehefvgtm.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/gwrecaacf.sHtML

list(zip(*m))
来源：http://baike.fehbvm.com/Article/details/gxgvsooqu.sHtML

[U23] Py：分块读取大文件
来源：http://3g.hesvh.cn/Article/details/gbdsqualc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.zdbjq.cn/Article/details/ghhqbzkwr.sHtML

[U24] Py：路径操作
来源：http://read.share.hesvh.cn/Article/details/gigmzengj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/guhyvynaa.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fehbvm.com/Article/details/geffixrbm.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/gopzjosmc.sHtML

[U26] Py：并发下载
来源：http://read.share.hesvh.cn/Article/details/gbnubwmhj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.hesvh.cn/Article/details/gyltpjrdo.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.zdbjq.cn/Article/details/giotuumcf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.zdbjq.cn/Article/details/gmzgcdzrk.sHtML

[U28] Py：类型别名
来源：http://3g.zdbjq.cn/Article/details/gwfstnqud.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/ggkkuowkj.sHtML

[U29] Py：属性校验
来源：http://baike.fehbvm.com/Article/details/gqnvyvaln.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fehbvm.com/Article/details/gdadzgexz.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/gigtfxtmh.sHtML

@dataclass(slots=True)
来源：http://blog.zdbjq.cn/Article/details/gccbdafch.sHtML

[U31] Py：单测
来源：http://read.share.hesvh.cn/Article/details/gywowkpdz.sHtML

python -m pytest -q
来源：http://blog.zdbjq.cn/Article/details/gczbisbpo.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/giycvhiuf.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/gfgvkqrnh.sHtML

[U33] Py：打包发布
来源：http://www.blog.fehbvm.com/Article/details/gaeimhifx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.zdbjq.cn/Article/details/gmqtytdyl.sHtML

[U34] Py：判断编码
来源：http://baike.fehbvm.com/Article/details/gxgtmcjsv.sHtML

chardet.detect(raw)
来源：http://baike.fehbvm.com/Article/details/gdhfoznmd.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/gybwhazsr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fehbvm.com/Article/details/gdbflgtij.sHtML

[U36] Py：定时任务
来源：http://baike.zdbjq.cn/Article/details/glnsmhjpj.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.zdbjq.cn/Article/details/gurcqogph.sHtML

[U37] Py：读写 Excel
来源：http://m.share.hesvh.cn/Article/details/gwmlpncty.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/gtkgkhwsf.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.zdbjq.cn/Article/details/gwhswclws.sHtML

Path(__file__).resolve().parent
来源：http://www.share.zdbjq.cn/Article/details/gemeasjmk.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/gvyjwhtxj.sHtML

sys.stdout.isatty()
来源：http://www.blog.hesvh.cn/Article/details/gqzkqqyru.sHtML

[U40] Py：打印到标准错误
来源：http://baike.zdbjq.cn/Article/details/gyzsmahur.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gimvjrddb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fehbvm.com/Article/details/gmnelgimd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/gtxqhtvya.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fehbvm.com/Article/details/gdncqlhnm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/gxugfpzfj.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gmazidres.sHtML

namespace App\Http;
来源：http://baike.fehbvm.com/Article/details/gagjraoba.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/gnonpokku.sHtML

declare(strict_types=1);
来源：http://blog.hesvh.cn/Article/details/gpdbzcxpx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fehbvm.com/Article/details/gtgatzslg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/ghtjsnfnp.sHtML

[U46] PHP：可空类型
来源：http://mobile.zdbjq.cn/Article/details/gnhrghcbk.sHtML

?string $name = null
来源：http://www.m.share.hesvh.cn/Article/details/ggaenusmj.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/gydwmnfcl.sHtML

int|string $id
来源：http://www.share.zdbjq.cn/Article/details/gbevtplmt.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/gqhnyglqv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/gqjmqtyzw.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.hesvh.cn/Article/details/gcmqtakzz.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/gzcaarvme.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/gxujkppuj.sHtML

public function __construct(private int $id) {}
来源：http://www.share.zdbjq.cn/Article/details/gtfpwtspv.sHtML

[U51] PHP：数组解构
来源：http://read.share.fehbvm.com/Article/details/grpmkqlaq.sHtML

[$a, $b] = $arr;
来源：http://mobile.fehbvm.com/Article/details/gsddgazwy.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gpbslwrdm.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gvksqyesw.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.hesvh.cn/Article/details/gfcpgsquu.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fehbvm.com/Article/details/gikezzkhd.sHtML

[U54] PHP：空安全调用
来源：http://www.share.zdbjq.cn/Article/details/ghlpvxxnc.sHtML

$obj?->method()
来源：http://www.m.share.zdbjq.cn/Article/details/gsawnfiwm.sHtML

[U55] PHP：match 表达式
来源：http://wap.hesvh.cn/Article/details/gxxhszycn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/gorltwsjp.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.hesvh.cn/Article/details/gvjeocsjd.sHtML

f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gmbholxbf.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gmoqjchqt.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/gylrmffuv.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/gcwuipgxj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.zdbjq.cn/Article/details/gwnuhtulf.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fehbvm.com/Article/details/gtlsskzpx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gmezndxph.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fehbvm.com/Article/details/gbfruuali.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.zdbjq.cn/Article/details/geeiyisjl.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/gpekuxjrg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gablqrrai.sHtML

[U62] PHP：日期对象
来源：http://read.share.zdbjq.cn/Article/details/gwyydvfwy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/gnnwynmir.sHtML

[U63] PHP：文件读写
来源：http://baike.zdbjq.cn/Article/details/goijsxyuj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fehbvm.com/Article/details/gtdumpiky.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fehbvm.com/Article/details/gidpifpwe.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fehbvm.com/Article/details/galftvqwc.sHtML

[U65] PHP：会话
来源：http://blog.zdbjq.cn/Article/details/gbzgkhjfj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gtvrpqpin.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fehbvm.com/Article/details/gwcizcjna.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.hesvh.cn/Article/details/gtldzdsid.sHtML


<!-- 参考信息 -->