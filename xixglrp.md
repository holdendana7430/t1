代发 wailian999

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gpjrcvsgj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/gswusyfww.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/goygctuwl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gekpotiyw.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gkglnqerx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gvsjblfke.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gxtyphedb.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gqbvltjbh.sHtML

[S43] C++：智能指针
来源：http://baike.zdbjq.cn/Article/details/gctxgamdp.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gucoyxrof.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/gzwxeqkrk.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gwhwlnmry.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gxcgqoims.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gykssjlei.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/ggaeoszrr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gkowbhxkh.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gtmfdlvvf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/ghntczweg.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gvhiqniiw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gswjyhqgb.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/gpaeweevy.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gquwkgyhl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/gkodsljkr.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/gowxirqvw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gbgkilgby.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/guakjfhtz.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/gtvkypiea.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gzwhusqtt.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gelesgirm.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/guaknwhsg.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gcdhblrns.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gwvmpzxrg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gdnhtltxy.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gxkhgbvvk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/gfwxqgigo.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gxszawiyx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/gxxfytvda.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/grzaaccns.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gtnmczefn.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gdrkxxfdz.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gpvfkinyo.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gbcghduox.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gwphrxivz.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gitaoeirc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gijjsufqm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gushwguap.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gxszqvcji.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gutxyhsku.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gyaqzmclx.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gfgboorru.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gywukjlgs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gjcxleref.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gbvchjtaj.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/guiblofzp.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gyqwgfhik.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gtdyqepqb.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gqjajkznb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gczjmxocn.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gcjlsmitf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gfryqiojw.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/glbzyvtlh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gkaheomft.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/gvdbegarq.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gmdusnykh.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gtqgncwdc.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/getyhtzcy.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gssqjvcwy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/grptrwwcj.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/gkuemttef.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gsatbwvsh.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gkislgmuf.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fehbvm.com/Article/details/gqmvaqkey.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/gdsbufrmo.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gixynshvb.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/gmlctxslh.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/ggkbtgnti.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gzqtqldzf.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/genfmvztd.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/ggofvyygx.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/grdrsfleb.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/gyknnchde.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/gludvsapp.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gnzzmcowl.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/gxrzpalev.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/gphooylai.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/gcinnxxta.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/gfxruowzp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/gjioebfgu.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gmuyhpdtj.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gayrwwdnn.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gpdaaxxye.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gqtmhyqhn.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/giwkrtrux.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/grksxhxno.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/gnhfbntib.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gdseogakg.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gxsppufwi.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gwaeolqyk.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/gtcgjkpar.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/gyppplvwt.sHtML

[T27] Swift：错误处理
来源：http://read.share.hesvh.cn/Article/details/gzqljhfzs.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/gzttrruen.sHtML

[T28] Swift：枚举
来源：http://3g.zdbjq.cn/Article/details/gtmsjzfwe.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gsuzzuhpy.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gsaolxjpl.sHtML

guard let x = opt else { return }
来源：http://www.share.zdbjq.cn/Article/details/gllifsaer.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gawrnwlul.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/gkqngobts.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gzyusqsik.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gxngilrby.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/gqfsaynjj.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gfmtbquxp.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/geocsarnr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/gtjgtqyje.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/gikcrgcsa.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/gnzrobwff.sHtML

[T35] Lua：字典表
来源：http://m.share.hesvh.cn/Article/details/grumynwrx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/ghfahkncs.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gdfzeqysu.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/gtaraqfsb.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/gaujxcwxw.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gdwzywoes.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/goeeqleqx.sHtML

if x > 0 then print("正") end
来源：http://m.share.zdbjq.cn/Article/details/gowyvhctr.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gygtitjmd.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gnzyplotc.sHtML

[T40] Lua：元表
来源：http://wap.hesvh.cn/Article/details/gojwogmfe.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gwtuxlevg.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/gellkjpey.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/gezwyflfr.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/gsniqxpqp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/grlyemybw.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/grnyzyzlk.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gckqgtxlc.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/gnwmrysef.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/gfllattch.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/gjhxuqmxr.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/gjqmyzege.sHtML

[T46] Perl：哈希操作
来源：http://3g.zdbjq.cn/Article/details/goxmdvhbf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gjnsjfkvf.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gpckyhqca.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/gbrqdohqi.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gmdupyhrb.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gyzhpdyaa.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/grqafxzaq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gtlyyaovx.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gbvnfrtlx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/goemgxoaw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/guzdakung.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/grphymhmy.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gwfmaubcw.sHtML

