代发 wailian999

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/gsebgeqoz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/givwmnnns.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gowndoeqf.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/glwhjvpsj.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gjkluoscd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gtryvbssz.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/gdozxmgny.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/ghxrzmlkx.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gwpwxhtgf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gmmxkfqee.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/grycjtdci.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gfoqxsyps.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gqlzqzyyd.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gsmycybhp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gzueoqxlp.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/gwacevcfz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gmsniofjm.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gsvtsurrl.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gflqqlehk.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gkwjdhyyf.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/gdfmnoyxw.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gbdrpgqtx.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gonptzczz.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/giybysdbw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gvtaqyjte.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/ghwofcdcr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/gusrzcwkk.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gqkibwbba.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gnersbrjf.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gvfzvfbus.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gfkgnljyg.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/gjbdpsfmy.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gvlljvjwv.sHtML

[S59] C++：静态断言
来源：http://read.share.fehbvm.com/Article/details/gnkcmdcqp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/gnmgmzgxu.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/giaktcerp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/gkzuyrvmu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmhiqnzmq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/guqfqywym.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghvpzzogb.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gjbjoaihv.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gazcoqsod.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gtbyepcpz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/garhgpqky.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gwpizjyte.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gsmpchikl.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/gpyaxwaht.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gpntkwevl.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/grflbzdqw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/grjymzyip.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/grofxmxal.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gzbwlgfip.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gbsamnszd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gdgcamvlb.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/gcqhhokot.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gdrghjaum.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/gdcpmwyir.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/guyiubrwy.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/guxddmgol.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/grvrgrfbx.sHtML

[T11] Kotlin：协程
来源：http://www.share.hesvh.cn/Article/details/ggnvoeovh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gliranwyn.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/gkgazjmim.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gtfpethcz.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gqmsozjje.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/gshdmmxsn.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gsfqfbvui.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/ghujnzxyh.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gijcbuliz.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gylixeuio.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gzuxalkii.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gisgdfdbc.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gfebarpwj.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gmjkyipfo.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gwfiiqnir.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/glbejgafu.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gowkogarh.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gkiwlpymu.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gefwqthug.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/gcohlikqq.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/gjrhdgsmt.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/gsqvvswto.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gtypxtrey.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gsczredhf.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/gxjakvxjg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/gahgwzucq.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gplahmowv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gyylpavly.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/gmldfnfpw.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gvcmlnqnf.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/gwpudumon.sHtML

class A: Base { override func f() {} }
来源：http://mobile.hesvh.cn/Article/details/gjdssxbze.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gibothnoo.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/gcggnkfof.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/guhykvwrr.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/ghdwrxkrz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gcsagybyn.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gmaqtpvpy.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gqpwwxwdd.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/gbqwmzdom.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gsjwbcoap.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gmslohldv.sHtML

[T32] Lua：局部变量
来源：http://read.share.fehbvm.com/Article/details/gqsgkpjsj.sHtML

local a = 1
来源：http://baike.zdbjq.cn/Article/details/gmdghdtuh.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fehbvm.com/Article/details/gsarjpjop.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/gjooxwovn.sHtML

[T34] Lua：遍历表
来源：http://www.share.hesvh.cn/Article/details/gcyboftmr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/ghivhjess.sHtML

[T35] Lua：字典表
来源：http://m.share.hesvh.cn/Article/details/gfijbivxk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/gslamlmbd.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/gaysgnmxq.sHtML

function add(a, b) return a + b end
来源：http://baike.fehbvm.com/Article/details/ggvjqokel.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gtebnpsob.sHtML

"a" .. "b"
来源：http://read.share.fehbvm.com/Article/details/gvdzdgeqw.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/gpozstgqv.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/gwbobgryz.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/gpifdmdth.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gfqyxgoui.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/gzojiwufp.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/gojouqenz.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gtuszfnto.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/glgyqehdi.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/gocpdrhgl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/getgbsdry.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/grstquitf.sHtML

"值: $a"
来源：http://www.m.share.fehbvm.com/Article/details/gwyezhkwy.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/gdyfpwdum.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/gdxvqrnoi.sHtML

[T45] Perl：数组遍历
来源：http://wap.zdbjq.cn/Article/details/gvveoawlx.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdjsvtqbw.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/gcwdqmcdk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/grcnafhfe.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/grmmpydfe.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.zdbjq.cn/Article/details/gvkzbkqfw.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/glmrhykqf.sHtML

$s =~ s/old/new/g;
来源：http://www.share.hesvh.cn/Article/details/gpnztkacq.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gcitubzyf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gejhkhaqd.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gzzgxunao.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/gngwmsvuu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.zdbjq.cn/Article/details/glzgsiegk.sHtML

