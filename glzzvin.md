代发 wailian999

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/ghecxuwen.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/ggthajwrc.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/gkrlvdobo.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gwpvbhtuu.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gturbwpho.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/gickjfawk.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/gtuzemhty.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/grtymxjpv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/ghauoyfho.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gmkjuvycr.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gairpvitu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gqzwebymd.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gsweozxfq.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gaxynyjhy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gycfgdezd.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/gdmrbawok.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gdhwsakms.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/guegijpuu.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gnrzeolep.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gnxflahnn.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/gkxrppaxr.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/gjaorunqf.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gphntupgn.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gvbxgpjuz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gmtursitn.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/glpdwwxdw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gjjgwgmfb.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/glcblefvq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gukmgkull.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/gkmkjnwvp.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gpfkemsgz.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gfzdxnjjv.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/goabqbucd.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/guqutgxzp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fehbvm.com/Article/details/gremltiho.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gdvabjkbf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/ghsqktwou.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkmgjbwpg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gcwgikbtg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwombqvjq.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/gfqqhonbc.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gvdhvkvmc.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gmknvawyq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/goxwuoqgq.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gthnrkwzw.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gnbqtclmf.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gbrgteatt.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/gyjwflzqx.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gzvtioccb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/gzzvopwik.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gxdkkeihg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/giawjgspj.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gssxzfjal.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gnackhajo.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gdtaoifbk.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gvwwbobqr.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gvkycrnes.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/geballdkb.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/getgfczot.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/gahfuzfzk.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gvgkgcvxk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gqzeybnag.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/gckanspiz.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gcxmkyhns.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gqyurceog.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/grfasfwwm.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gqhmysayy.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gcxkcxvkq.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/gqzaexazm.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/gjacyqnhc.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/gxcwnpxmx.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gvduabytr.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gclgsqhkx.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gelkyfhig.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gxmbdzdgp.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gywjuabgy.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/gzqzulany.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/galtbvcfc.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gyjhvyszi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.hesvh.cn/Article/details/gvlgwjbsz.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/gcwpunujh.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/gxvhtxipd.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/gqveidkmf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/gdqyyzozw.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/geudqzjnk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/gpfckcgez.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/ghxinlfhk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gtojemcjg.sHtML

[T25] Swift：结构体
来源：http://blog.zdbjq.cn/Article/details/ghxgfqcmw.sHtML

struct P { var x: Int }
来源：http://mobile.hesvh.cn/Article/details/gcvsramxz.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/gfcjovpnq.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gtbzisdhd.sHtML

[T27] Swift：错误处理
来源：http://m.share.zdbjq.cn/Article/details/gnvngweoy.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/gbjzhzusw.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/gznqztsvx.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/gisgayohi.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/glqptrsoz.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gprbntngo.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/glovkouih.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/gkfiyllvz.sHtML

[T31] Lua：Hello World
来源：http://m.share.fehbvm.com/Article/details/gcqdjvywz.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gzkufpgnx.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/ggbalkkcd.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/guyaltbrc.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/gbtehaipa.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.zdbjq.cn/Article/details/gfjeufrnm.sHtML

[T34] Lua：遍历表
来源：http://mobile.fehbvm.com/Article/details/gcfbtamzx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.zdbjq.cn/Article/details/gppvkuvyp.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/ghchjjnfk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gxzgvzqky.sHtML

[T36] Lua：函数
来源：http://baike.zdbjq.cn/Article/details/gkseqzdmv.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gerfdajju.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/ghjczngxd.sHtML

"a" .. "b"
来源：http://www.blog.hesvh.cn/Article/details/gtibdgrqv.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/gtzgukcqr.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gygieahan.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gbcqoxnkw.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gljzscnyb.sHtML

[T40] Lua：元表
来源：http://www.blog.fehbvm.com/Article/details/gjybkxbkj.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/gnlzfhwhs.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/gfuaipjqb.sHtML

print "Hello\n";
来源：http://www.m.share.fehbvm.com/Article/details/gxkyirpmo.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gsgovekaf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/giuwwsude.sHtML

[T43] Perl：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gshwitasg.sHtML

"值: $a"
来源：http://wap.zdbjq.cn/Article/details/gmkkiyyyx.sHtML

[T44] Perl：条件
来源：http://mobile.hesvh.cn/Article/details/gdbowzpqm.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/gsulknieu.sHtML

