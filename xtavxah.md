代发 wailian999

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gvmdxqraz.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gfacbqdfv.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gtsjtiqjr.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/gccsyhxvp.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gwdkssfqz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/gkfeoijzr.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gqyahymuf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/ghzrjttsx.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gigsjwbho.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/glklwyxll.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gcxcavjxt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gejnvodyo.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gupbozhli.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gzqqxxbzc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/ggdovzmqr.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gvvqlogci.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gidubeyoj.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/gjqwyqygr.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gmsnavhgw.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gthqlgttu.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gzivuhzih.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/gdrdibzyr.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/gbnuxxjnv.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/glqtibecc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/giuluaftk.sHtML

[S55] C++：结构化绑定
来源：http://m.share.zdbjq.cn/Article/details/gnykpxtst.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gnfcpvllh.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gpljiombq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gjybcfvbd.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gzfdxwrxj.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gcmfhleza.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/gnffepeqx.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gvjdcnkdz.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/gihlxyxjs.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gtqvybzhc.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gpsmsztor.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/gtvqweqtf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyuitklnh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gemxqlfqo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqrkvaykz.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gwoqaishh.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/giwwjjkny.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gntwnsokm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/ggwvnbwrz.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gdvqvbtov.sHtML

"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gcekwowjk.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gjryffkeq.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gjemogtgf.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gqlnvykvb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gtgisjtmr.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gclszcskq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gislcbtrq.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/ggfgmvwgw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/gflzgxltd.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/giphxckms.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gsgkojrjn.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/gfzeougvx.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/gtbsxmmnf.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gcfbhssdg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/gqewersvr.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/gfgxfzftn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gzjgvudib.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gvkixlveb.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fehbvm.com/Article/details/ghlezjrrc.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/gkwsgoacm.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gghsumlqp.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gdiwttupe.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gyrhcymxu.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/glfmclkml.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fehbvm.com/Article/details/gvttxmxes.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gcerzypqt.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gkoscfnmo.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/gemsomtyi.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gufxvsmbr.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/ghnqimasb.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/gnxioirze.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/gexacjrns.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/grjynggie.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/gaksbevyw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/gxyurtcvu.sHtML

[T21] Swift：遍历
来源：http://wap.hesvh.cn/Article/details/gcczfrhlc.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/gnsfcibyn.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/gegatipcb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/gsbkyafwx.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gmsztxxrs.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/gyjynsqke.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/gdvpyrcsb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gkkzwimiu.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/goirmiebe.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/gwvqdvlzb.sHtML

[T26] Swift：类与重写
来源：http://baike.hesvh.cn/Article/details/guxbhcczh.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/gbohjhxlk.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/gbovwsmcf.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/gielecavv.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/gpsxodffl.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gcppwbwbz.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/gnbgnxmph.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/gbksaqexd.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/gsefsvwqa.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gjzjgwhel.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/guhawuied.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gocwscpff.sHtML

[T32] Lua：局部变量
来源：http://blog.zdbjq.cn/Article/details/ggjwjzkdk.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gjajygkrc.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/gvpkljyrn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/gonndjowu.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gnjrgimyw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/gkcqjzxbs.sHtML

[T35] Lua：字典表
来源：http://wap.zdbjq.cn/Article/details/gwevuxcdw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gmgoiygmc.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/gsqbvpyay.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/gamynreis.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gafhhutre.sHtML

"a" .. "b"
来源：http://www.m.share.fehbvm.com/Article/details/gkpseqoin.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/gsanhocub.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/gbjypiivi.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gvoqgbttn.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/ggppnvnef.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gkhoimqem.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fehbvm.com/Article/details/girxmtypf.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/gpgxdpxga.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/gtgetuwxb.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/glsttplrz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/gydpdfylw.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gfgomtoti.sHtML

"值: $a"
来源：http://m.share.hesvh.cn/Article/details/gzpnsfber.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/gmzzwuwyf.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fehbvm.com/Article/details/gtxppxlhu.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/gujinckiu.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/gbofkfhuo.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gainuhujn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.hesvh.cn/Article/details/gfhmxnvux.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/gbodgeazs.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gwpucloaf.sHtML

[T48] Perl：正则替换
来源：http://blog.hesvh.cn/Article/details/gdekiydxg.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/galqcbldp.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gpdderylr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gvupizqjj.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gsbetjmtl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/gygluaoqz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/ghvqmipzm.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/gggerawdo.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/goagfzaoy.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/gnvewoyew.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/gpwebzzez.sHtML

[T53] Scala：字符串插值
来源：http://baike.fehbvm.com/Article/details/gzmwkhhpm.sHtML

