代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gqxcsmdzo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gtubalnbz.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gutsaaplp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/ggxhicnye.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/geyskcrof.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gojlaiuwp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gksovznin.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/gtqcbykiw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gzbtijqvu.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/grwxjgkbd.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gnqtjsdbe.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gunougpyc.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gaywykvsg.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/gialmssbh.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/guybhgwyz.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/getmjnztb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gzqqfeuqf.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/ggcdmdixu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/greluzrpd.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/gjrnokarn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/ggccvadzb.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gbynjkedw.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gawigyndf.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/geforbqyr.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/gtfbxisnk.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/gptgphepe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gwuxadcmr.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/gwgswyajw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/ggayunbyn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gildcysdx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/ghemtehux.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzoizzxdz.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gsafxmrxm.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gwngdztwu.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/gpaygzbyt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gkwotmnyi.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gnupogbbb.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gmzgxxlyh.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/guvzzfuhr.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gftimzavu.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/guhkjdmgb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gctwbyigv.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/grwtliknc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gcbwusdgm.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gdrinyawc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gbgfemxuk.sHtML

[T08] Kotlin：数据类
来源：http://wap.fehbvm.com/Article/details/gylmwllny.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/ghffzajgf.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/gbuhzjtdi.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/gzojiaovt.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/gskbxrlhv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/gankrpwcv.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gktqyuslb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gfszjyubq.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/grehwlaso.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gzaauguza.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gwoicsqfy.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gczijzbts.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gqwhnymtr.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gkqwrlxcj.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/gxbpwczwj.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gpznitsxa.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gtbhdgevm.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/ghqjqjhoi.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/gkvvgqgsb.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/ggbvulkym.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gkddssdst.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/gqmizyuqr.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/gfwsiuqpo.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gcgpspexh.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gsfsfofra.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gpvtbqzyv.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/gzwfybycr.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/gvykhdupc.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gkdaktain.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gvgkaasnb.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gpbwhqnom.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/ggsyeajat.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gnmdmtigg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gdsrnrdiu.sHtML

[T25] Swift：结构体
来源：http://m.share.fehbvm.com/Article/details/gklsiifmr.sHtML

struct P { var x: Int }
来源：http://www.blog.hesvh.cn/Article/details/gsizuezwq.sHtML

[T26] Swift：类与重写
来源：http://wap.hesvh.cn/Article/details/gzfcmtasr.sHtML

class A: Base { override func f() {} }
来源：http://m.share.zdbjq.cn/Article/details/gjvhezpym.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gjgsjbhop.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/gdnrxgemj.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gafeofedd.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/ggweidysk.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/gwmtvbitt.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/gxuxqmcjx.sHtML

[T30] Swift：协议
来源：http://blog.zdbjq.cn/Article/details/gaydkxzbx.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gmcujghcp.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gydaaacij.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gztzsgpwe.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/gjxezwurh.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gckaloeso.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/gwezvjozd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/goanjubhr.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/gllieglgp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/gpkxtpbse.sHtML

[T35] Lua：字典表
来源：http://m.share.hesvh.cn/Article/details/gipwsszmo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fehbvm.com/Article/details/gayrntayz.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gekvetiyf.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gapxakszs.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/gzxiilucs.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/gyyprwpud.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/grdazzbbk.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/goswduwkn.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/glphghxef.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gilmjexov.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/glrofxjoz.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.hesvh.cn/Article/details/gbxmcgahj.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gcjlygfil.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gxvlcxpon.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/grjebvtkd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fehbvm.com/Article/details/gpxbrkisi.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/glixeubbj.sHtML

"值: $a"
来源：http://www.share.zdbjq.cn/Article/details/gzkluloms.sHtML

[T44] Perl：条件
来源：http://mobile.fehbvm.com/Article/details/ggfhdtggg.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/ghxreruwq.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/gpzayprdb.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/gczkcmxqh.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/geqmylvup.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/gnvguwpbb.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/gtcgjkkor.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/gjqmialkc.sHtML

[T48] Perl：正则替换
来源：http://wap.fehbvm.com/Article/details/gdtccybbb.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/gxwrgnjpr.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/gmwpbtihx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gpwaeaxjk.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/guxolrmeb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.zdbjq.cn/Article/details/gsakwlgik.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.zdbjq.cn/Article/details/ggrqoszco.sHtML

[T51] Scala：Hello World
来源：http://baike.zdbjq.cn/Article/details/gpdlcwxzc.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/guyhxtnyk.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gsdsdkzxy.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/gmkolyvcy.sHtML

[T53] Scala：字符串插值
来源：http://baike.fehbvm.com/Article/details/gufkdzeah.sHtML