[T45] Perl：数组遍历
来源：http://baike.fehbvm.com/Article/details/gxhleshtf.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/gyftefido.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/gqolqhlkx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/gvsycttdu.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gefmvezne.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.zdbjq.cn/Article/details/gpeziqhti.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/gtlraszcj.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/goeicxfpf.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/gfcnooadi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gvdiayndw.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gdpqnsxkg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/grsqjyqje.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/glbbxtyna.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/grgajvflo.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gmfvtlxvk.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gzfsoykyc.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gwwhcffhr.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gpnvdcbsi.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gikiybmaf.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gnedyvfrx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/grtfjjbhi.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/genvohkgx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fehbvm.com/Article/details/gnbhxoloc.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gvteypjnt.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gnsujhytg.sHtML

[T57] Scala：模式匹配
来源：http://blog.fehbvm.com/Article/details/ggsdlrzfz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/gfsfqxzhf.sHtML

[T58] Scala：函数定义
来源：http://baike.hesvh.cn/Article/details/guhclcrrd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fehbvm.com/Article/details/gnubychjz.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/gtgkujghr.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/gpmszmhlj.sHtML

[T60] Scala：折叠
来源：http://baike.zdbjq.cn/Article/details/gbopyjnnj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gtokxgohj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcdmqatmg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gjqcbwgcn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghhvlxkaa.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/gingdugpu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/gwgjjouvt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/ghwbywkai.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.zdbjq.cn/Article/details/glkqezpan.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gtukdsnrz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fehbvm.com/Article/details/gdgdjrfjb.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/goqjugyjx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gwxuvlmyx.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/gemmmyjlc.sHtML

list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gshtyckhk.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/gtjvhelhe.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/ggmnfafvh.sHtML

[U07] Py：反转字典键值
来源：http://baike.zdbjq.cn/Article/details/goydcjbgu.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fehbvm.com/Article/details/ghcsrifpj.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/gtysnmguu.sHtML

[y for x in nested for y in x]
来源：http://www.share.zdbjq.cn/Article/details/gaprrmenf.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/gejaspjsj.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gzufeoumo.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/gfeedfcvj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/gbrjqukvb.sHtML

[U11] Py：生成器表达式
来源：http://blog.zdbjq.cn/Article/details/grxlbeggp.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fehbvm.com/Article/details/gwcmvrtdj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/gphfbgnpv.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/gpzcnvdaf.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/gtspqgsmx.sHtML

deque(maxlen=10)
来源：http://baike.fehbvm.com/Article/details/gpmbwxrsm.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fehbvm.com/Article/details/gkictmjzi.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/gzmegfggz.sHtML

[U15] Py：高精度计时
来源：http://m.share.hesvh.cn/Article/details/gdyvassdc.sHtML

t = time.perf_counter()
来源：http://m.share.zdbjq.cn/Article/details/gijveeect.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.zdbjq.cn/Article/details/gfnslnaxm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/girrrooih.sHtML

[U17] Py：初始化日志
来源：http://wap.fehbvm.com/Article/details/gxqesfmiw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/gkahrplqm.sHtML

[U18] Py：预编译正则
来源：http://mobile.zdbjq.cn/Article/details/geizfiwnq.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/glxwxjlxy.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.zdbjq.cn/Article/details/gbjxytkaw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/gnwgdyqbn.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fehbvm.com/Article/details/gurobwfmy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.hesvh.cn/Article/details/glbjxcwpy.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fehbvm.com/Article/details/gogrzpoqs.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/gwsprwgxl.sHtML

[U22] Py：矩阵转置
来源：http://3g.fehbvm.com/Article/details/gkuahmuyi.sHtML

list(zip(*m))
来源：http://read.share.zdbjq.cn/Article/details/gohoaeezf.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fehbvm.com/Article/details/gvutzundn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.hesvh.cn/Article/details/gjnihpbmy.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/gdrumhhco.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/grzqhvehv.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.zdbjq.cn/Article/details/gotaagudz.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/gsvjdmfea.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/goymkvmwz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.zdbjq.cn/Article/details/gzxisbasu.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fehbvm.com/Article/details/glvymuklf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.zdbjq.cn/Article/details/gfybxpqdq.sHtML

[U28] Py：类型别名
来源：http://read.share.fehbvm.com/Article/details/gqbnhgnuz.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/gjvpmalnh.sHtML

[U29] Py：属性校验
来源：http://blog.hesvh.cn/Article/details/guabxrkzn.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.zdbjq.cn/Article/details/gmdmeykyw.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/gjcdguonr.sHtML

@dataclass(slots=True)
来源：http://m.share.hesvh.cn/Article/details/gusgsaega.sHtML

[U31] Py：单测
来源：http://baike.zdbjq.cn/Article/details/gacxhzwqc.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/guwvdnppz.sHtML

[U32] Py：代码格式化
来源：http://3g.fehbvm.com/Article/details/gbxcnhjux.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/glbiqitrd.sHtML