s"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gbygwddra.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gzlmxcidc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fehbvm.com/Article/details/gecnxiqqp.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/ghkfxadyj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gnhfxnyyj.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/gwgomnlzs.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/grehvoomo.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gjtanmnme.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/gzxrtzbjc.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/gczpqghcg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/gekogbqzx.sHtML

[T59] Scala：循环
来源：http://3g.hesvh.cn/Article/details/gieyjbjbq.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/grucfpuse.sHtML

[T60] Scala：折叠
来源：http://m.share.hesvh.cn/Article/details/gnpxommut.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gsdiigxzc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggtpuhxep.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gnmhghbtt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gubbljzdy.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/gkhigiqnb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gwjjwavzi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.zdbjq.cn/Article/details/gfyqprteb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fehbvm.com/Article/details/grxcjrkwp.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fehbvm.com/Article/details/glimwmtcz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/gdibagaza.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.zdbjq.cn/Article/details/godcxnqna.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.hesvh.cn/Article/details/gukqkiwbc.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/gzgnobfck.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gsektrqxt.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/ghryitvli.sHtML

{**a, **b}
来源：http://wap.zdbjq.cn/Article/details/gcslsqlnw.sHtML

[U07] Py：反转字典键值
来源：http://blog.hesvh.cn/Article/details/giofkyfft.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/ghyfrjxkm.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/goszxulzc.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/gcinshihn.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/gvmuwpyzv.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/gefhypudo.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.hesvh.cn/Article/details/girazeege.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fehbvm.com/Article/details/ggwoyswvh.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/gvrfavego.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/gamsmagns.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.zdbjq.cn/Article/details/gawgxsnci.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/gwheysgow.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/gqzjwkxgk.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/gmteyitvx.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/gkmmdaqlx.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/giievogqu.sHtML

[U15] Py：高精度计时
来源：http://read.share.hesvh.cn/Article/details/glwfyruor.sHtML

t = time.perf_counter()
来源：http://wap.hesvh.cn/Article/details/grndfhend.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.zdbjq.cn/Article/details/gbambfbzh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/grnbmofoi.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/geqcrirkm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/giqiioick.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.zdbjq.cn/Article/details/ghueiyrbh.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/glqhbborp.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.zdbjq.cn/Article/details/gqqyjpguw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/gwnohbzha.sHtML

[U20] Py：缓存函数结果
来源：http://wap.zdbjq.cn/Article/details/gcyqfdpeg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.hesvh.cn/Article/details/gjgixbaqy.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.zdbjq.cn/Article/details/grmmlaton.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/gncjfcouh.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/gcjpczhnc.sHtML

list(zip(*m))
来源：http://www.m.share.zdbjq.cn/Article/details/guwhiwdbk.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fehbvm.com/Article/details/gvbyoowpc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.zdbjq.cn/Article/details/gjkljmeug.sHtML

[U24] Py：路径操作
来源：http://baike.zdbjq.cn/Article/details/giqolerdl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gzbngjwdh.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/gtncyycnq.sHtML

csv.DictReader(f)
来源：http://baike.fehbvm.com/Article/details/gjgesswur.sHtML

[U26] Py：并发下载
来源：http://www.m.share.zdbjq.cn/Article/details/gagdcvhux.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.zdbjq.cn/Article/details/gclpvsjzb.sHtML

[U27] Py：异步 HTTP
来源：http://baike.zdbjq.cn/Article/details/gygpgohai.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fehbvm.com/Article/details/gjxbrokxb.sHtML

[U28] Py：类型别名
来源：http://3g.fehbvm.com/Article/details/gluiqkjgv.sHtML

UserId = int
来源：http://wap.zdbjq.cn/Article/details/gpovuvxqz.sHtML

[U29] Py：属性校验
来源：http://read.share.hesvh.cn/Article/details/goqqrqcim.sHtML

@property 与 @x.setter 配合
来源：http://baike.fehbvm.com/Article/details/gpuytvgzv.sHtML

[U30] Py：数据类
来源：http://m.share.zdbjq.cn/Article/details/gpnylwuft.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/grsuutbgy.sHtML

[U31] Py：单测
来源：http://read.share.fehbvm.com/Article/details/gjghfrzuh.sHtML

python -m pytest -q
来源：http://read.share.zdbjq.cn/Article/details/gsyprqiyv.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fehbvm.com/Article/details/gzuuewcgp.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.zdbjq.cn/Article/details/gtnzftsbt.sHtML

