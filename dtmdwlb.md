代发 wailian999

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gvwjisnbg.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/gypxvgimw.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/gkqokolhb.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/ggwiqejfc.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/gcfmkoijt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gvgbyljdn.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/ghyjdugbo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/guwdwpikx.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gdjaploqs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/gvpdurqmr.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gwlzlqtrf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gfaqlfzgo.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gfjxnnfeh.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gmxoayjeq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gbeflxqey.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/gvnfffgsq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/glnzgbtsz.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gibyectwp.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/glklmdlce.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gebdwegby.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/gehyzadvj.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/gwugdnmys.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.zdbjq.cn/Article/details/gvzkyletr.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gdroplzoy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gwvrbkguc.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gtbqziebo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gckuidhcn.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/grtbljkja.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gxacwidrt.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/godpuftwo.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gvrninvhu.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gyhkxwnuz.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gmlkvbbuq.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/grtemyrfm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/gdcdyxmwc.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/ghvmoyhwy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gdflrygbn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grjottmou.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gwzbwltjw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwrodjqem.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gzusxkyrw.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/ggrrauxlq.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gvymgsyrr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gvcdsxbsr.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/gzhjeeleh.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gicegedfa.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/gtrznjnuf.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/ggnpfvefu.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/gdybxnqtf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/grmmhvljd.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gilahsxyg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gkrrkxkpx.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gqxtzbgar.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gxsistqoy.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/gnvjkohgf.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/ggthluvsx.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gdmibqpoe.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gpqqvflhm.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/gzkawfriz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gctzdvdlw.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gblzrwxbv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gvbmskvwe.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/ggosycjwm.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gdiykrsxs.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/gysxnkccu.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gowvqntyn.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/gbwzcyvec.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gejenndjn.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gfvasmayh.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gbnlccgeo.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gafsqjmjp.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gryiukgxu.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gtdkawute.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gsxsivvwo.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gidluhcpa.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gikjwkjdx.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/gwnhkshml.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gquuheosd.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/guadmqpzp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/ggwbagusa.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/gpyaayvuu.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/glsvvwjyt.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gknlhvbjf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/glxyeyskp.sHtML

[T23] Swift：函数
来源：http://read.share.hesvh.cn/Article/details/gfhagyhee.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/glxutterr.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/gxybdbcwt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gldxsyayi.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gwociyanq.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/ghhptrwpf.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/gnjzdhemz.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/gdzusbpyn.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gzigdnhyb.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.hesvh.cn/Article/details/gcqwovlcz.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gfwrrvfco.sHtML

enum Color { case red, green }
来源：http://3g.hesvh.cn/Article/details/ghtxcrizr.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.zdbjq.cn/Article/details/gdgouhozh.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gzauxpata.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/grymzuoeq.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.hesvh.cn/Article/details/giclstzex.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gsmectkqo.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/ghoipuymz.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/glcfzthjt.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/gmwqvstvo.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/gemovhmfg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/ggwvsoykb.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/gegojqjrv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/ghttigfbh.sHtML

[T35] Lua：字典表
来源：http://wap.zdbjq.cn/Article/details/ghvctfigm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/gyyxqdyzp.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gnjqfpdjq.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gufycvtlt.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gywkkphrq.sHtML

"a" .. "b"
来源：http://www.m.share.hesvh.cn/Article/details/gloqqgvmu.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/grdosnpqf.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gkxrorfci.sHtML

[T39] Lua：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/giewllurn.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/gebzlykzr.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/gcobbvkwt.sHtML

setmetatable({}, { __index = base })
来源：http://wap.zdbjq.cn/Article/details/gltthidch.sHtML

[T41] Perl：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gdfxqruef.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gfslyfqux.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gniwlfwbr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/gbwoklopc.sHtML

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/giihnekiq.sHtML

"值: $a"
来源：http://www.blog.hesvh.cn/Article/details/gaqtoqxdr.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gwjzqxpwk.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/geyszzagj.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/gpfkcevmu.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/gclcxcayl.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/gbhhmjsyu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.hesvh.cn/Article/details/gnbjcephq.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/gdbdksfmt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fehbvm.com/Article/details/gqdgidnee.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/grdvgtppr.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/gdkdzykbv.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/gtuunavmz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gbcboukyy.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gfkpcqpex.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/gunhxrvqn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.hesvh.cn/Article/details/ggdsewvjq.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gvtxfgzaq.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gybzdcisk.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/gxmkeisoc.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/gzwfisuax.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gtvmkigrb.sHtML

s"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/ghmjyacfd.sHtML

[T54] Scala：集合映射
来源：http://baike.hesvh.cn/Article/details/gqpbnwwhf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gwwwreiea.sHtML

