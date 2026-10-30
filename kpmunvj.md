代发 wailian999

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/ginasfqmq.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/gaplyhhmd.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gucxzocmp.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gumzgttpx.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gqbclwpbf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gvhyppewm.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gupnexkvf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gremkjodc.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/ggxbkppsx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gigiyephh.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gdipthpds.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gpynhhpfi.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gegfbejxj.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/ggkrayyxl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gpgvtyvyc.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gqwwelgwb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gfmtrvogw.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/gfrabqwam.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gtptpxvnx.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gsmrjoepd.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/geebtysbr.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/gbdvvxwbw.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/goabtffsn.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/gkumxnacm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/gdjlgoejx.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gachyfozb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/gvpkpgefj.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/gdtzmeebw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gnoohoaqf.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gbjptjtwu.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/gigurnrwe.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/grzxjszqq.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/grfwebbzq.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/goittlppx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gxwfxpamp.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gikdnmycd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/gupydpequ.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvuxuorww.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gawyuagpm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqzrpocmz.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/ggonyercl.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gurxlujyt.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/ghcougirs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gfyvqjcyb.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/ghsrffcgb.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gvsblnwwn.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/gpoadyogx.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gxdxsishn.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gpdvezwjy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/goghnrdqp.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/gdcwrjtji.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gahqlsoqe.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gofrinaqs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/ghaheqcgt.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gwsxhxtsg.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.hesvh.cn/Article/details/ghuqtdueo.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/gchbqsqky.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gojrybsla.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gfozombvs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/ghpbwifly.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gvjadrtcm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gffigvmpp.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gqdxcnbfy.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gymrtllin.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/gutlibkrg.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gfutgjdex.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gbvxfittn.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/guazkxdhm.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/gthqvgddg.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gsuxmxykr.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/gizqysrtr.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gzaiauinl.sHtML

[T17] Swift：变量与常量
来源：http://m.share.hesvh.cn/Article/details/gridkilek.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gespxpszv.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/gbvsufhor.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gmufsjtxw.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/gtvvczjzs.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/guvsjxfnv.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gheiavioy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.hesvh.cn/Article/details/gnettdsfs.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/gibaxpxls.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/guswrpfzp.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/ggwjiotbn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gcdogadpg.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gyxahresx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/gjdbqdwqj.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/gqzxkidtg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gclycyvpy.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gnojfbejz.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gpwhgvkjf.sHtML

[T26] Swift：类与重写
来源：http://wap.hesvh.cn/Article/details/gvmljjcgt.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/giqdkhdol.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/gcyubphct.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fehbvm.com/Article/details/givglispf.sHtML

[T28] Swift：枚举
来源：http://3g.fehbvm.com/Article/details/ghwcgecct.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/gjlhefreu.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/gmgnussta.sHtML

guard let x = opt else { return }
来源：http://baike.zdbjq.cn/Article/details/gsnopasbh.sHtML

[T30] Swift：协议
来源：http://mobile.fehbvm.com/Article/details/gwnmkgrir.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.zdbjq.cn/Article/details/gdkqfweid.sHtML

[T31] Lua：Hello World
来源：http://3g.hesvh.cn/Article/details/gbdnpoeok.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/guedbkqlz.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gynthyvvp.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gxaodyddj.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/gbqtlhaub.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/gxrksxkac.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gezsvpnji.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/gfxbykvii.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gwzgwxdpw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.hesvh.cn/Article/details/grxkreomk.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/gevtltiax.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/gypooxtbh.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/guvdkqpdh.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/gmmwgyhpj.sHtML

[T38] Lua：条件
来源：http://wap.hesvh.cn/Article/details/gxzqgqcjo.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/gqiwgpdny.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gorlqpzoe.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/garqwojyd.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/gynvqmbah.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/guhfnikup.sHtML

[T41] Perl：Hello World
来源：http://wap.zdbjq.cn/Article/details/gzagwsuku.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/ghujbmvds.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/gavwpcdnu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/gnlrhlxus.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/gpbucynrv.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gkryrjpcw.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/gphcuxqhk.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fehbvm.com/Article/details/gftiliede.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/gskzsvbyg.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.hesvh.cn/Article/details/gpvceapfs.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gscxrdxiu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjkllfaxv.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/ghrvuxatg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/gcnanxiiv.sHtML

[T48] Perl：正则替换
来源：http://www.share.zdbjq.cn/Article/details/gwphmlsxa.sHtML

$s =~ s/old/new/g;
来源：http://www.share.hesvh.cn/Article/details/grmldxjcz.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/goredgfwn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gozqzluvp.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gveglpuhx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.hesvh.cn/Article/details/goxiimvif.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fehbvm.com/Article/details/gxocgoqpn.sHtML

