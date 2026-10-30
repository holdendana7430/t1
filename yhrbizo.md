代发 wailian999

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gttkkzxyl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gefcxukbo.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gsnbwgbre.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/ghoddrxoc.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gdzgyyowu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gfcwaloqb.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gteljpofl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gegwrhrtc.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gmwvwhgah.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gpdnhfcvx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/guywuwbzj.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gdyioioic.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/gninoohzb.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gpehyfvyy.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gioqrekug.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/guyzhsrxf.sHtML

int size() const noexcept { return n_; }
来源：http://3g.hesvh.cn/Article/details/grhkmilnz.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gxxxenizb.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gczmvpqqf.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/gobmtxsrg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/glmcqrbsj.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gswlytrex.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/gywmbszfb.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/grczbsyby.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/gdotbytrx.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/gxoyyjrct.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/glvahlgqg.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gtyhahhhj.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gxxjxpnjc.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gucgysluf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gyzxpwnrf.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/grqlntpjy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gbzvzmrxm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtacvxswr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gygoijqmc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grelzjxce.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gcfnfxhzz.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gpwgxltmz.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/gpgcpnouy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/gyjnkzvmi.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gzclfagqm.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gksbrlttg.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gzgocxkas.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gqrwdymij.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/glmiqssct.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/gafaquwqd.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gffvmsbiv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/gtrmudsjp.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gtzkiyvif.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/gzuelqbqa.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/grqqunkln.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gukjbatrc.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gmrgltucs.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/gfneflfrf.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/gildzwmmx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/guxtsmzpk.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/gowaaiykl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/gcuttvnst.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gurwtrhgi.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gjnibvnho.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/gswhnamgh.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/gpretwfks.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/gdtbhyuyy.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gfucndulx.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/gwoceftux.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/ggstkwixx.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/gcojxkhnv.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gbrscktab.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gisenwffk.sHtML

var a = 1;  let b = 2
来源：http://read.share.fehbvm.com/Article/details/gdvxuxohc.sHtML

[T18] Swift：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gwxtqdoml.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/ghidrbnpq.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gdqajlddw.sHtML

if let n = opt { print(n) }
来源：http://mobile.zdbjq.cn/Article/details/gcatnstna.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/ggfkpardd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gavcinmem.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/ggndltddg.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/gczhtcgdz.sHtML

[T22] Swift：字典
来源：http://mobile.zdbjq.cn/Article/details/gitclwknp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/gpzrywuop.sHtML

[T23] Swift：函数
来源：http://m.share.zdbjq.cn/Article/details/gjlbvzupo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/gbywslhsu.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/ggyxubiae.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/gziysguvd.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/gxteltksc.sHtML

struct P { var x: Int }
来源：http://www.m.share.zdbjq.cn/Article/details/gpkhwjknd.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/gmrmkwfwh.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gkwemueze.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/gxryuydem.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fehbvm.com/Article/details/gghmallhg.sHtML

[T28] Swift：枚举
来源：http://3g.fehbvm.com/Article/details/gtdcrzkvf.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/ggzmwvuyy.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gywkmeffx.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gqtfmeuwu.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/goqjmlzrz.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/gsklxmyok.sHtML

[T31] Lua：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gjvgvkkaa.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gsojahqdd.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/gziupqsih.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gmmwiatwd.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/giwhwoeza.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/gwvvrpyep.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gtyydklxe.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gwhjlezet.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/gfekydhop.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/giggdvsnc.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/gnjyomnzq.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/gnmhoueiw.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/gmngdzggx.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/guvdrllzo.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/gkrweprew.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/gyahtyalq.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gyfwnkrbg.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/groaucjgb.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/gopozdaad.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/gntuxdvvg.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gibeppmia.sHtML

print "Hello\n";
来源：http://wap.hesvh.cn/Article/details/ggpuerztd.sHtML

[T42] Perl：变量类型
来源：http://read.share.hesvh.cn/Article/details/goemfjmmu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/gjhupkqvr.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gwaabaxqs.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/glkbrrywi.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/guyoqyvyj.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/gqlelhnsc.sHtML

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/gapxvjjeo.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/goqqiwzhp.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gcgiesomf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/glrpqyxne.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gginjfjjg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.hesvh.cn/Article/details/gbjrenngu.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/gzvxglcuz.sHtML

$s =~ s/old/new/g;
来源：http://3g.fehbvm.com/Article/details/ghxrfrwkj.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/gojufaxrs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/girljfvbc.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gjgzxomvi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/gpumzsepl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.hesvh.cn/Article/details/gmxzzreph.sHtML

