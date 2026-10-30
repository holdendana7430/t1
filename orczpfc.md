代发 wailian999

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gehsilxeg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gvtnmplgf.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gepnhankq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/gazgihipg.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gcqzjzdwr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gljcbxoot.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gopucqlfu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/ghssuevzt.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/ggmxyrygx.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gloassffn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/gpnzcielq.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gzlitxigd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/gmejgpzsz.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/gushumuuw.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gvpsxyhjp.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gfbaiyenh.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gvbaxvrlt.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/grvejkwav.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gpbxwicav.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/gdugkofva.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gmzwfdhjk.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gxprkceks.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gemzutsuu.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gujzhffir.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gqhggsgwj.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gmfxnwkqa.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gyqxnthav.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gpkcncwmi.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gfrzuwmyp.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/gtvlrapsx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/gpfjbibzz.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gvlpabswr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gfsqteios.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gaifgbtlr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gqqeeouqs.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqbgspbev.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gpdzqwacl.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gjytrlwxg.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gbtatxuim.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/gicpqyjbn.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gbatvgfkb.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/grbkylbmi.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gsnqhskvz.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gaclcizvu.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gzcvarhuu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gisrqbdgz.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gajcigpcn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gdalndmtl.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gkqdtdsqg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/grgxsdevf.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gwzbloagf.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.hesvh.cn/Article/details/ghgwdhcjj.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gwgpfwuke.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/giaixijnc.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/ggiinozfl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gutcbsthf.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gvjupkxex.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gxphhwyxp.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/gljftschj.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gcbjorxen.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/goodhqgrj.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/glvskhrgm.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/ghbytaywu.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/gmjsjefpy.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/guqltvkas.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/galejmwqm.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gotgagvlr.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gwnxxeilw.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/ginznjnsw.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/gmymdzywy.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/grkohynqv.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/gkdchiitd.sHtML

[T19] Swift：可选绑定
来源：http://www.share.hesvh.cn/Article/details/gjrwvrxwu.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/gpqtgvmxb.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/gdncvsmhk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fehbvm.com/Article/details/gctkaxkki.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gzknidune.sHtML

for x in a { print(x) }
来源：http://3g.zdbjq.cn/Article/details/gcctyojoy.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/guvchclrw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gmpcalkin.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gibmireqk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gpkqmnmyz.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/gegoeoinp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gyeotjqxy.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/goxgzsjfh.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gxejbqlpt.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gteiguuvb.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/gvygnmurq.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/gecbayrnv.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fehbvm.com/Article/details/gndclesza.sHtML

[T28] Swift：枚举
来源：http://3g.zdbjq.cn/Article/details/gelhokxgi.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/gfnjrnyyl.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/ghhuzmpxg.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gldmqsndu.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gcofbtjvf.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gxtonkwcx.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/gpipqewdu.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gapdkpkic.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/gjxpuigpf.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/grneyzqvz.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/gfurfkczu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/ghgihavuk.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/gvbyyfgav.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/gufsxyfny.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gawdjhuph.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gjrxlcavw.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/gyhhoyxxa.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/guuyywqhn.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gsxgeyjkh.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/giriwzxgb.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/goxnvpjbg.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/gmthjfnue.sHtML

[T39] Lua：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gmzxdwuxw.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/gxzxkkrla.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/gozvzqtsk.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/getoiwxwx.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/gjdvkzwks.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/gdfgrhkio.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/gxxmwxxpc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/gqtmhlfpw.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gdtlchabj.sHtML

"值: $a"
来源：http://www.m.share.fehbvm.com/Article/details/gddoonsza.sHtML

[T44] Perl：条件
来源：http://wap.fehbvm.com/Article/details/groycdumq.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fehbvm.com/Article/details/ggcbsnxzk.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/guhgtpxhb.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/gyvkmptua.sHtML

[T46] Perl：哈希操作
来源：http://baike.hesvh.cn/Article/details/ghbitjtga.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/gvlvxnmcm.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fehbvm.com/Article/details/gdqxzhihd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/goduywurs.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gwlpyemlj.sHtML

$s =~ s/old/new/g;
来源：http://read.share.zdbjq.cn/Article/details/ghmpuumim.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/gqxdifypp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gkpkyuxcf.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gxzwujnpj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/geiqsfwxp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/grzfbcdjl.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/gsxusallv.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gkclunwtc.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gclsvrwzg.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/gskpisupu.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gcytdadic.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gomrzjrxm.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/ganuehmcg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/gvjsouefl.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/ggehkktrk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fehbvm.com/Article/details/grdsgzvky.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/galucnswo.sHtML