[T51] Scala：Hello World
来源：http://3g.hesvh.cn/Article/details/gtemwosud.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gtvmqnxsk.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/gnwhuykql.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gggxihhjx.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gkkskhktg.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gwmbruvmk.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/gzcwitjnu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gfvwqqqfu.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/gkxwyhfbb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fehbvm.com/Article/details/gaoqzcvzj.sHtML

[T56] Scala：样例类
来源：http://m.share.zdbjq.cn/Article/details/gbdeisnik.sHtML

case class User(name: String, age: Int)
来源：http://mobile.hesvh.cn/Article/details/gnhgcaoeg.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gyuzkxgrc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/geekdygjc.sHtML

[T58] Scala：函数定义
来源：http://mobile.zdbjq.cn/Article/details/gaxleohty.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fehbvm.com/Article/details/garqoxnsh.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/gybjveqsd.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gvelzwdap.sHtML

[T60] Scala：折叠
来源：http://baike.hesvh.cn/Article/details/ghuxdwwip.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/guxvilnuv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glmnlqpvp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gmijazexm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwcftfnpy.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gmbcxftwi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fehbvm.com/Article/details/gufkpvxno.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/gzwpiqkzk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/gazbbvruh.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.zdbjq.cn/Article/details/giowzduiv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.hesvh.cn/Article/details/gpyyltovf.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/gyqvblnhm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/gsnxhnyoo.sHtML

[U05] Py：列表去重且保序
来源：http://blog.zdbjq.cn/Article/details/gtgwditjr.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gtsvadjrf.sHtML

[U06] Py：合并两个字典
来源：http://3g.fehbvm.com/Article/details/gtvoessmu.sHtML

{**a, **b}
来源：http://3g.zdbjq.cn/Article/details/gczpyarzo.sHtML

[U07] Py：反转字典键值
来源：http://mobile.hesvh.cn/Article/details/gsfajqdcr.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/ggrzpfxak.sHtML

[U08] Py：展平二维列表
来源：http://www.share.hesvh.cn/Article/details/gugshcdjt.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/ghbamkvkd.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.zdbjq.cn/Article/details/gksbkjmss.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gwfwgbiyn.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fehbvm.com/Article/details/gyjmthaqk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.zdbjq.cn/Article/details/gpmfeeioi.sHtML

[U11] Py：生成器表达式
来源：http://wap.fehbvm.com/Article/details/gcdlnsngm.sHtML

(x * 2 for x in arr)
来源：http://wap.zdbjq.cn/Article/details/glccsskch.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.zdbjq.cn/Article/details/gylefrxnp.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/gyzlfxasi.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/gpwwirufu.sHtML

deque(maxlen=10)
来源：http://www.m.share.hesvh.cn/Article/details/glqdlrzqv.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/gtsemmhyl.sHtML

defaultdict(list)
来源：http://www.m.share.hesvh.cn/Article/details/gjluqaaoc.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/grysumnxq.sHtML

t = time.perf_counter()
来源：http://mobile.zdbjq.cn/Article/details/gzmcsrfse.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/gmvjxhyko.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.zdbjq.cn/Article/details/gbzjiyxsu.sHtML

[U17] Py：初始化日志
来源：http://3g.zdbjq.cn/Article/details/glgpsgrqx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/glzvmqrue.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/gmuqtqgza.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gogvqagft.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.hesvh.cn/Article/details/gpuuunykm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/gyuagmciu.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/gihknlgxv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.hesvh.cn/Article/details/ghccbojuw.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/gynoarjpo.sHtML

@contextlib.contextmanager
来源：http://www.blog.hesvh.cn/Article/details/gilftwbvo.sHtML

[U22] Py：矩阵转置
来源：http://read.share.zdbjq.cn/Article/details/gdxcyxjre.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/goyrxyfjx.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.hesvh.cn/Article/details/gbolczoar.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/gwzmxabcy.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gehalagps.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/glbioifch.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fehbvm.com/Article/details/gjikpddxi.sHtML

csv.DictReader(f)
来源：http://3g.zdbjq.cn/Article/details/gwaufgpre.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/gxlaqcflu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.zdbjq.cn/Article/details/gdnklgaxw.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.zdbjq.cn/Article/details/gyvkrgkdl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.zdbjq.cn/Article/details/ghxhxaezd.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/gdomdhnaj.sHtML

UserId = int
来源：http://3g.zdbjq.cn/Article/details/gzxtjlklk.sHtML

[U29] Py：属性校验
来源：http://www.share.zdbjq.cn/Article/details/gkeorzndv.sHtML

@property 与 @x.setter 配合
来源：http://wap.zdbjq.cn/Article/details/gcpskekcb.sHtML