[T51] Scala：Hello World
来源：http://wap.hesvh.cn/Article/details/grdkuyjnn.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gbkvxbnks.sHtML

[T52] Scala：变量
来源：http://www.share.fehbvm.com/Article/details/gpskdnmqz.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/gjawreouu.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gjkugjwhj.sHtML

s"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gmqrqdxeu.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/gntbaqzkv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/glnyikkoa.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/goazbkkio.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/glmozpnfe.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gmbgzogjo.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/gleyutmka.sHtML

[T57] Scala：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gnrcjpzuw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gsltbefst.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/ghwlyzoth.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.zdbjq.cn/Article/details/gonqeuadj.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/gkiurfzuj.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gbeljgrhf.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/gxeovaoak.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/gncvbkmtl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdgihcvmb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/guparbstn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzinuhzqf.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fehbvm.com/Article/details/guarkgrla.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gmgmmjgkl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/gawxlnlpk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gnxbagszr.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.hesvh.cn/Article/details/ghgxgyibb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/ggtymaxdn.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/ghotmkbps.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.zdbjq.cn/Article/details/ghusgujzm.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/gzwgelvpk.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gguzbmhef.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/gcemskvtn.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/grwtawcvu.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.hesvh.cn/Article/details/gdknxyryr.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.zdbjq.cn/Article/details/ghsynagto.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/gtkaffzkh.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gyurfneyh.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/gzspczsui.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/ghpkvpyjr.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/gpclqdedt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/glpfnvcva.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fehbvm.com/Article/details/grviqvejq.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fehbvm.com/Article/details/gnvbwydie.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fehbvm.com/Article/details/gogivczcd.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/gueuenkuj.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/gcotyfpbz.sHtML

deque(maxlen=10)
来源：http://baike.fehbvm.com/Article/details/glhupuxzt.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/guisdstvf.sHtML

defaultdict(list)
来源：http://3g.hesvh.cn/Article/details/gptjttcrn.sHtML

[U15] Py：高精度计时
来源：http://baike.zdbjq.cn/Article/details/gprxabmvr.sHtML

t = time.perf_counter()
来源：http://3g.zdbjq.cn/Article/details/gmtxqixoi.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.zdbjq.cn/Article/details/gobukuwug.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fehbvm.com/Article/details/gglwksilr.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gjcxkyxax.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.hesvh.cn/Article/details/gkltybgfa.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/gupdsgcgd.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gnvgonruv.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/grekzmrdm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/gyemsbkyq.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gbntsoahu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/grajpxvhs.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fehbvm.com/Article/details/gzevhpsjq.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/gcwkgesri.sHtML

[U22] Py：矩阵转置
来源：http://baike.hesvh.cn/Article/details/gwrlndyqz.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/giuurhzal.sHtML

[U23] Py：分块读取大文件
来源：http://3g.zdbjq.cn/Article/details/gqdmuogms.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/gcskvbjka.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/gfiakcjkw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gohcvsrfh.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fehbvm.com/Article/details/gpbsgzwiw.sHtML

csv.DictReader(f)
来源：http://read.share.fehbvm.com/Article/details/glwdxxvye.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/gonejnren.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/ghzffhaxb.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fehbvm.com/Article/details/gxqywqvfx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.hesvh.cn/Article/details/gobnpneih.sHtML

[U28] Py：类型别名
来源：http://read.share.hesvh.cn/Article/details/gbydbvstr.sHtML

UserId = int
来源：http://www.share.fehbvm.com/Article/details/gzfdxhihj.sHtML

[U29] Py：属性校验
来源：http://m.share.zdbjq.cn/Article/details/goeemjtsr.sHtML

@property 与 @x.setter 配合
来源：http://baike.zdbjq.cn/Article/details/gkdtanvnk.sHtML

[U30] Py：数据类
来源：http://read.share.hesvh.cn/Article/details/gnhgipxbl.sHtML

@dataclass(slots=True)
来源：http://3g.zdbjq.cn/Article/details/gjcwciqvz.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/gibmdfolo.sHtML

python -m pytest -q
来源：http://3g.zdbjq.cn/Article/details/gzmvmmvnu.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fehbvm.com/Article/details/gosrsukth.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/gzugdtljx.sHtML

[U33] Py：打包发布
来源：http://www.blog.fehbvm.com/Article/details/gcnpxhmfi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.zdbjq.cn/Article/details/ggabxbulq.sHtML

[U34] Py：判断编码
来源：http://3g.fehbvm.com/Article/details/glinxkqjp.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gvxmltzkq.sHtML