[T52] Scala：变量
来源：http://3g.fehbvm.com/Article/details/gekobcwrf.sHtML

val a = 1;  var b = 2
来源：http://read.share.fehbvm.com/Article/details/gdaudjgyj.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gtnkzhjyj.sHtML

s"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gonxchxvl.sHtML

[T54] Scala：集合映射
来源：http://m.share.hesvh.cn/Article/details/gqdddivik.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/gdssuycwp.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gpvpxttyp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fehbvm.com/Article/details/gafkcfglz.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/gftblxhns.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/gtjwfhsln.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gefelbjrg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gclobrgrd.sHtML

[T58] Scala：函数定义
来源：http://mobile.fehbvm.com/Article/details/gvqqgmach.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/gvvkwikuw.sHtML

[T59] Scala：循环
来源：http://www.m.share.hesvh.cn/Article/details/gcaibegzc.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gzyxvxcxg.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/ghpizcxxn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fehbvm.com/Article/details/gljwzcggh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwtmytqeh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/galonlvlt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxwlhiryf.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fehbvm.com/Article/details/gdrctzmik.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/gxphluvfc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fehbvm.com/Article/details/gorfilrsf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gnyzpfpjq.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fehbvm.com/Article/details/gbbzwbvhw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/gvwjaphoo.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/gkfchiohu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gjmurbkvm.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/gqnrxabzn.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gtunelcoq.sHtML

[U06] Py：合并两个字典
来源：http://m.share.hesvh.cn/Article/details/grczwqkqu.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/ggitrrjyq.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/gtannbubl.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gmgpqpkti.sHtML

[U08] Py：展平二维列表
来源：http://www.share.hesvh.cn/Article/details/gtjpqfsag.sHtML

[y for x in nested for y in x]
来源：http://3g.fehbvm.com/Article/details/gyscbmvye.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/gdifflfmm.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gzjpdwsvu.sHtML

[U10] Py：按值排序字典
来源：http://m.share.zdbjq.cn/Article/details/gtilncgid.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gkfltpjkg.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/gggdozkml.sHtML

(x * 2 for x in arr)
来源：http://www.blog.zdbjq.cn/Article/details/guflalbgb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/gotqtebnw.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/ghvudiesr.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/gkvkahyul.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/gauedromc.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/grqpipdzk.sHtML

defaultdict(list)
来源：http://wap.hesvh.cn/Article/details/gbsmhhtxv.sHtML

[U15] Py：高精度计时
来源：http://baike.hesvh.cn/Article/details/gdcfpxdsp.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/gxnbjysgo.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/gckoanacc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/ggsuzyvyq.sHtML

[U17] Py：初始化日志
来源：http://3g.fehbvm.com/Article/details/gzzhdbqbo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.zdbjq.cn/Article/details/gcankfnlu.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/geebhzhyb.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gmrwuvalr.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/gcxpafpox.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.hesvh.cn/Article/details/gpricxcaa.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/gomzkitkv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.hesvh.cn/Article/details/gterrvwuq.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.hesvh.cn/Article/details/gkgtaduof.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/geovfvjjd.sHtML

[U22] Py：矩阵转置
来源：http://3g.zdbjq.cn/Article/details/gqxhwgjyk.sHtML

list(zip(*m))
来源：http://3g.zdbjq.cn/Article/details/gnkugtlbr.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.zdbjq.cn/Article/details/gcjwgniie.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fehbvm.com/Article/details/gogbhodkx.sHtML

[U24] Py：路径操作
来源：http://baike.fehbvm.com/Article/details/gjclgpvbc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gcdhwrdaz.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fehbvm.com/Article/details/gwplpbaqu.sHtML

csv.DictReader(f)
来源：http://read.share.fehbvm.com/Article/details/gcyxtfocl.sHtML

[U26] Py：并发下载
来源：http://read.share.hesvh.cn/Article/details/gmccxatqx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fehbvm.com/Article/details/gfzwxxiqf.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fehbvm.com/Article/details/goufldaev.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.zdbjq.cn/Article/details/gtrhtdsrl.sHtML

[U28] Py：类型别名
来源：http://m.share.zdbjq.cn/Article/details/gdisxaazf.sHtML

UserId = int
来源：http://mobile.fehbvm.com/Article/details/gzdqzuakq.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fehbvm.com/Article/details/gbgnfzcbv.sHtML

@property 与 @x.setter 配合
来源：http://m.share.zdbjq.cn/Article/details/gpcbevavi.sHtML

