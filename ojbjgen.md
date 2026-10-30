代发 wailian999

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gysnpfisj.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gubepcziu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gzmsgaege.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvtgkikv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkevjkvlk.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcogzton.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gondslxue.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gmttadaag.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gposknqxa.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gowgizkdu.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnkfayuf.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmxjyftp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geofyrjoz.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gdvqkynlb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gblkgodlv.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzktyxodf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrxhltvr.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/ggpbvulmn.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gxzodtjzh.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gvaumsjop.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/ggysqoanu.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gktxmwkwh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/grymiahms.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/guzdqanrw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/grvdmyeey.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gbeaypqmd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfupbjvx.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gprujcqvf.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gpdiqdsmk.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/glrtpwiyo.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gcnunmedo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gqlpsziji.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gqivnpdof.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqixfxtem.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gwobahdkw.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpephciw.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwfioxjv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwmgeywm.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gkozoehog.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabdvjstv.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdfhfhrb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvxxrwjw.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbqhrogl.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghinopkei.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfskyzaq.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/glhzoxdph.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcykpkfe.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkogqzbrd.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwynsyvf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvjkerql.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspvzbdpn.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gjtbsvain.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gipkknqph.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/glmsiynla.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxemttjtg.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqegmnatg.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gsxykyfzv.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gapmxumcd.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gxaqzofuj.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gbjraxkvc.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemkyyqfi.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/giswvmowx.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmdwsbvw.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgwsgumg.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gzggghsux.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/gdeukwrrn.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuadakhi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmatuoizf.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvhfhjyx.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gveelidhq.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvajhvzz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gbltroiri.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gurnitxya.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpljnlbe.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gvgihjkzg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gpzojwjzo.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gxiqnsqkx.sHtML

struct P { var x: Int }
来源：http://m.share.fanxiaobao.xyz/Article/details/gejjeyodr.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcubjyfh.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gknbnkyqz.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvrkzmkk.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwqcpdku.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/guokbpeaw.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyowdcrn.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gommopnxt.sHtML

guard let x = opt else { return }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghohoxoye.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gafyiidyl.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhuvtimv.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gtnejmlde.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggafeyfth.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gazwxkqay.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gqudodgja.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxltjgjch.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmgijcnw.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsboqjwc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/gxiywfznr.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrrenrpw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlojupuj.sHtML

[T36] Lua：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmcvcgsc.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbthimmw.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrwufwps.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikowlvrb.sHtML

[T38] Lua：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlusojcw.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqezvbvjo.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goaioihto.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guihvizqy.sHtML

[T40] Lua：元表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabmaugpi.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gojpukqji.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/goxxjheuc.sHtML

print "Hello\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gveanmlsq.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcntkahph.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gktsjukes.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbcddwne.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtcoigbr.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxkhkeio.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgpjcihc.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grndxecgb.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fanxiaobao.xyz/Article/details/goxrekfcs.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnbufdlt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogxkkmuu.sHtML

[T47] Perl：正则捕获
来源：http://blog.fanxiaobao.xyz/Article/details/gmdjbkbwi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/geviaobqa.sHtML

[T48] Perl：正则替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gttplcxxr.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpwfrmfv.sHtML

[T49] Perl：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlibgnjp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlnasthg.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuioxsoq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fanxiaobao.xyz/Article/details/gctnmobqo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdiwrmupd.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gwguhbski.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gpdffejes.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbgtlxlv.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gisbgunzy.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gzibxskvz.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gcgvigktm.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkdurgbp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfjxpyxk.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfwpjapv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvlzubfv.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/gfnweqpot.sHtML

