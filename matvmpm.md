代发 wailian999

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gjpyanogt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/goevwvjit.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gxxhwmurx.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gvgzdjhxo.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gmkvqvcxc.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/gfkeerufx.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/gtpephcap.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gtmqwjwzp.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/glemvyrlg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gljseazdk.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/ghetwukrx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gfqouzpkm.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/grlamznfg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gfxjwxmdm.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gfgbgxtlf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gulhnrfzm.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gkfrutivq.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/ghvfytfow.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/ggvhmlnri.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/gwpjamhhu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gfaqijxuo.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gomxktpsl.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gtcocabqn.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gxzmrntiu.sHtML

int size() const noexcept { return n_; }
来源：http://3g.hesvh.cn/Article/details/gkfrflofz.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gptaepvsi.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gzjkpszli.sHtML

[S54] C++：异常处理
来源：http://wap.hesvh.cn/Article/details/gnacrqzfc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/guzamyzix.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/gaxkfvmax.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gkadgralc.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gkorqqjfz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/gmigyyqez.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gmrzrubai.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gvagtnzvg.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/gehkvpmeq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/grwlbxfli.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gwqafbiau.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gzxfvhikq.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/gqxiqbere.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/gizieewmh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfeuyqanl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gayfmnlbs.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gowislhoo.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gsnhwrcby.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gaeybkotv.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gdpidnyzs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/gwbqogxkt.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gptspcicp.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gheswljcl.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gcepwmjfl.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/gygckjmzc.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/guisrxnqn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/grcapphwc.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gdahmluwf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gzrlrxxbr.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gaoyqvpvv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gudxpxkrl.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/ghihuipvt.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gbzcwtbiy.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gtkxennjz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/ghmntgcfm.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gvykkebrb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gavyuwyam.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gcnesohdp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gykgnerxn.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/ggynxywit.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gqtdvpxsy.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/ggexzorfj.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/gyahltnmr.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gkmxlqdcp.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gtzwpxvji.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/gqgyfdxjh.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/gylfonnwr.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/ghdiwmgiy.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gdwlafnqn.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gvavodvac.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/glfuigzsr.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gpguhquoo.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/gvptvhiua.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/gnsveldlb.sHtML

if let n = opt { print(n) }
来源：http://3g.fehbvm.com/Article/details/gtkllwkdz.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/ggutdnsmd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gkfxdvzyz.sHtML

[T21] Swift：遍历
来源：http://www.share.hesvh.cn/Article/details/guqfdqmbj.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/gzcitvcei.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/gpojdxqjo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.hesvh.cn/Article/details/govscotjf.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/gahhxmlzb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/glsdujwmx.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/gzkzteyob.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gjzdazxwz.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/glhqstoqc.sHtML

struct P { var x: Int }
来源：http://wap.fehbvm.com/Article/details/gjssgbjnm.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/gbgtmqleg.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/gpciyrmza.sHtML

[T27] Swift：错误处理
来源：http://m.share.zdbjq.cn/Article/details/grqjpmpml.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/glbgyquxf.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gsfcpfsdn.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gcokflguo.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/gatoucoqp.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gfadswpfh.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/gcdjfcqax.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/ggeefwwlv.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gmcxkuxxr.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gtsklihrs.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/ggtmlogka.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gwncntqft.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/ghoanntiq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/gybeggshc.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/gxtcwdgho.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/gzzjwovzz.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gisfbjzup.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gnyxvcaxr.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/gjcytcuwv.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/ghngustdx.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gxuotheni.sHtML

"a" .. "b"
来源：http://www.m.share.hesvh.cn/Article/details/gsccozqqo.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/ggdtyzhey.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gmcprbjxc.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gvgsoazsy.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gyhruvvlm.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/gnmbnupgg.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.hesvh.cn/Article/details/gtuvukwqq.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/gkthgltpt.sHtML

print "Hello\n";
来源：http://wap.zdbjq.cn/Article/details/gcenzmypa.sHtML

[T42] Perl：变量类型
来源：http://read.share.fehbvm.com/Article/details/gyklyihyc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/guzduwjli.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gndjypsxl.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/gzhbcxveo.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gbeogwhup.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/gvusfbedb.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.zdbjq.cn/Article/details/gbbzohicx.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/gmfanivht.sHtML

