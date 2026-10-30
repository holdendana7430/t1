代发 wailian999

[S43] C++：智能指针
来源：http://3g.fehbvm.com/Article/details/gxcyujgjt.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/grmnyeddw.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/gnorkourt.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gbxkhdrwt.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gmimdgnir.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/grdtmzkbt.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/gmgbupyfd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/gfjoybzva.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/goyqtheoh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gcvkpnchf.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gzlummlmv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gcjzveytw.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/grouvutin.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/gqbcgzxdf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gghmxhjwu.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/gvxqdeefm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gavnmxcsd.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gjuqcihdn.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gyerhepmj.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gsofxgibp.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gufyipyvg.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gkuuuxhpt.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/getpcvhne.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/gqnwljkzb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/ggkfjkevg.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gzfwmqjzr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/godwjzfmc.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gifkgwqfi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gygsbkhgu.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gktlrenjx.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gdqjbxhqs.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gcqtzbnkd.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gcaiygrpb.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gkbbgbfkc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/gekapvexp.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gmmcwfeqs.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/guaccrivd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtooprcjo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gaxhjogiv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdtaqaewr.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gkucxujbc.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gqzmggjgb.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/gtvgyrkki.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/gnyuetnbs.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gjkwlpukb.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gifjwqudh.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/guqfudhhu.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/glpsiedip.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gvxhyqnch.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gbuznqtfm.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gniffkhwl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gqxpffiwl.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/ghzekofif.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gpjiaxghk.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gsoxmownj.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gjrhzfipa.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gsvlrxtbe.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gzfbmnlzg.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/geztkejte.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/gvzsgexgz.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/gcscqnmbl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/giayubuut.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gykrycbfe.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gylnzaxjv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/geyxmzsqw.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/glhtjppgc.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gfchrzlds.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gfkveytcr.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gayeerurd.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/guragtdwk.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gorvdhxjr.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gnbercenp.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/ghjdfskxw.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gmczufctx.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gyassdnnh.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gvtlvoles.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gpdqysgme.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/gcrxhxwnd.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/gzqehnhdn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gnmexvirn.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/gjxvrwbrd.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/godzhlirg.sHtML

[T22] Swift：字典
来源：http://blog.fehbvm.com/Article/details/gwtgufvoh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gcqvaywbl.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/gvncaslam.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/glqhwgbho.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/ghohcuwds.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/ghiasjevx.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/grwajmthb.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/glgiunnop.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/gpounrsxm.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/goxxjqoli.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/gwpsqaqny.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fehbvm.com/Article/details/gimcpbxfz.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/grdwacsle.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/giihqqxqz.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/gyxqgswxt.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gtheslplc.sHtML

[T30] Swift：协议
来源：http://www.share.fehbvm.com/Article/details/gvcstwicm.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/genqcpunl.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/gbnzogxcf.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gniqqijjh.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/gybdoigik.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gstethdwb.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fehbvm.com/Article/details/gfuujwyyl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/ghrlsumvt.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/ghbsrvhzh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/gomgvzsvs.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gbnyifilc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gsavtsfib.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/gyvdomesf.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/gxxdsonpy.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gzgdvvnpu.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gadhseomw.sHtML

[T38] Lua：条件
来源：http://www.blog.zdbjq.cn/Article/details/gdmmlugxq.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/gofsawkww.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gslvkpjno.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/ghllswxgq.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/gynvicqql.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/grmmvfizw.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/gjkyjfnza.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/gncyynjzy.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/gokgzjsva.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gsripvbqf.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gglqfrusf.sHtML

"值: $a"
来源：http://baike.fehbvm.com/Article/details/gcrwmpkok.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/gtbddibln.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.hesvh.cn/Article/details/gjzmdyurw.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/gtbnbbhje.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/givbslbvi.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/gqxbgtpqg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/gboiieerg.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/govygbzgx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/gvsiydkeh.sHtML

[T48] Perl：正则替换
来源：http://mobile.zdbjq.cn/Article/details/gmtochyno.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/ggdmixodi.sHtML

[T49] Perl：函数
来源：http://www.blog.zdbjq.cn/Article/details/gkpfwjgum.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gjnckusbs.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/ghvgzblsf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/giguensxy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/gtwzildok.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gnboozwuk.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gxvynruve.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/girxjniet.sHtML

val a = 1;  var b = 2
来源：http://www.blog.hesvh.cn/Article/details/gqqjktucl.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gxjjaedas.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gumqdcfpx.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gmckggovk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/giapeqgkw.sHtML

[T55] Scala：集合过滤
来源：http://blog.zdbjq.cn/Article/details/ghgpzvzco.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/gmptncdsp.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/gsxbhiqza.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gjketfrdk.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gjgpsyriv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.zdbjq.cn/Article/details/ggbohhswa.sHtML