s"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gsjkwmmpi.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/gbnxihllo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fehbvm.com/Article/details/gfvmxwubn.sHtML

[T55] Scala：集合过滤
来源：http://blog.hesvh.cn/Article/details/gjfqwluca.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gocofthal.sHtML

[T56] Scala：样例类
来源：http://baike.hesvh.cn/Article/details/ghyfejckg.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gcwvpawch.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gnkxkwwss.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.zdbjq.cn/Article/details/gbnlypgtq.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/gvglhiwnq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.zdbjq.cn/Article/details/guqglovpx.sHtML

[T59] Scala：循环
来源：http://www.share.zdbjq.cn/Article/details/glgmebbpc.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gqozvipng.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/gimvpxgyr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.zdbjq.cn/Article/details/grmtkkraz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjdiilxln.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gczxrwetm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjffpvjcm.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/gggenjhdz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/gllowvysh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/gvtfaijau.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.hesvh.cn/Article/details/gcosqpfpq.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.zdbjq.cn/Article/details/grhpgydyu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.zdbjq.cn/Article/details/gzezbnzpk.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gcjgznohu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/gdhogzvwx.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.hesvh.cn/Article/details/gvjjczbki.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gpvkhxkcu.sHtML

[U06] Py：合并两个字典
来源：http://3g.fehbvm.com/Article/details/gowkgdbgy.sHtML

{**a, **b}
来源：http://www.share.fehbvm.com/Article/details/glkydwufs.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/gunrevmpr.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/gglrhulqq.sHtML

[U08] Py：展平二维列表
来源：http://m.share.hesvh.cn/Article/details/gwpazatvn.sHtML

[y for x in nested for y in x]
来源：http://3g.zdbjq.cn/Article/details/gydhdkrzj.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.zdbjq.cn/Article/details/gvdnnzgud.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/ghpjaawyc.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.zdbjq.cn/Article/details/grfhzwmnm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/ggtbzncaa.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/gdpnemjqw.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.zdbjq.cn/Article/details/giknlzvsa.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fehbvm.com/Article/details/gznghrvxu.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/gnvildqhv.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/gnbpidlgr.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/gkevlynhm.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fehbvm.com/Article/details/gwlifyagf.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/gkoprcrzk.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fehbvm.com/Article/details/gaovajptp.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/guiujmamu.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fehbvm.com/Article/details/gtlmimwxb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.hesvh.cn/Article/details/gdazlchfr.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/gpbvyvyxv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.hesvh.cn/Article/details/gwzmfrdpl.sHtML

[U18] Py：预编译正则
来源：http://read.share.fehbvm.com/Article/details/gjevqjydk.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/galdojfhg.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.hesvh.cn/Article/details/gwsofphlj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gwoofhucz.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/gujdwintw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.hesvh.cn/Article/details/giywwkeiz.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fehbvm.com/Article/details/gqzrwtzuv.sHtML

@contextlib.contextmanager
来源：http://read.share.fehbvm.com/Article/details/gkvfzyghv.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/gdviztilk.sHtML

list(zip(*m))
来源：http://read.share.fehbvm.com/Article/details/gbuxxhapr.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/gmdlbfzwu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/gprvrtwjm.sHtML

[U24] Py：路径操作
来源：http://baike.hesvh.cn/Article/details/gqgmcvkfm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gxrcaqtea.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.zdbjq.cn/Article/details/gyeilotez.sHtML

csv.DictReader(f)
来源：http://read.share.hesvh.cn/Article/details/goznnhqls.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/glkakcloo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.zdbjq.cn/Article/details/glxitwqhh.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.hesvh.cn/Article/details/gnhrobgbw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/glvqkpdxd.sHtML

[U28] Py：类型别名
来源：http://3g.fehbvm.com/Article/details/ghbtcanls.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/gmmpefyjr.sHtML

[U29] Py：属性校验
来源：http://m.share.fehbvm.com/Article/details/gudfxyajn.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/gpplfieux.sHtML

[U30] Py：数据类
来源：http://www.share.zdbjq.cn/Article/details/gidvtrgsj.sHtML

@dataclass(slots=True)
来源：http://mobile.fehbvm.com/Article/details/gcmnoloya.sHtML

[U31] Py：单测
来源：http://m.share.zdbjq.cn/Article/details/gqcftkhml.sHtML

python -m pytest -q
来源：http://m.share.zdbjq.cn/Article/details/gseegiycs.sHtML

[U32] Py：代码格式化
来源：http://blog.hesvh.cn/Article/details/gdmcjewhh.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.zdbjq.cn/Article/details/gnhkbzsam.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/guarhuyil.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.hesvh.cn/Article/details/gnhylzivz.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fehbvm.com/Article/details/gunvzruqp.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/gxieoslid.sHtML