[T51] Scala：Hello World
来源：http://blog.fehbvm.com/Article/details/gadlruvwc.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gshnvbszu.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/gzbkseale.sHtML

val a = 1;  var b = 2
来源：http://blog.zdbjq.cn/Article/details/gxbsqnswe.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gxhgrqrcr.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gmfdtxzdz.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/gfpkotqvr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/gbnrnnvau.sHtML

[T55] Scala：集合过滤
来源：http://m.share.hesvh.cn/Article/details/glaghfpca.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gfasknsvy.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/gfcyghfry.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gycujxnek.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/goxljcgqd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/giocupmwq.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gqrhumacq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/guwcauozj.sHtML

[T59] Scala：循环
来源：http://read.share.zdbjq.cn/Article/details/gvptodwsu.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gmidwqdpw.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gewljzvqj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.zdbjq.cn/Article/details/gtzgsieye.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gyzdpoloq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gttmlvmxf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqswuobsm.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fehbvm.com/Article/details/gmywsosus.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/gibtvbniz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/ghsovhset.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/ghbyoxbcq.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/grdjqqxnm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.hesvh.cn/Article/details/gfyvycsoh.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/gsozjcyku.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.zdbjq.cn/Article/details/gtoofofpt.sHtML

[U05] Py：列表去重且保序
来源：http://3g.hesvh.cn/Article/details/gwauxmofd.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gmhvhxxpe.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gcingiixh.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gqrlcocdg.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/gmahwyxan.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gcgkohfji.sHtML

[U08] Py：展平二维列表
来源：http://blog.fehbvm.com/Article/details/gjipkzaya.sHtML

[y for x in nested for y in x]
来源：http://www.share.fehbvm.com/Article/details/gbtmevtfq.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.zdbjq.cn/Article/details/gviycckev.sHtML

max(d, key=d.get)
来源：http://www.blog.fehbvm.com/Article/details/gjfxsramj.sHtML

[U10] Py：按值排序字典
来源：http://baike.zdbjq.cn/Article/details/gneuqzwvd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/gsmehlztz.sHtML

[U11] Py：生成器表达式
来源：http://3g.fehbvm.com/Article/details/gwsddzhjz.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/guipckrbr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/gjajevlut.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.zdbjq.cn/Article/details/gwpbcvrrd.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/giraetgfp.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/glgfpmstn.sHtML

[U14] Py：分组收集到列表
来源：http://baike.hesvh.cn/Article/details/gohlrnwgz.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/gadqvbmtb.sHtML

[U15] Py：高精度计时
来源：http://www.share.fehbvm.com/Article/details/gsukvaxgv.sHtML

t = time.perf_counter()
来源：http://3g.zdbjq.cn/Article/details/groldrriw.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/gbhnqemmr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/glddfkmoc.sHtML

[U17] Py：初始化日志
来源：http://read.share.zdbjq.cn/Article/details/gdgbkcikh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.hesvh.cn/Article/details/gzzkorlpt.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.zdbjq.cn/Article/details/gjrmuuski.sHtML

pat = re.compile(r"\d+")
来源：http://3g.zdbjq.cn/Article/details/gkbkavygi.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fehbvm.com/Article/details/gmlgtokxg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fehbvm.com/Article/details/guvjkqbgq.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/gllovlltm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.hesvh.cn/Article/details/gztwkpyex.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/gskncckem.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/gspoknllr.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/gtvcocraw.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/gpkflzkgy.sHtML

[U23] Py：分块读取大文件
来源：http://blog.hesvh.cn/Article/details/gdbpwqepw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.hesvh.cn/Article/details/gpfagsive.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/gqmjycvuh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gjiowiyjc.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.hesvh.cn/Article/details/gkiuunurt.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/gbjhrwgqy.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/gvljtqjdp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.zdbjq.cn/Article/details/gbvmrfrut.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/gmsieduub.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/gnftkdeuw.sHtML

[U28] Py：类型别名
来源：http://m.share.zdbjq.cn/Article/details/gzqknemyo.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/gnbcusnnn.sHtML

[U29] Py：属性校验
来源：http://m.share.fehbvm.com/Article/details/glgwvojph.sHtML

@property 与 @x.setter 配合
来源：http://3g.fehbvm.com/Article/details/gwuohocqv.sHtML

[U30] Py：数据类
来源：http://www.share.fehbvm.com/Article/details/gdtzsebco.sHtML

@dataclass(slots=True)
来源：http://3g.fehbvm.com/Article/details/gdausncjx.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/gxvmkdvqj.sHtML

python -m pytest -q
来源：http://blog.zdbjq.cn/Article/details/gvqeizqri.sHtML