[T46] Perl：哈希操作
来源：http://read.share.zdbjq.cn/Article/details/gwfixdwgk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gnbfuvzna.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/gejajbmhh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/gpwvedcia.sHtML

[T48] Perl：正则替换
来源：http://wap.fehbvm.com/Article/details/ggtxvobzl.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/glztbtznv.sHtML

[T49] Perl：函数
来源：http://baike.fehbvm.com/Article/details/giyjvtyfm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gherufbvv.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gfqyquwzz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/glciesgih.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/garzjbhkv.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gtidxxaek.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gagzpolgz.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gcilvzvwq.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gtrijmayn.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/godxbiohu.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gfcskmiip.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/gxantbasx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/gziwnnmbc.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gztarutru.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fehbvm.com/Article/details/gzapkpphp.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/gtglzwpbl.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/gpegzxzrs.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/gxmzwrpdl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/gtedurphe.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/gvdsmoavt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.zdbjq.cn/Article/details/ghrdrxuhd.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/gjbesnxls.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/gbalmduvk.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/ghprrrwnv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fehbvm.com/Article/details/gicbmqxic.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmzujcbvn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gogthhpli.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdndrlhez.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.hesvh.cn/Article/details/ggkjcqpek.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/grzdhpjmp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/gschrlrox.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/gotywgstv.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/gwqsizzcv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/gyzcofobx.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gxjwvdozo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.zdbjq.cn/Article/details/gfigvtwpc.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/gronijwna.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/goekvcqrp.sHtML

[U06] Py：合并两个字典
来源：http://baike.zdbjq.cn/Article/details/gwyemdovo.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/gbwnobeme.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/gpbrcebhb.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fehbvm.com/Article/details/guzpzluyj.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/gwuksscbh.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fehbvm.com/Article/details/gwnyqnpij.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/gqctivopp.sHtML

max(d, key=d.get)
来源：http://mobile.zdbjq.cn/Article/details/gtyttxhih.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/gtbejvkdn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/gqnvvzmsp.sHtML

[U11] Py：生成器表达式
来源：http://3g.fehbvm.com/Article/details/gwtfcyzwd.sHtML

(x * 2 for x in arr)
来源：http://baike.zdbjq.cn/Article/details/gjkisrzsg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.hesvh.cn/Article/details/gmjaxjwoc.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/gkvagzbbo.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fehbvm.com/Article/details/giqmzofij.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/gylqzkufz.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/gbecbwxvj.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/gfmiodhkl.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gjfaogfbf.sHtML

t = time.perf_counter()
来源：http://3g.zdbjq.cn/Article/details/gyfuutdop.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/gakpfhbng.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/gyzedrill.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/gkiurvoom.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fehbvm.com/Article/details/gikvvhxde.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/gvlpsdmqo.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fehbvm.com/Article/details/guzktehcn.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/grmhllddm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fehbvm.com/Article/details/gocmzleae.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fehbvm.com/Article/details/goptatjim.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fehbvm.com/Article/details/guhppcyeb.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/gkwcuucel.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/gsglondxo.sHtML

[U22] Py：矩阵转置
来源：http://blog.zdbjq.cn/Article/details/guorusros.sHtML

list(zip(*m))
来源：http://blog.zdbjq.cn/Article/details/gocazlpih.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.zdbjq.cn/Article/details/gughivaqy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.hesvh.cn/Article/details/gwzkiumbo.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/gakcpolgb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gaggycipg.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/gnbkkudkk.sHtML

csv.DictReader(f)
来源：http://3g.zdbjq.cn/Article/details/gzzazyjdr.sHtML

[U26] Py：并发下载
来源：http://www.share.fehbvm.com/Article/details/gthvoxhcy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.zdbjq.cn/Article/details/glcsqovbv.sHtML

[U27] Py：异步 HTTP
来源：http://3g.zdbjq.cn/Article/details/ghsrlrqef.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.hesvh.cn/Article/details/gxzsyeeug.sHtML