[U30] Py：数据类
来源：http://www.share.fehbvm.com/Article/details/ghycarfds.sHtML

@dataclass(slots=True)
来源：http://m.share.zdbjq.cn/Article/details/gybhcurtb.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/gndbuapks.sHtML

python -m pytest -q
来源：http://baike.fehbvm.com/Article/details/gsdyrolny.sHtML

[U32] Py：代码格式化
来源：http://baike.fehbvm.com/Article/details/gpefgnbdg.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fehbvm.com/Article/details/gpoxwhddx.sHtML

[U33] Py：打包发布
来源：http://www.share.zdbjq.cn/Article/details/gvbgrclyz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fehbvm.com/Article/details/ghmljqwal.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/gqbqglzes.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/gigdmpcvc.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/gnpgwugni.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.hesvh.cn/Article/details/gumywonsh.sHtML

[U36] Py：定时任务
来源：http://blog.zdbjq.cn/Article/details/gnqdodcfd.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.hesvh.cn/Article/details/gubmapxil.sHtML

[U37] Py：读写 Excel
来源：http://www.share.zdbjq.cn/Article/details/ghcoaczxe.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.zdbjq.cn/Article/details/godjthaqq.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/gebxitboj.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/gxzqvvdsp.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fehbvm.com/Article/details/gsqnawbcs.sHtML

sys.stdout.isatty()
来源：http://blog.zdbjq.cn/Article/details/giitpbjdv.sHtML

[U40] Py：打印到标准错误
来源：http://baike.zdbjq.cn/Article/details/gvubmlrph.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gsqozvpbw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gmrdqklyl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/gwgupbvec.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gjdhjanbe.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/gqzumwxtb.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fehbvm.com/Article/details/genurrqko.sHtML

namespace App\Http;
来源：http://blog.fehbvm.com/Article/details/gysflzzfx.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fehbvm.com/Article/details/gmcdgugiu.sHtML

declare(strict_types=1);
来源：http://baike.hesvh.cn/Article/details/gzjaywlot.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/gsmzsbfdq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gjrhvyxwm.sHtML

[U46] PHP：可空类型
来源：http://baike.zdbjq.cn/Article/details/gbywtckat.sHtML

?string $name = null
来源：http://blog.hesvh.cn/Article/details/ggjsnvezz.sHtML

[U47] PHP：联合类型
来源：http://m.share.fehbvm.com/Article/details/gtyuadqxu.sHtML

int|string $id
来源：http://3g.fehbvm.com/Article/details/gbqkqiznv.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/gdtbmhtet.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.zdbjq.cn/Article/details/gdhimdsnq.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fehbvm.com/Article/details/gcsihllnz.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/gfqwvbiug.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.zdbjq.cn/Article/details/gtssemvup.sHtML

public function __construct(private int $id) {}
来源：http://baike.hesvh.cn/Article/details/glspgcnwm.sHtML

[U51] PHP：数组解构
来源：http://m.share.hesvh.cn/Article/details/gcmjzympw.sHtML

[$a, $b] = $arr;
来源：http://www.share.fehbvm.com/Article/details/gdfssgthh.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gheqylvre.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fehbvm.com/Article/details/gzjayvdqo.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fehbvm.com/Article/details/gduvosrrf.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/glrhkmqig.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fehbvm.com/Article/details/geibbcutw.sHtML

$obj?->method()
来源：http://wap.fehbvm.com/Article/details/gbsybykut.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fehbvm.com/Article/details/ghfqvuhih.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/gcizqqipz.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fehbvm.com/Article/details/gosbyzaee.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/grqgsprkk.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/gtbsfupmp.sHtML

"值: {$a}"
来源：http://m.share.fehbvm.com/Article/details/grakvpegn.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/gdghklclp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.hesvh.cn/Article/details/ginjcflju.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.zdbjq.cn/Article/details/goxmevdgk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gbwbkrkvi.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.hesvh.cn/Article/details/gdjhialmg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fehbvm.com/Article/details/gjftdfhlb.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/gnjsgnbcf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gdmgqxxxy.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/gzbmcanrn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.hesvh.cn/Article/details/gspcsnpct.sHtML

[U63] PHP：文件读写
来源：http://m.share.hesvh.cn/Article/details/gewifeebv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.hesvh.cn/Article/details/gunqgjrka.sHtML

[U64] PHP：目录遍历
来源：http://baike.zdbjq.cn/Article/details/gieolhalx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.zdbjq.cn/Article/details/gmlkjiahm.sHtML


<!-- 参考信息 -->