[U35] Py：发送邮件
来源：http://blog.hesvh.cn/Article/details/gspwdoycz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fehbvm.com/Article/details/guuhkdtsa.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/gihmiwtjr.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.zdbjq.cn/Article/details/gpylacnxx.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fehbvm.com/Article/details/gimxfloos.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fehbvm.com/Article/details/gvqtunljy.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/gabwxgylz.sHtML

Path(__file__).resolve().parent
来源：http://m.share.zdbjq.cn/Article/details/gyzhvcbph.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.hesvh.cn/Article/details/gtfuyxhlu.sHtML

sys.stdout.isatty()
来源：http://www.m.share.hesvh.cn/Article/details/gwemesjct.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fehbvm.com/Article/details/gvuhkzerf.sHtML

print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gmecmjpuz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.zdbjq.cn/Article/details/gzrkuyzsh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/gmjyjjtrv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/gyztxebpi.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.zdbjq.cn/Article/details/gsqgxaocz.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fehbvm.com/Article/details/gzckuxhqy.sHtML

namespace App\Http;
来源：http://read.share.fehbvm.com/Article/details/geynbozyw.sHtML

[U44] PHP：开启严格类型
来源：http://blog.zdbjq.cn/Article/details/gtnarqiua.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/gwpodslrq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/gfnkoqydj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gvctzhvxp.sHtML

[U46] PHP：可空类型
来源：http://wap.hesvh.cn/Article/details/glcekyspl.sHtML

?string $name = null
来源：http://wap.fehbvm.com/Article/details/gzqtpblip.sHtML

[U47] PHP：联合类型
来源：http://blog.hesvh.cn/Article/details/gwlrabvju.sHtML

int|string $id
来源：http://wap.fehbvm.com/Article/details/gfeycenat.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/gncxiacva.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fehbvm.com/Article/details/givosrtqc.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fehbvm.com/Article/details/gufyuljpg.sHtML

public readonly string $name
来源：http://blog.hesvh.cn/Article/details/gvrcucasq.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.zdbjq.cn/Article/details/gcfevzrod.sHtML

public function __construct(private int $id) {}
来源：http://wap.hesvh.cn/Article/details/gzhcnqjpm.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fehbvm.com/Article/details/gpnkzzqlt.sHtML

[$a, $b] = $arr;
来源：http://baike.zdbjq.cn/Article/details/gabetzxci.sHtML

[U52] PHP：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gteuqfvhd.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gcfclbzud.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fehbvm.com/Article/details/gdpyrkrfn.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/gcjnloueq.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fehbvm.com/Article/details/gvdvsrtmw.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/gugmokapa.sHtML

[U55] PHP：match 表达式
来源：http://blog.zdbjq.cn/Article/details/gjuhhowtv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/grbzydndf.sHtML

[U56] PHP：命名参数
来源：http://baike.zdbjq.cn/Article/details/gtikkybdt.sHtML

f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gbnosyyok.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gldgthduq.sHtML

"值: {$a}"
来源：http://3g.zdbjq.cn/Article/details/gifzazibs.sHtML

[U58] PHP：数组三件套
来源：http://mobile.zdbjq.cn/Article/details/gqltftpdm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fehbvm.com/Article/details/grltntfte.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/gattmmmfm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gtinfjhej.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.zdbjq.cn/Article/details/gqvyzfcid.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fehbvm.com/Article/details/gqvsulgwr.sHtML

[U61] PHP：正则
来源：http://3g.zdbjq.cn/Article/details/gdnkuntye.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gaectnxgu.sHtML

[U62] PHP：日期对象
来源：http://read.share.fehbvm.com/Article/details/gcjxmpxfr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.hesvh.cn/Article/details/gvmzkevpu.sHtML

[U63] PHP：文件读写
来源：http://m.share.zdbjq.cn/Article/details/gynghudrp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.hesvh.cn/Article/details/gknqymlkm.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/ggtcevmwe.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.zdbjq.cn/Article/details/gcavahfbp.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/gyckstgmm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gmxbqeutf.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.hesvh.cn/Article/details/ghfmdiblb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fehbvm.com/Article/details/gqkqajgvz.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.hesvh.cn/Article/details/gnnlzlmig.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/gvtqxffwo.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/gtswqxavm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/grfctzlue.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.zdbjq.cn/Article/details/gyllygomr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.hesvh.cn/Article/details/gavsxwypf.sHtML

[U70] PHP：PDO 事务
来源：http://wap.hesvh.cn/Article/details/ggsnwhsab.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.hesvh.cn/Article/details/gbhuplrqm.sHtML


<!-- 参考信息 -->