[U32] Py：代码格式化
来源：http://mobile.hesvh.cn/Article/details/gsxflumlz.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.hesvh.cn/Article/details/gilenbhgv.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/gwfpqudpe.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.hesvh.cn/Article/details/gdeekotrt.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fehbvm.com/Article/details/gpxfktulh.sHtML

chardet.detect(raw)
来源：http://m.share.hesvh.cn/Article/details/gfkqwkfqb.sHtML

[U35] Py：发送邮件
来源：http://mobile.fehbvm.com/Article/details/ggihbhcsm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fehbvm.com/Article/details/gzwwmpppd.sHtML

[U36] Py：定时任务
来源：http://mobile.fehbvm.com/Article/details/gykqvgxmu.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fehbvm.com/Article/details/gwlwurgwt.sHtML

[U37] Py：读写 Excel
来源：http://wap.fehbvm.com/Article/details/gnsevwsth.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.hesvh.cn/Article/details/gtjwoipps.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/gmyseicea.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fehbvm.com/Article/details/gnywyxgbk.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/grubstzej.sHtML

sys.stdout.isatty()
来源：http://read.share.hesvh.cn/Article/details/gddpswkpp.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.zdbjq.cn/Article/details/ghfdgdoyh.sHtML

print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gxoibwwfj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fehbvm.com/Article/details/gqlhuvafh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fehbvm.com/Article/details/gtxdmpfjk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.zdbjq.cn/Article/details/ggubxllnk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/gbuzebnpo.sHtML

[U43] PHP：声明命名空间
来源：http://3g.hesvh.cn/Article/details/gmhevinfv.sHtML

namespace App\Http;
来源：http://read.share.hesvh.cn/Article/details/gymlgnljx.sHtML

[U44] PHP：开启严格类型
来源：http://blog.hesvh.cn/Article/details/gblazvdgw.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/gmfbgajua.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.hesvh.cn/Article/details/gjjroyber.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gekthyfpd.sHtML

[U46] PHP：可空类型
来源：http://read.share.fehbvm.com/Article/details/gsahodgrx.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gluvqlkgg.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/glysidhhh.sHtML

int|string $id
来源：http://www.m.share.hesvh.cn/Article/details/gbugngnmp.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fehbvm.com/Article/details/gckcwjdrp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/gphblrosn.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fehbvm.com/Article/details/gqiokzneg.sHtML

public readonly string $name
来源：http://baike.zdbjq.cn/Article/details/gdeqtebax.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.hesvh.cn/Article/details/grsfdmewg.sHtML

public function __construct(private int $id) {}
来源：http://blog.zdbjq.cn/Article/details/gkplnlzdj.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.zdbjq.cn/Article/details/gswwahjur.sHtML

[$a, $b] = $arr;
来源：http://mobile.zdbjq.cn/Article/details/gnoxwtbkz.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gzmlddcnf.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/gtdbkxstf.sHtML

[U53] PHP：空合并运算符
来源：http://wap.zdbjq.cn/Article/details/gzzlgyeoy.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/gboveehwx.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fehbvm.com/Article/details/grfujrcha.sHtML

$obj?->method()
来源：http://baike.zdbjq.cn/Article/details/gpzprenod.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gsimlyhnt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/gahuijwov.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/geyixdevd.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gtjwlgrsh.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/grvqkkrkf.sHtML

"值: {$a}"
来源：http://www.m.share.fehbvm.com/Article/details/gmwbaaihz.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/gyhkfqssw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fehbvm.com/Article/details/ghasqaylh.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fehbvm.com/Article/details/gapxtawov.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gnteadpjc.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/gkqndbjjm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gjjcudfxq.sHtML

[U61] PHP：正则
来源：http://m.share.fehbvm.com/Article/details/gtyglgmdp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gvrcodvra.sHtML

[U62] PHP：日期对象
来源：http://www.share.hesvh.cn/Article/details/gsgmnxxfi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fehbvm.com/Article/details/gghohjsot.sHtML

[U63] PHP：文件读写
来源：http://wap.zdbjq.cn/Article/details/grkqilnxo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fehbvm.com/Article/details/gvvfnkoyo.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fehbvm.com/Article/details/gvtmcwtda.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/ggpiofikg.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/gzsavfrsv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gfywxnolg.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fehbvm.com/Article/details/goziicyny.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fehbvm.com/Article/details/gjglschkf.sHtML

[U67] PHP：处理文件上传
来源：http://3g.hesvh.cn/Article/details/gmcrgmgjy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.zdbjq.cn/Article/details/gpxkjxwaj.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.zdbjq.cn/Article/details/gruholjls.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/gzkqxsbtb.sHtML


<!-- 参考信息 -->