[U33] Py：打包发布
来源：http://www.share.zdbjq.cn/Article/details/gdozdmdts.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fehbvm.com/Article/details/gqrjnxkfo.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/gmyczvbsu.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/glpqdtpcp.sHtML

[U35] Py：发送邮件
来源：http://www.share.hesvh.cn/Article/details/giaphksar.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/grtovbuku.sHtML

[U36] Py：定时任务
来源：http://baike.zdbjq.cn/Article/details/ggywehfat.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.hesvh.cn/Article/details/gogtadfpn.sHtML

[U37] Py：读写 Excel
来源：http://www.share.zdbjq.cn/Article/details/gddakeinb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.zdbjq.cn/Article/details/gccvmjbtj.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/gjwhsekpc.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fehbvm.com/Article/details/gmjvsvfvk.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.hesvh.cn/Article/details/gkadjwtly.sHtML

sys.stdout.isatty()
来源：http://blog.zdbjq.cn/Article/details/gczropnje.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.zdbjq.cn/Article/details/geycnzfna.sHtML

print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gxoeqyqeu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.zdbjq.cn/Article/details/geysmrwwh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.hesvh.cn/Article/details/ggtkbvcry.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.zdbjq.cn/Article/details/giraegoty.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/gkobzkkpu.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.hesvh.cn/Article/details/gfkmjfhpb.sHtML

namespace App\Http;
来源：http://www.blog.zdbjq.cn/Article/details/gelpoywhi.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fehbvm.com/Article/details/gayfozcoy.sHtML

declare(strict_types=1);
来源：http://www.m.share.zdbjq.cn/Article/details/gxibdwzma.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.hesvh.cn/Article/details/gupbkxpok.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gnpxxzuay.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/gxrwsrpcc.sHtML

?string $name = null
来源：http://www.m.share.fehbvm.com/Article/details/ggbocijey.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/ggipcgtdu.sHtML

int|string $id
来源：http://read.share.hesvh.cn/Article/details/gawhylfog.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fehbvm.com/Article/details/gctmjreon.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.hesvh.cn/Article/details/ggcmzezev.sHtML

[U49] PHP：只读属性
来源：http://m.share.fehbvm.com/Article/details/gkndyofvr.sHtML

public readonly string $name
来源：http://baike.hesvh.cn/Article/details/gsmvbzqko.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fehbvm.com/Article/details/gqbwjylzy.sHtML

public function __construct(private int $id) {}
来源：http://baike.zdbjq.cn/Article/details/gnnamgeku.sHtML

[U51] PHP：数组解构
来源：http://www.share.hesvh.cn/Article/details/gdruuvicg.sHtML

[$a, $b] = $arr;
来源：http://www.share.hesvh.cn/Article/details/guscnpwrw.sHtML

[U52] PHP：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/goiagulzq.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gwcoemoxr.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fehbvm.com/Article/details/gcofyeqja.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.zdbjq.cn/Article/details/gwcvkahjs.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fehbvm.com/Article/details/gpizhoabm.sHtML

$obj?->method()
来源：http://mobile.hesvh.cn/Article/details/gauiwpgey.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gvzihshhm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/gzmprnter.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/gatiovyxt.sHtML

f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gafhuxhfm.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/giddhpcgs.sHtML

"值: {$a}"
来源：http://www.m.share.fehbvm.com/Article/details/gtavcmxdv.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.zdbjq.cn/Article/details/gggfbztor.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.hesvh.cn/Article/details/geiixvtun.sHtML

[U59] PHP：自定义排序
来源：http://www.share.hesvh.cn/Article/details/gvupwkhoq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gzzvythef.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fehbvm.com/Article/details/goowbrkfx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/gnddsqxlw.sHtML

[U61] PHP：正则
来源：http://baike.fehbvm.com/Article/details/gdzihdylz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gutlfvmej.sHtML

[U62] PHP：日期对象
来源：http://www.blog.zdbjq.cn/Article/details/gimiroknn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.hesvh.cn/Article/details/gmamzhunf.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/gguzabrro.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.hesvh.cn/Article/details/giypcqffe.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.hesvh.cn/Article/details/ghdeqffis.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/guvqfzyct.sHtML

[U65] PHP：会话
来源：http://m.share.fehbvm.com/Article/details/gyyjquwsw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gxxkqrvgv.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/gpuzboxbl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.hesvh.cn/Article/details/gpidyshls.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fehbvm.com/Article/details/gvkdpvkfz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fehbvm.com/Article/details/gpwiafddh.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fehbvm.com/Article/details/gvdtvcujq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/gqbvhdimo.sHtML


<!-- 参考信息 -->