case class User(name: String, age: Int)
来源：http://blog.zdbjq.cn/Article/details/gbcpidehg.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gdpziwbkn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gaipuwyyw.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/gspuoqrwf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.hesvh.cn/Article/details/gtnynpxsh.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gmlbbqxpk.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gktywbdri.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/gxmdovvpj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/gdmyyaxkq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxwzvzppu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/geaotuyxf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gyofucmtd.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gxayfxlzv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/gnmhtuzfw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/guecgrqnk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gjtkltqzz.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.zdbjq.cn/Article/details/givcwtwkg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/gnpqshnlc.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.zdbjq.cn/Article/details/gaobnsnfz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/gvvkaeevv.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.hesvh.cn/Article/details/ggljxmavg.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gthdtuedo.sHtML

[U06] Py：合并两个字典
来源：http://blog.hesvh.cn/Article/details/gozjldefh.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/gxcilfnfh.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/giduinatz.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/gfuyqkbuk.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/gnvloslzn.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gyypvjtrf.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/gwwruyuyv.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/gsxxsvogb.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/gvibtbcxu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fehbvm.com/Article/details/gymjismwj.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/gwdiagzsg.sHtML

(x * 2 for x in arr)
来源：http://wap.zdbjq.cn/Article/details/gwevopygk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/gjwxbpaba.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/gyotgdmog.sHtML

[U13] Py：固定长度队列
来源：http://3g.zdbjq.cn/Article/details/goouwomxe.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/gtbozsvjm.sHtML

[U14] Py：分组收集到列表
来源：http://baike.hesvh.cn/Article/details/glfaacegz.sHtML

defaultdict(list)
来源：http://www.share.hesvh.cn/Article/details/gwjwnkrrc.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/gmeknlebv.sHtML

t = time.perf_counter()
来源：http://www.share.hesvh.cn/Article/details/gmpmokloc.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/gnmpafpga.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/gilnwbgvn.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gkbhfpeut.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/gtyhpndkv.sHtML

[U18] Py：预编译正则
来源：http://read.share.zdbjq.cn/Article/details/gsnbysfvw.sHtML

pat = re.compile(r"\d+")
来源：http://wap.zdbjq.cn/Article/details/gmiaqmmlb.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fehbvm.com/Article/details/gpxzxruml.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fehbvm.com/Article/details/gmjjgrxaw.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/gerdfxuxd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.hesvh.cn/Article/details/gjtdsdhov.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/gqlddvfpg.sHtML

@contextlib.contextmanager
来源：http://www.share.hesvh.cn/Article/details/gcjvrdjgd.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/gsxdhstsm.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/grjameyim.sHtML

[U23] Py：分块读取大文件
来源：http://baike.hesvh.cn/Article/details/gduuefehg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/ggvkuwonl.sHtML

[U24] Py：路径操作
来源：http://www.share.fehbvm.com/Article/details/gigompflg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/ggvdzpobg.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.hesvh.cn/Article/details/ghcwprerr.sHtML

csv.DictReader(f)
来源：http://m.share.hesvh.cn/Article/details/gqbthlzzv.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/gyztmqybz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/gjpqnqteg.sHtML

[U27] Py：异步 HTTP
来源：http://blog.hesvh.cn/Article/details/gofivldcj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.hesvh.cn/Article/details/glymmrszl.sHtML

[U28] Py：类型别名
来源：http://www.m.share.hesvh.cn/Article/details/gbakocnjy.sHtML

UserId = int
来源：http://www.m.share.fehbvm.com/Article/details/glvpaisce.sHtML

[U29] Py：属性校验
来源：http://baike.zdbjq.cn/Article/details/gkugpxrog.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fehbvm.com/Article/details/gthrmzpnb.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/gyhdhqymr.sHtML

@dataclass(slots=True)
来源：http://baike.hesvh.cn/Article/details/gbkysdpfo.sHtML

[U31] Py：单测
来源：http://read.share.fehbvm.com/Article/details/gehhrahgn.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/gtaxtjsnn.sHtML

[U32] Py：代码格式化
来源：http://read.share.fehbvm.com/Article/details/grnonhxei.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gmolzousv.sHtML

[U33] Py：打包发布
来源：http://3g.zdbjq.cn/Article/details/glxhcykqu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/gkyfsnblg.sHtML

[U34] Py：判断编码
来源：http://www.m.share.hesvh.cn/Article/details/ggonphiux.sHtML