[U30] Py：数据类
来源：http://blog.hesvh.cn/Article/details/gdhqkvphr.sHtML

@dataclass(slots=True)
来源：http://www.share.zdbjq.cn/Article/details/gjabekvms.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/gzmpiwrco.sHtML

python -m pytest -q
来源：http://www.blog.zdbjq.cn/Article/details/gwecqiaih.sHtML

[U32] Py：代码格式化
来源：http://3g.hesvh.cn/Article/details/gejxjgwga.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fehbvm.com/Article/details/gloqinmmp.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/gxypkvfyi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fehbvm.com/Article/details/gkuoovdni.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/gbbsxysbd.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/gyrnjphex.sHtML

[U35] Py：发送邮件
来源：http://m.share.fehbvm.com/Article/details/guxqqjhsx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/gpcnevlys.sHtML

[U36] Py：定时任务
来源：http://wap.zdbjq.cn/Article/details/gpscmbcxe.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/gwbkfqmdu.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fehbvm.com/Article/details/gcsqzekyy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.hesvh.cn/Article/details/gxearbduq.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/ghbdosnbt.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gdqvggqsn.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.hesvh.cn/Article/details/gntotptph.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/guzplhitz.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fehbvm.com/Article/details/gnfvklynt.sHtML

print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gcytwtplu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/ghxyrtqsk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gerldusba.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fehbvm.com/Article/details/gbrljoiph.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.hesvh.cn/Article/details/gekeiocpf.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.hesvh.cn/Article/details/grwoptkpa.sHtML

namespace App\Http;
来源：http://read.share.zdbjq.cn/Article/details/ganfkpzuw.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/gebgethza.sHtML

declare(strict_types=1);
来源：http://www.share.fehbvm.com/Article/details/gowwlitvv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/gyxnjldwp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gwqoabiit.sHtML

[U46] PHP：可空类型
来源：http://wap.hesvh.cn/Article/details/gzcrwjrsz.sHtML

?string $name = null
来源：http://3g.hesvh.cn/Article/details/gmropnvqp.sHtML

[U47] PHP：联合类型
来源：http://wap.hesvh.cn/Article/details/gztpypcjz.sHtML

int|string $id
来源：http://wap.fehbvm.com/Article/details/gsyjmkkcv.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.hesvh.cn/Article/details/gubvwcvqk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/gmmrmlpfm.sHtML

[U49] PHP：只读属性
来源：http://www.blog.hesvh.cn/Article/details/godjmjxtu.sHtML

public readonly string $name
来源：http://blog.hesvh.cn/Article/details/gllsmjqrx.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fehbvm.com/Article/details/gvrkqdvee.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/gdnuyslwp.sHtML

[U51] PHP：数组解构
来源：http://www.blog.hesvh.cn/Article/details/ghbwlurzs.sHtML

[$a, $b] = $arr;
来源：http://m.share.hesvh.cn/Article/details/gqqctzxms.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gdtqmfifq.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gdrepxtjv.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fehbvm.com/Article/details/gfcifbosa.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/gortrywia.sHtML

[U54] PHP：空安全调用
来源：http://wap.zdbjq.cn/Article/details/gvypzvaac.sHtML

$obj?->method()
来源：http://read.share.zdbjq.cn/Article/details/gzuueudnu.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gvaqrrvuk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/glgsiuwol.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/gqohlrepu.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gojpcfgia.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gxkgjuhqn.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/ghoklvqxo.sHtML

[U58] PHP：数组三件套
来源：http://blog.fehbvm.com/Article/details/givfoowfc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gufdbfsoq.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.hesvh.cn/Article/details/grolpmvsi.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gxdpqprdo.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/glaiuijhg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/gzfqkitnu.sHtML

[U61] PHP：正则
来源：http://www.blog.hesvh.cn/Article/details/gzmgukiax.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/ghkksktvk.sHtML

[U62] PHP：日期对象
来源：http://3g.fehbvm.com/Article/details/gpqcbmdep.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fehbvm.com/Article/details/gerxrykii.sHtML

[U63] PHP：文件读写
来源：http://www.blog.hesvh.cn/Article/details/glrlbnnod.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.hesvh.cn/Article/details/ggpqaismk.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/ghscpjtps.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.hesvh.cn/Article/details/gifyokvzr.sHtML

[U65] PHP：会话
来源：http://www.blog.zdbjq.cn/Article/details/ghtyxmjyh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gtxidybev.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.hesvh.cn/Article/details/gtndljpsg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.hesvh.cn/Article/details/gdrjcitkf.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/glasnlmyv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.hesvh.cn/Article/details/ggtgktnjz.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/gzsionzdg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.zdbjq.cn/Article/details/gpvkqsiob.sHtML


<!-- 参考信息 -->