[T58] Scala：函数定义
来源：http://blog.zdbjq.cn/Article/details/gccixkomv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/gkvairqfl.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/goxwlovzu.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/glacuanav.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/gvlmlvfvk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.zdbjq.cn/Article/details/gpxerxbvg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gsvkjygqy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gfcmnshih.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpmbouymv.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/gwfbeawgf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/gtzbqdgwe.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/gjfeoghsz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.hesvh.cn/Article/details/goekmoglr.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/ggauojpah.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/gphhmqenq.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/getadaies.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/gcrfrdtqr.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fehbvm.com/Article/details/gdexcrgir.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gwlhciecy.sHtML

[U06] Py：合并两个字典
来源：http://www.share.zdbjq.cn/Article/details/gnofxwlca.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gfjbwcsjh.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/gbtokjjfl.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fehbvm.com/Article/details/gmvidazzi.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/gghpwqjqf.sHtML

[y for x in nested for y in x]
来源：http://baike.zdbjq.cn/Article/details/gqptlusev.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/gcrkrnyrs.sHtML

max(d, key=d.get)
来源：http://www.share.fehbvm.com/Article/details/gljlpbjdx.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.zdbjq.cn/Article/details/gafotxzwl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/ggiotkghm.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/glfcdbdtb.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/gjqvruyxh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.hesvh.cn/Article/details/gzitytrsk.sHtML

Counter(arr).most_common(3)
来源：http://blog.zdbjq.cn/Article/details/ggirvpzeq.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fehbvm.com/Article/details/gpmyjwpha.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gemwrblvq.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/gddrlwrcf.sHtML

defaultdict(list)
来源：http://www.m.share.fehbvm.com/Article/details/gfavzggbl.sHtML

[U15] Py：高精度计时
来源：http://wap.fehbvm.com/Article/details/gfhknyojb.sHtML

t = time.perf_counter()
来源：http://www.share.hesvh.cn/Article/details/gykjxlfsz.sHtML

[U16] Py：命令行参数解析
来源：http://baike.hesvh.cn/Article/details/ghqbmvzte.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/grymbvahj.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/guovghamd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.hesvh.cn/Article/details/gshgcmuoz.sHtML

[U18] Py：预编译正则
来源：http://read.share.fehbvm.com/Article/details/gtqkrqvah.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.hesvh.cn/Article/details/guvjixtdp.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gjxmdskln.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.hesvh.cn/Article/details/gistgqtqr.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/gmddxmgkr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/gmquouitp.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.zdbjq.cn/Article/details/gmkmhytcm.sHtML

@contextlib.contextmanager
来源：http://www.m.share.hesvh.cn/Article/details/gpapbfmmh.sHtML

[U22] Py：矩阵转置
来源：http://baike.zdbjq.cn/Article/details/gtxgknfnr.sHtML

list(zip(*m))
来源：http://blog.zdbjq.cn/Article/details/ginwqwrvk.sHtML

[U23] Py：分块读取大文件
来源：http://wap.hesvh.cn/Article/details/gzfyoieqq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/giweqlwat.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/gizlaezfv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gbefoypzn.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.hesvh.cn/Article/details/gkswtdfhj.sHtML

csv.DictReader(f)
来源：http://www.m.share.zdbjq.cn/Article/details/ghmtfxtkc.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/gultqgyhx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/gkvdstklv.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/gdwmrqyhw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fehbvm.com/Article/details/gwikhgasp.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/gjtzauzcw.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/geatyrbyy.sHtML

[U29] Py：属性校验
来源：http://www.share.zdbjq.cn/Article/details/gtwicldbr.sHtML

@property 与 @x.setter 配合
来源：http://wap.zdbjq.cn/Article/details/gnwxobjpj.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/ggprfllph.sHtML

@dataclass(slots=True)
来源：http://mobile.zdbjq.cn/Article/details/glfszpmwo.sHtML

[U31] Py：单测
来源：http://blog.fehbvm.com/Article/details/gdyellnzc.sHtML

python -m pytest -q
来源：http://baike.fehbvm.com/Article/details/gjlmagzgu.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/gikxraqtd.sHtML

ruff format . && ruff check --fix .
来源：http://wap.zdbjq.cn/Article/details/gniggohxi.sHtML

[U33] Py：打包发布
来源：http://www.blog.hesvh.cn/Article/details/gtindytib.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fehbvm.com/Article/details/gvzmiqlkb.sHtML

[U34] Py：判断编码
来源：http://www.blog.fehbvm.com/Article/details/gboasegoh.sHtML

chardet.detect(raw)
来源：http://blog.zdbjq.cn/Article/details/ghmjfeizc.sHtML