case class User(name: String, age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gxxpasebq.sHtML

[T57] Scala：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gzghaesbe.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gadjndxhv.sHtML

[T58] Scala：函数定义
来源：http://m.share.fanxiaobao.xyz/Article/details/geewlnago.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvvyesbc.sHtML

[T59] Scala：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykqummms.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gemnbypdn.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimbicucm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gynemwhrg.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gknjadfxd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gzykexbrh.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gbqcfwrdh.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/gxvytwlxz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fanxiaobao.xyz/Article/details/gzkfmubqh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxtpzsgg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyjyjvqv.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktzfxnog.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfglfkuaa.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxqwajfz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fanxiaobao.xyz/Article/details/gwptvathy.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gsmrjrlbu.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvdzgsno.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfuehweb.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/gmoeztacm.sHtML

[U07] Py：反转字典键值
来源：http://blog.fanxiaobao.xyz/Article/details/gokckqyzf.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fanxiaobao.xyz/Article/details/gfuuzdcbs.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzcfukzy.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/gvpwehuhs.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpcyvtik.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/gpukqfgdq.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/gutzddigt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuvetvwt.sHtML

[U11] Py：生成器表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gkwdlfwgl.sHtML

(x * 2 for x in arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gtqjcdyvx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/grihrqfzu.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/goguufwbg.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gghzzsqor.sHtML

deque(maxlen=10)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdatwwec.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fanxiaobao.xyz/Article/details/gejldgxyi.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/gifnbaift.sHtML

[U15] Py：高精度计时
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxgrozrc.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/gcozkmwem.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fanxiaobao.xyz/Article/details/grqfetwmv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fanxiaobao.xyz/Article/details/giaxvfmls.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gegneciid.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/grralfgtj.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksxhsdwb.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gspdospje.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuygbspr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsndfxnon.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fanxiaobao.xyz/Article/details/geqdiwrvr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fanxiaobao.xyz/Article/details/geenmngoc.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fanxiaobao.xyz/Article/details/gebwkdyjw.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzuffmsl.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/gzdewabsg.sHtML

list(zip(*m))
来源：http://baike.fanxiaobao.xyz/Article/details/gtsdfznff.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyhaifvx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fanxiaobao.xyz/Article/details/gykhtkyyc.sHtML

[U24] Py：路径操作
来源：http://wap.fanxiaobao.xyz/Article/details/gelqfvrqj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltstyaxk.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fanxiaobao.xyz/Article/details/gkgoejcls.sHtML

csv.DictReader(f)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmtlvajy.sHtML

[U26] Py：并发下载
来源：http://3g.fanxiaobao.xyz/Article/details/gymgvgbwf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysglvbtr.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fanxiaobao.xyz/Article/details/gswbtfcdp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fanxiaobao.xyz/Article/details/gxnyvklki.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/glgsemlaf.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/gkbjeeiea.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrmlnaze.sHtML

@property 与 @x.setter 配合
来源：http://wap.fanxiaobao.xyz/Article/details/gfssjapyv.sHtML

[U30] Py：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gtrxhhekj.sHtML

@dataclass(slots=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gurlmsluz.sHtML

[U31] Py：单测
来源：http://wap.fanxiaobao.xyz/Article/details/gnsjwvopj.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/gdftomuzw.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gawyjkdxe.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fanxiaobao.xyz/Article/details/gqagtwpjp.sHtML

[U33] Py：打包发布
来源：http://www.share.fanxiaobao.xyz/Article/details/gzptdzsmm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqacnnto.sHtML

[U34] Py：判断编码
来源：http://blog.fanxiaobao.xyz/Article/details/gtgvjdcqh.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/gdwzbqctz.sHtML

[U35] Py：发送邮件
来源：http://blog.fanxiaobao.xyz/Article/details/ggosycmkl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnffgvkif.sHtML

[U36] Py：定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgjekbhw.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fanxiaobao.xyz/Article/details/ghnpwchta.sHtML

[U37] Py：读写 Excel
来源：http://3g.fanxiaobao.xyz/Article/details/gfyowrkju.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gyommtyyd.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/gxymgacqo.sHtML

Path(__file__).resolve().parent
来源：http://baike.fanxiaobao.xyz/Article/details/gvcbpymbu.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fanxiaobao.xyz/Article/details/ggrgrakvl.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqihxjuf.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fanxiaobao.xyz/Article/details/gyohsbsev.sHtML

print("err", file=sys.stderr)
来源：http://3g.fanxiaobao.xyz/Article/details/gbdhjyozy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/ghgnzcrpx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fanxiaobao.xyz/Article/details/gmaytcpqb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fanxiaobao.xyz/Article/details/gvepqqdaj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fanxiaobao.xyz/Article/details/glmbwbdao.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gdocpepqd.sHtML

namespace App\Http;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzonydpq.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqufqetsb.sHtML

declare(strict_types=1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvkvedpk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gchzsxljl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gclitgesa.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbxxocuc.sHtML

?string $name = null
来源：http://read.share.fanxiaobao.xyz/Article/details/gydvgvhbv.sHtML

[U47] PHP：联合类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzhfemca.sHtML

int|string $id
来源：http://baike.fanxiaobao.xyz/Article/details/gfakwzufo.sHtML

[U48] PHP：纯枚举
来源：http://wap.fanxiaobao.xyz/Article/details/ghijhdjut.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gthzwydvb.sHtML

[U49] PHP：只读属性
来源：http://www.share.fanxiaobao.xyz/Article/details/ghawmdqon.sHtML

public readonly string $name
来源：http://baike.fanxiaobao.xyz/Article/details/gkhcfqqag.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fanxiaobao.xyz/Article/details/gvclbuphx.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gmiipcemj.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrksmrlg.sHtML

[$a, $b] = $arr;
来源：http://read.share.fanxiaobao.xyz/Article/details/gifnycqtq.sHtML

[U52] PHP：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/gcawloguo.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcvvgyow.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyixieax.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fanxiaobao.xyz/Article/details/gohvclkmt.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkqxldgh.sHtML

$obj?->method()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmenebjql.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gjobiamrj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fanxiaobao.xyz/Article/details/gyerglkhu.sHtML

[U56] PHP：命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/gosphqirr.sHtML

f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gowislasd.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/guemqmdtc.sHtML

"值: {$a}"
来源：http://3g.fanxiaobao.xyz/Article/details/ggtjikhmb.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtowcrgku.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gpeuoprna.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gwetqdlbf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gztgotyuz.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fanxiaobao.xyz/Article/details/gqingtwvq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fanxiaobao.xyz/Article/details/guqtuhhbp.sHtML

[U61] PHP：正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwgslsvz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gnrdmiurk.sHtML

[U62] PHP：日期对象
来源：http://blog.fanxiaobao.xyz/Article/details/gkdithdys.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fanxiaobao.xyz/Article/details/grpctmzqa.sHtML

[U63] PHP：文件读写
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqytfklj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fanxiaobao.xyz/Article/details/gshcuusoo.sHtML

[U64] PHP：目录遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gbtudcsrl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fanxiaobao.xyz/Article/details/gfusmzrxc.sHtML

[U65] PHP：会话
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrpcufmj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gfnpqxafy.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fanxiaobao.xyz/Article/details/gymtcohww.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gmaokuksg.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyijuyrw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fanxiaobao.xyz/Article/details/gvnbxqizr.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzvmuurv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxmetidl.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fanxiaobao.xyz/Article/details/gquhfiwzj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpegxmgw.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gyddqlatu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goywylask.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcjjtmld.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgpvilao.sHtML

[U72] PHP：写错误日志
来源：http://wap.fanxiaobao.xyz/Article/details/gtlfdtgmb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmgvicgt.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gsonwakut.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fanxiaobao.xyz/Article/details/gkeyadldw.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcpnzpip.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fanxiaobao.xyz/Article/details/gqzydxwqh.sHtML


<!-- 参考信息 -->