chardet.detect(raw)
来源：http://3g.hesvh.cn/Article/details/gpkejuqay.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/gsnrcddod.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.zdbjq.cn/Article/details/grruqizpx.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/gkqgyzbcs.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.zdbjq.cn/Article/details/gcoktongv.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/gbewnsita.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fehbvm.com/Article/details/gozylwdvl.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fehbvm.com/Article/details/gfdwvixqm.sHtML

Path(__file__).resolve().parent
来源：http://wap.hesvh.cn/Article/details/gyzimnjsn.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/gkwucfria.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/gogvckeco.sHtML

[U40] Py：打印到标准错误
来源：http://3g.zdbjq.cn/Article/details/gdvaajnus.sHtML

print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/ghyttxddl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fehbvm.com/Article/details/gmhomfsxa.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gwrwpqqov.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/gvxlnjaec.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.hesvh.cn/Article/details/gtpubkhzo.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/gybifpqui.sHtML

namespace App\Http;
来源：http://www.blog.hesvh.cn/Article/details/gjcwuzywv.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gjaxosxcq.sHtML

declare(strict_types=1);
来源：http://wap.hesvh.cn/Article/details/gvwphirld.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/gtnutqwlm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gimrtfzzf.sHtML

[U46] PHP：可空类型
来源：http://blog.hesvh.cn/Article/details/gcmdooyos.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/gldbnvbby.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/gbypvhaux.sHtML

int|string $id
来源：http://wap.hesvh.cn/Article/details/gvjqzehiv.sHtML

[U48] PHP：纯枚举
来源：http://wap.zdbjq.cn/Article/details/gctrglxlb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/gmdynjhnb.sHtML

[U49] PHP：只读属性
来源：http://m.share.hesvh.cn/Article/details/glgeyznun.sHtML

public readonly string $name
来源：http://www.share.fehbvm.com/Article/details/ggzgvzhhz.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.hesvh.cn/Article/details/glktybnvi.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/gbhtepreh.sHtML

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/gzrqwdpiu.sHtML

[$a, $b] = $arr;
来源：http://3g.hesvh.cn/Article/details/gbnzmzdcb.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gaxdoytya.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.zdbjq.cn/Article/details/gczrpogcn.sHtML

[U53] PHP：空合并运算符
来源：http://blog.hesvh.cn/Article/details/gkjlubinz.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fehbvm.com/Article/details/gzqsvnvgb.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fehbvm.com/Article/details/gfogbfmfy.sHtML

$obj?->method()
来源：http://wap.fehbvm.com/Article/details/gjbsbnpzj.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fehbvm.com/Article/details/gfuozgvom.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gkwmwibxw.sHtML

[U56] PHP：命名参数
来源：http://blog.hesvh.cn/Article/details/gntxpwrqz.sHtML

f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gqgdtwtii.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gptwgedxy.sHtML

"值: {$a}"
来源：http://m.share.zdbjq.cn/Article/details/gytfpbzdl.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/gtfkeehli.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.zdbjq.cn/Article/details/grvetfbfg.sHtML

[U59] PHP：自定义排序
来源：http://3g.fehbvm.com/Article/details/gesgwydta.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gfrukpyqu.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.zdbjq.cn/Article/details/gsnhcyjzt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gknbxisfi.sHtML

[U61] PHP：正则
来源：http://blog.zdbjq.cn/Article/details/gdtvedeaw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/gnamjngnl.sHtML

[U62] PHP：日期对象
来源：http://read.share.zdbjq.cn/Article/details/gbdrrxtgq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/gjvlkhwby.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fehbvm.com/Article/details/ggypdxhjx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fehbvm.com/Article/details/gpntepjgp.sHtML

[U64] PHP：目录遍历
来源：http://3g.zdbjq.cn/Article/details/gnaaowgkt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.hesvh.cn/Article/details/gkcfqyzyg.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/gfvxilkgi.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.hesvh.cn/Article/details/giemzpcgl.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/ggjcwklri.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.zdbjq.cn/Article/details/gvpqvozhv.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fehbvm.com/Article/details/gxwgaureg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.hesvh.cn/Article/details/gfnlcneiv.sHtML

[U68] PHP：PDO 连接
来源：http://wap.zdbjq.cn/Article/details/gytuwouoj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/gztzlwiov.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/ghqfxlsaz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.zdbjq.cn/Article/details/gvkvmmkwl.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.zdbjq.cn/Article/details/ghngmmpsj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fehbvm.com/Article/details/gwdpohtkh.sHtML


<!-- 参考信息 -->