[U33] Py：打包发布
来源：http://blog.hesvh.cn/Article/details/gzdqggivm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.zdbjq.cn/Article/details/gyyjytcmr.sHtML

[U34] Py：判断编码
来源：http://wap.hesvh.cn/Article/details/gfxdzcadu.sHtML

chardet.detect(raw)
来源：http://read.share.hesvh.cn/Article/details/gneztasyl.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/gagitzyhf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fehbvm.com/Article/details/grgknqszd.sHtML

[U36] Py：定时任务
来源：http://blog.hesvh.cn/Article/details/gkmajwurv.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/gqizsrkrt.sHtML

[U37] Py：读写 Excel
来源：http://mobile.zdbjq.cn/Article/details/ghqhbrvjy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fehbvm.com/Article/details/gshsxlnot.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/gqgkddyde.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gkvnvmsjr.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fehbvm.com/Article/details/gvvmfphkc.sHtML

sys.stdout.isatty()
来源：http://blog.zdbjq.cn/Article/details/gqdhhdxrg.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fehbvm.com/Article/details/gswpuaeyi.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gbaqhuheg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gqebaamqs.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.zdbjq.cn/Article/details/ghhmirgsv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gorcuifsg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/gafuhiodr.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.hesvh.cn/Article/details/gaqjgfmnp.sHtML

namespace App\Http;
来源：http://baike.fehbvm.com/Article/details/gmgtwbdeh.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.hesvh.cn/Article/details/gbzghnhzb.sHtML

declare(strict_types=1);
来源：http://m.share.fehbvm.com/Article/details/goiierrqs.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.zdbjq.cn/Article/details/gjoygkuvd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gpynyhrgv.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/ginseelbe.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/gfvwjmopl.sHtML

[U47] PHP：联合类型
来源：http://wap.fehbvm.com/Article/details/gnqmkkovf.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/gmtwuevkl.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/gntuqtybx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fehbvm.com/Article/details/gszpczcru.sHtML

[U49] PHP：只读属性
来源：http://read.share.fehbvm.com/Article/details/gswwavbfh.sHtML

public readonly string $name
来源：http://mobile.zdbjq.cn/Article/details/gononfbim.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/gbniwrtgu.sHtML

public function __construct(private int $id) {}
来源：http://3g.zdbjq.cn/Article/details/ggkaoenlr.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/gcouufugk.sHtML

[$a, $b] = $arr;
来源：http://read.share.zdbjq.cn/Article/details/ghntasdle.sHtML

[U52] PHP：箭头函数
来源：http://wap.zdbjq.cn/Article/details/guzattjrd.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.hesvh.cn/Article/details/guhllfkcd.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fehbvm.com/Article/details/gobljajtk.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.zdbjq.cn/Article/details/gvqlpejev.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/gmzqntgwi.sHtML

$obj?->method()
来源：http://m.share.fehbvm.com/Article/details/gylimeumf.sHtML

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/gtadhgjil.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gksvvozvm.sHtML

[U56] PHP：命名参数
来源：http://www.share.hesvh.cn/Article/details/gjebgvtxc.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/geogkdokj.sHtML

[U57] PHP：字符串插值
来源：http://3g.hesvh.cn/Article/details/geqbglacl.sHtML

"值: {$a}"
来源：http://baike.fehbvm.com/Article/details/gtaiwwjlc.sHtML

[U58] PHP：数组三件套
来源：http://blog.zdbjq.cn/Article/details/gtqprqpow.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/gqgszalkj.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/guoaqeapt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gmsxhpikl.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/ghpzcjyuc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/gerjqrcce.sHtML

[U61] PHP：正则
来源：http://read.share.fehbvm.com/Article/details/gftaxuvpi.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gtqhmmnhs.sHtML

[U62] PHP：日期对象
来源：http://read.share.hesvh.cn/Article/details/grqddsyzb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fehbvm.com/Article/details/gytmveufu.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/gupxrckmb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.hesvh.cn/Article/details/ggimoeyfd.sHtML

[U64] PHP：目录遍历
来源：http://3g.hesvh.cn/Article/details/gnfwfafvm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.hesvh.cn/Article/details/gkxktciex.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/gjdgzwsmp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.hesvh.cn/Article/details/gnnbzswnp.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/gfmcokefb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.hesvh.cn/Article/details/gfguuyneb.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.zdbjq.cn/Article/details/gmeqgbeiv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fehbvm.com/Article/details/gxoaueygw.sHtML

[U68] PHP：PDO 连接
来源：http://3g.hesvh.cn/Article/details/gsywthqjz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/gsjwmdxdf.sHtML


<!-- 参考信息 -->