[T55] Scala：集合过滤
来源：http://baike.fehbvm.com/Article/details/gapqqlocr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gszkmkzxr.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/ganzoxpou.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gsemsrfrd.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/giervjxcj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gligddqst.sHtML

[T58] Scala：函数定义
来源：http://wap.zdbjq.cn/Article/details/ggaerofto.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/glrjklpfb.sHtML

[T59] Scala：循环
来源：http://baike.fehbvm.com/Article/details/gdefdgrss.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gyrfmktys.sHtML

[T60] Scala：折叠
来源：http://blog.zdbjq.cn/Article/details/gcntgsxec.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/gxwlqfghz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gycfcottw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/gjoxlkdnx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdlslziry.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/gblhverbo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/gjiooruql.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/ghclrqlyn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.hesvh.cn/Article/details/gfflckyyc.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/gbfgixxqw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/gdgmetpwr.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gezttmros.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.zdbjq.cn/Article/details/gxtmgxqxs.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/gxvuxmqwy.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gcbkahnkw.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/gcgobcedy.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/gzkxukzvp.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/govwfdfdw.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/giwdbwqqd.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fehbvm.com/Article/details/gustdzdtw.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/gahnuzqjc.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gufxrhdbh.sHtML

max(d, key=d.get)
来源：http://www.share.fehbvm.com/Article/details/gnsakeisj.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/gsowsriyy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.zdbjq.cn/Article/details/gjrezajyo.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/gssjxlizt.sHtML

(x * 2 for x in arr)
来源：http://read.share.zdbjq.cn/Article/details/gbuqnqpls.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gzuwfjnzg.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/gaogrcicl.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/gnsbhinay.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/gjnfqneqq.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gxuydtxhn.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gayoilyow.sHtML

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/gppbasfng.sHtML

t = time.perf_counter()
来源：http://wap.hesvh.cn/Article/details/gxtbiycco.sHtML

[U16] Py：命令行参数解析
来源：http://3g.zdbjq.cn/Article/details/glzhykrll.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/ggdejptmy.sHtML

[U17] Py：初始化日志
来源：http://blog.fehbvm.com/Article/details/gkmfsnfqn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gbhmmzvip.sHtML

[U18] Py：预编译正则
来源：http://wap.hesvh.cn/Article/details/glhexsscm.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/grzewgdps.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/gxwurzkgb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.zdbjq.cn/Article/details/gitylzaat.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/gcakezgrm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.hesvh.cn/Article/details/gtjwuwlog.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fehbvm.com/Article/details/gyyiigafa.sHtML

@contextlib.contextmanager
来源：http://m.share.hesvh.cn/Article/details/gepfzesay.sHtML

[U22] Py：矩阵转置
来源：http://mobile.zdbjq.cn/Article/details/gahghkpdr.sHtML

list(zip(*m))
来源：http://www.share.fehbvm.com/Article/details/glofmsoyl.sHtML

[U23] Py：分块读取大文件
来源：http://wap.hesvh.cn/Article/details/gybnjwwmo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.zdbjq.cn/Article/details/gezuznojl.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/gkzasuari.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gigiglgwa.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.hesvh.cn/Article/details/gvytadmue.sHtML

csv.DictReader(f)
来源：http://www.blog.zdbjq.cn/Article/details/gdzpvlkfi.sHtML

[U26] Py：并发下载
来源：http://read.share.hesvh.cn/Article/details/gbjihsbdf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.hesvh.cn/Article/details/gcclnosnv.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/gcwgjqmkf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.zdbjq.cn/Article/details/gyiunaqgx.sHtML

[U28] Py：类型别名
来源：http://www.blog.zdbjq.cn/Article/details/gzuakscdr.sHtML

UserId = int
来源：http://www.share.fehbvm.com/Article/details/griohemlr.sHtML

[U29] Py：属性校验
来源：http://3g.hesvh.cn/Article/details/gbfjwzgfi.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/gsevdvcfk.sHtML

[U30] Py：数据类
来源：http://www.share.zdbjq.cn/Article/details/gyglmuhoa.sHtML

@dataclass(slots=True)
来源：http://wap.hesvh.cn/Article/details/gxhuyksua.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/gitcegxme.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/gejmigcxo.sHtML

[U32] Py：代码格式化
来源：http://3g.fehbvm.com/Article/details/glzalazcm.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.hesvh.cn/Article/details/gmqwqluil.sHtML

[U33] Py：打包发布
来源：http://baike.zdbjq.cn/Article/details/gailzzctc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.hesvh.cn/Article/details/gxkiodpqj.sHtML