[U35] Py：发送邮件
来源：http://www.share.hesvh.cn/Article/details/gixthkyrn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.hesvh.cn/Article/details/goppqxngx.sHtML

[U36] Py：定时任务
来源：http://mobile.fehbvm.com/Article/details/gwwmpnztm.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fehbvm.com/Article/details/gcyjeaiet.sHtML

[U37] Py：读写 Excel
来源：http://blog.zdbjq.cn/Article/details/gwudirndu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fehbvm.com/Article/details/gpmifllxc.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.hesvh.cn/Article/details/gowdixono.sHtML

Path(__file__).resolve().parent
来源：http://baike.hesvh.cn/Article/details/gjzkqitbm.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fehbvm.com/Article/details/ggdcbnnxp.sHtML

sys.stdout.isatty()
来源：http://www.m.share.hesvh.cn/Article/details/gyufwcxwg.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.zdbjq.cn/Article/details/gmqykngng.sHtML

print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gabmdnliq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/gmrazyyhe.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fehbvm.com/Article/details/gwmiwlgdf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/guuvuvvnc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.hesvh.cn/Article/details/gawtlmyeg.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.hesvh.cn/Article/details/gcxvxdgry.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/geuyegkhs.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.zdbjq.cn/Article/details/gqaxggecf.sHtML

declare(strict_types=1);
来源：http://wap.hesvh.cn/Article/details/gpkznrmrt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fehbvm.com/Article/details/gsiotqizh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gvklzvpxp.sHtML

[U46] PHP：可空类型
来源：http://m.share.fehbvm.com/Article/details/ggfnofijb.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/gszctugpl.sHtML

[U47] PHP：联合类型
来源：http://mobile.hesvh.cn/Article/details/gkbryhols.sHtML

int|string $id
来源：http://www.blog.hesvh.cn/Article/details/gvdewrhnf.sHtML

[U48] PHP：纯枚举
来源：http://blog.fehbvm.com/Article/details/gdicmjggw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.hesvh.cn/Article/details/gvryrpkgm.sHtML

[U49] PHP：只读属性
来源：http://baike.zdbjq.cn/Article/details/gtrfdlehx.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/gvnwgvdqq.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fehbvm.com/Article/details/gwqrzkukr.sHtML

public function __construct(private int $id) {}
来源：http://3g.fehbvm.com/Article/details/gegrdudof.sHtML

[U51] PHP：数组解构
来源：http://3g.hesvh.cn/Article/details/gsikroeee.sHtML

[$a, $b] = $arr;
来源：http://read.share.hesvh.cn/Article/details/gxqkxwisp.sHtML

[U52] PHP：箭头函数
来源：http://baike.fehbvm.com/Article/details/goynzzcmg.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gviupnjbu.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/gafwvqjna.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fehbvm.com/Article/details/gmitvcbxo.sHtML

[U54] PHP：空安全调用
来源：http://www.share.zdbjq.cn/Article/details/gamkxtepk.sHtML

$obj?->method()
来源：http://m.share.zdbjq.cn/Article/details/gxtzcbpsr.sHtML

[U55] PHP：match 表达式
来源：http://mobile.hesvh.cn/Article/details/ghhrdkobs.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gntoaimqk.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gldzmhwzj.sHtML

f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/glckolejc.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gigmdidif.sHtML

"值: {$a}"
来源：http://3g.zdbjq.cn/Article/details/gbjwhbfry.sHtML

[U58] PHP：数组三件套
来源：http://www.share.hesvh.cn/Article/details/gnahptpln.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fehbvm.com/Article/details/gbrwatuws.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/gzfcbolfn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gtofetnik.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.hesvh.cn/Article/details/gnobprqnk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/gmnunobwn.sHtML

[U61] PHP：正则
来源：http://baike.fehbvm.com/Article/details/gkvohpzya.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gceonuytr.sHtML

[U62] PHP：日期对象
来源：http://www.blog.zdbjq.cn/Article/details/gbesazvyn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fehbvm.com/Article/details/gwnpdauxj.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.hesvh.cn/Article/details/gkajdufxz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/genbvyobm.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/gbcpyyzlk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fehbvm.com/Article/details/guvpaflbp.sHtML

[U65] PHP：会话
来源：http://mobile.hesvh.cn/Article/details/gmihjxcrc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/ggbzbtytn.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.zdbjq.cn/Article/details/gxdqdolao.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fehbvm.com/Article/details/gvebzsdpa.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.hesvh.cn/Article/details/gnlnikjan.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fehbvm.com/Article/details/gfcyldfyd.sHtML

[U68] PHP：PDO 连接
来源：http://3g.hesvh.cn/Article/details/gaiplantz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.hesvh.cn/Article/details/gonklkamp.sHtML


<!-- 参考信息 -->