[U28] Py：类型别名
来源：http://read.share.zdbjq.cn/Article/details/gcyrcanxq.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gcfzmhywy.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/gaxldpfht.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/ggnaoxmcq.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/gfjfoeqnv.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/gwasukpkd.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/gxgrrriod.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/gtwweqmzw.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gywssqkhe.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.zdbjq.cn/Article/details/gdyeyitmu.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/gpkfiznqq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.hesvh.cn/Article/details/gywblfiee.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/gcxkhywwu.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/gogmnrnhz.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.hesvh.cn/Article/details/gvmebfwbv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.hesvh.cn/Article/details/gkwkjmnax.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/ggxkbtyts.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/gutphmhpm.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/gyhgxwouf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.zdbjq.cn/Article/details/gplmfvksg.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/gelpyqgdn.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/gaqnxesvw.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fehbvm.com/Article/details/gppfiashs.sHtML

sys.stdout.isatty()
来源：http://wap.fehbvm.com/Article/details/gcjyfedya.sHtML

[U40] Py：打印到标准错误
来源：http://3g.hesvh.cn/Article/details/gglsyhevh.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/ghhojgqes.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.hesvh.cn/Article/details/gdhawmoxu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.hesvh.cn/Article/details/gjnmxajhz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fehbvm.com/Article/details/gmcovajeo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/grywbxvlr.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/gduzpuxuy.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/gffzrlslp.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.hesvh.cn/Article/details/gpijyqpor.sHtML

declare(strict_types=1);
来源：http://read.share.fehbvm.com/Article/details/glgkpnovg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/gognbvtuy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/grqzzatkj.sHtML

[U46] PHP：可空类型
来源：http://mobile.zdbjq.cn/Article/details/gkfwnspfj.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gfnhdogux.sHtML

[U47] PHP：联合类型
来源：http://www.share.zdbjq.cn/Article/details/gpbzgvvhv.sHtML

int|string $id
来源：http://www.blog.hesvh.cn/Article/details/gkztjbmjg.sHtML

[U48] PHP：纯枚举
来源：http://m.share.zdbjq.cn/Article/details/gnszqrovi.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/gnggyxryi.sHtML

[U49] PHP：只读属性
来源：http://read.share.fehbvm.com/Article/details/ggyfvowet.sHtML

public readonly string $name
来源：http://wap.fehbvm.com/Article/details/gqbpaooay.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.hesvh.cn/Article/details/gaufnitzu.sHtML

public function __construct(private int $id) {}
来源：http://m.share.zdbjq.cn/Article/details/gjrjougdo.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/guduxbvam.sHtML

[$a, $b] = $arr;
来源：http://baike.zdbjq.cn/Article/details/gbrcjzxxn.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gvapnrdwr.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/gpfwobvsl.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.hesvh.cn/Article/details/gckhseyyt.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/gschhpydk.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fehbvm.com/Article/details/gxspzmejg.sHtML

$obj?->method()
来源：http://www.m.share.zdbjq.cn/Article/details/gfgxjfdin.sHtML

[U55] PHP：match 表达式
来源：http://baike.zdbjq.cn/Article/details/ghfxcwhsq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/gafnuidqe.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/gkadyfiah.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gclnvyhvt.sHtML

[U57] PHP：字符串插值
来源：http://baike.fehbvm.com/Article/details/guejcrnyp.sHtML

"值: {$a}"
来源：http://www.share.hesvh.cn/Article/details/gyugmtssq.sHtML

[U58] PHP：数组三件套
来源：http://wap.fehbvm.com/Article/details/gkbnphknw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.zdbjq.cn/Article/details/gwixlhoqr.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/gkagkhrhn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gzadwzgkp.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.zdbjq.cn/Article/details/gvggbzdtz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/gkjtordud.sHtML

[U61] PHP：正则
来源：http://wap.fehbvm.com/Article/details/govxjpuhm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/grbrwtpwe.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/gkjutwtnr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.hesvh.cn/Article/details/gvaldtxyf.sHtML

[U63] PHP：文件读写
来源：http://wap.zdbjq.cn/Article/details/ggqlfmxqh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.hesvh.cn/Article/details/gxawjkhaa.sHtML

[U64] PHP：目录遍历
来源：http://wap.fehbvm.com/Article/details/gwygjnnmt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.zdbjq.cn/Article/details/gmziqldji.sHtML

[U65] PHP：会话
来源：http://www.blog.zdbjq.cn/Article/details/gblaiuyrq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.hesvh.cn/Article/details/gbqrvofoz.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/guzqxrxoj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.zdbjq.cn/Article/details/gvovmdnar.sHtML


<!-- 参考信息 -->