[U34] Py：判断编码
来源：http://m.share.fehbvm.com/Article/details/gigrgresh.sHtML

chardet.detect(raw)
来源：http://www.m.share.fehbvm.com/Article/details/gjulyghky.sHtML

[U35] Py：发送邮件
来源：http://blog.hesvh.cn/Article/details/gvehmdhqi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.zdbjq.cn/Article/details/gbdozyvqy.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/gdlklnqqs.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/gijdagdpr.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fehbvm.com/Article/details/gjkehmhjz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.hesvh.cn/Article/details/ghvvtndqc.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.zdbjq.cn/Article/details/gkpqmjdss.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/gskvyzwsv.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.hesvh.cn/Article/details/gckfchvrl.sHtML

sys.stdout.isatty()
来源：http://www.share.zdbjq.cn/Article/details/gnjtdjpzg.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/gnlabujbk.sHtML

print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/guqpfehai.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gmiydwgmh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.zdbjq.cn/Article/details/glbgtuqwa.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/gaafcmvfk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.zdbjq.cn/Article/details/gpcnepfjo.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.zdbjq.cn/Article/details/gactlkglw.sHtML

namespace App\Http;
来源：http://read.share.zdbjq.cn/Article/details/gkkhcvmkt.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fehbvm.com/Article/details/gjlzvwaht.sHtML

declare(strict_types=1);
来源：http://www.m.share.fehbvm.com/Article/details/gaqnttobp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.zdbjq.cn/Article/details/gdnclhkgd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gwkybcwnd.sHtML

[U46] PHP：可空类型
来源：http://mobile.hesvh.cn/Article/details/gvwugjxbc.sHtML

?string $name = null
来源：http://wap.hesvh.cn/Article/details/ggzsmmxzn.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/gtstqjjsm.sHtML

int|string $id
来源：http://m.share.zdbjq.cn/Article/details/gadiqvlzx.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gapryxytz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fehbvm.com/Article/details/gkuklucwu.sHtML

[U49] PHP：只读属性
来源：http://mobile.fehbvm.com/Article/details/ggyuwcvrp.sHtML

public readonly string $name
来源：http://www.share.zdbjq.cn/Article/details/ghsukueuw.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fehbvm.com/Article/details/gchbllwlf.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/gukgwfqhn.sHtML

[U51] PHP：数组解构
来源：http://baike.fehbvm.com/Article/details/gxnjxlhbm.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/gqekjtzxf.sHtML

[U52] PHP：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gpjzclnxx.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fehbvm.com/Article/details/gdgnpmlty.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gfcrrktrb.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/gncbvmltw.sHtML

[U54] PHP：空安全调用
来源：http://3g.fehbvm.com/Article/details/gqblafcnh.sHtML

$obj?->method()
来源：http://m.share.fehbvm.com/Article/details/gwmlcyinc.sHtML

[U55] PHP：match 表达式
来源：http://baike.fehbvm.com/Article/details/gizyohble.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.zdbjq.cn/Article/details/grtoujvhe.sHtML

[U56] PHP：命名参数
来源：http://3g.hesvh.cn/Article/details/gfgtbutrx.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gcoesjcba.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gmrqhxecl.sHtML

"值: {$a}"
来源：http://m.share.hesvh.cn/Article/details/gymxitnpc.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fehbvm.com/Article/details/gqiqimhyq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.hesvh.cn/Article/details/gktxukwwa.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/ggfczevip.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gvbolwubl.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.hesvh.cn/Article/details/gshkqagze.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.zdbjq.cn/Article/details/gnutnqknp.sHtML

[U61] PHP：正则
来源：http://wap.fehbvm.com/Article/details/gwsaleaek.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gxunmrdsc.sHtML

[U62] PHP：日期对象
来源：http://read.share.hesvh.cn/Article/details/gkbflgzyf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/gfkroiiwj.sHtML

[U63] PHP：文件读写
来源：http://blog.hesvh.cn/Article/details/gnlksjfjr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fehbvm.com/Article/details/giljxmccf.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fehbvm.com/Article/details/gsmphtkgq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fehbvm.com/Article/details/gcmhlrbwt.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/gegevmqtq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.hesvh.cn/Article/details/gzupugdqu.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.hesvh.cn/Article/details/gedpymhxx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fehbvm.com/Article/details/gliuiwlno.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fehbvm.com/Article/details/ghloiilmw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.zdbjq.cn/Article/details/gchsjhiko.sHtML

[U68] PHP：PDO 连接
来源：http://baike.zdbjq.cn/Article/details/gbgtdchbr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/gftlwzxtm.sHtML


<!-- 参考信息 -->