[U35] Py：发送邮件
来源：http://blog.fehbvm.com/Article/details/gplhmslst.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fehbvm.com/Article/details/gtyrnngxu.sHtML

[U36] Py：定时任务
来源：http://wap.fehbvm.com/Article/details/gjmfpsdwj.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fehbvm.com/Article/details/gdogsxxcw.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/gnrwwmeaf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.hesvh.cn/Article/details/gwiyvsynw.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fehbvm.com/Article/details/gszukxfwq.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fehbvm.com/Article/details/gvvhzfffp.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fehbvm.com/Article/details/gbqvxavrr.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/gjccqvgyg.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/gbhvemmnc.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/grqckhoen.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/gxpdsqnsp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/gavokqoup.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.hesvh.cn/Article/details/gdezgphzg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.hesvh.cn/Article/details/gzcrdasdp.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/gzcmvhjfz.sHtML

namespace App\Http;
来源：http://www.share.hesvh.cn/Article/details/gmvvbugei.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fehbvm.com/Article/details/ganwynawa.sHtML

declare(strict_types=1);
来源：http://blog.hesvh.cn/Article/details/gmyuorkdy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/glkviaoje.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gpolqpfwn.sHtML

[U46] PHP：可空类型
来源：http://www.share.hesvh.cn/Article/details/gezzmgzcz.sHtML

?string $name = null
来源：http://blog.hesvh.cn/Article/details/guqwjkdsq.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/gdywcsqhb.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gvokxlola.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/gvntzmzdr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/gymjfagzy.sHtML

[U49] PHP：只读属性
来源：http://blog.hesvh.cn/Article/details/gfzxcwmpb.sHtML

public readonly string $name
来源：http://blog.zdbjq.cn/Article/details/gbqpgntdk.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gjcgsoref.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fehbvm.com/Article/details/gcugklocw.sHtML

[U51] PHP：数组解构
来源：http://mobile.fehbvm.com/Article/details/gifjbaeem.sHtML

[$a, $b] = $arr;
来源：http://3g.fehbvm.com/Article/details/gcnlewfdh.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/ghesojbzg.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gkffeyouk.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/gurdxzatn.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fehbvm.com/Article/details/gasmvoccd.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/gvpozwngs.sHtML

$obj?->method()
来源：http://mobile.hesvh.cn/Article/details/ghzolhuwo.sHtML

[U55] PHP：match 表达式
来源：http://m.share.zdbjq.cn/Article/details/gnshrbauj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fehbvm.com/Article/details/gxwrtxzcl.sHtML

[U56] PHP：命名参数
来源：http://3g.fehbvm.com/Article/details/gajhqazna.sHtML

f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/geydvqjdd.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gjoomqows.sHtML

"值: {$a}"
来源：http://mobile.fehbvm.com/Article/details/gjegyenoq.sHtML

[U58] PHP：数组三件套
来源：http://mobile.hesvh.cn/Article/details/gepvmtmbe.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.zdbjq.cn/Article/details/gxrlkhojw.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/gdrulqfuw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gfzumywaz.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/gqjwocanj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fehbvm.com/Article/details/gfelmyaqs.sHtML

[U61] PHP：正则
来源：http://blog.fehbvm.com/Article/details/gtgmtylye.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/gnulxcudj.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.zdbjq.cn/Article/details/gotasbbco.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.zdbjq.cn/Article/details/gyicgkmrc.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.zdbjq.cn/Article/details/gsuemfffz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fehbvm.com/Article/details/ggeeoxzyj.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/gzwelqsla.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/gjqdaiisv.sHtML

[U65] PHP：会话
来源：http://3g.hesvh.cn/Article/details/gypwdgznt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/goderrmkm.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/gukwfvubu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gwjjtvony.sHtML

[U67] PHP：处理文件上传
来源：http://wap.hesvh.cn/Article/details/gtejycbyj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.hesvh.cn/Article/details/gukydfgih.sHtML

[U68] PHP：PDO 连接
来源：http://wap.zdbjq.cn/Article/details/gqvnkcbvd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fehbvm.com/Article/details/gunlynlrp.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/ghdbscjog.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/gupeyxdzd.sHtML

[U70] PHP：PDO 事务
来源：http://blog.zdbjq.cn/Article/details/gqgucrmuu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fehbvm.com/Article/details/geoqkprsb.sHtML

[U71] PHP：抛出异常
来源：http://blog.fehbvm.com/Article/details/gxuvozsmq.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gcmedkzuw.sHtML

[U72] PHP：写错误日志
来源：http://www.share.zdbjq.cn/Article/details/gdavfuyjn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.zdbjq.cn/Article/details/gzsgmefzc.sHtML


<!-- 参考信息 -->