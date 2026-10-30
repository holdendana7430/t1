代发 wailian999

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/gerryztpu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gwzmoawov.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gaeayurny.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gmnnztuiu.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gkaxysdgt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gnksdndgv.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gmbtlnokq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gmhklzdzi.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gjlspnulr.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gvpyrafzi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/grncoyokt.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gajprmpjt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/godplxlfv.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gxjlnszsw.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/gnggshrto.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/gyzllslqh.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gyutiyvps.sHtML

[S53] C++：移动语义
来源：http://3g.hesvh.cn/Article/details/giagyztzs.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gnwtpuzch.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gqsstqfwa.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gaevjomtk.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gbfmdvaxq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/gbbnpqscw.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gbfiqdqop.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjvgvbwly.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/grgluvwdf.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gpljvdbfy.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/grnpmxhlc.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/ggmqxargc.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/glslghnph.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/gbfvmxzlw.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gvyqzqehf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gypihnshi.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glqmpvwzs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gafxlnnoh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxqbyxhgz.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gjkvqekeh.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gyyodrczj.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gjvzibwww.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gvblguwor.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/gmisojsws.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gjqmvcmxm.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/ghnlymssd.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/ghzgssqxq.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gepvkzezw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gytnofkqc.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/guxsranjn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gbmflybik.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gbfyceiez.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/ggacscodh.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/gfpohxxex.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gwlchiyoq.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gnluzfnwd.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/geehnfhbu.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/gxpseduiz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gjdqzjbkm.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/gdcslttma.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/gsbrxntly.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gicbabrfm.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gazuzjpkm.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/gpaarwpax.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gsfiqjmek.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gdzyrubsf.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gyauqewbs.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gokqrfkig.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/gzssodikn.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/gtefrvqqy.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gesgrkuyt.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gtdcrauih.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/givswwiwt.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gmbfhbrah.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/glvxtuqdb.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/grakcfmjs.sHtML

if let n = opt { print(n) }
来源：http://blog.fehbvm.com/Article/details/grioqkdvz.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/gjhcjvbir.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/gmhviypnn.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/gcehbmxkn.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/gyuqeidih.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/grgqoaysg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gtyhyhivf.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/gfxsuktdi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/gszdixxjl.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gochwvzks.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/giqpwmedz.sHtML

[T25] Swift：结构体
来源：http://wap.zdbjq.cn/Article/details/gllrqvnep.sHtML

struct P { var x: Int }
来源：http://blog.zdbjq.cn/Article/details/goqqxbntk.sHtML

[T26] Swift：类与重写
来源：http://baike.hesvh.cn/Article/details/gxfpikagr.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/gejwqlpjk.sHtML

[T27] Swift：错误处理
来源：http://m.share.zdbjq.cn/Article/details/ggpquyett.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/gbkllkjqf.sHtML

[T28] Swift：枚举
来源：http://blog.fehbvm.com/Article/details/gvmtugrbc.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/gkdijvmcb.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/gpakkcxba.sHtML

guard let x = opt else { return }
来源：http://m.share.zdbjq.cn/Article/details/grtbywlns.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gqphyecbr.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/gwrjaczxl.sHtML

[T31] Lua：Hello World
来源：http://m.share.fehbvm.com/Article/details/gsppyvuai.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gywmwezlw.sHtML

[T32] Lua：局部变量
来源：http://baike.zdbjq.cn/Article/details/gkkxulscq.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gsjpqxegq.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/glcepprvc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/gukgozxnu.sHtML

[T34] Lua：遍历表
来源：http://mobile.zdbjq.cn/Article/details/gbzizliip.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/gdqqrotcr.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/gvowwgafw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/gmevitpxc.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gkhaefutq.sHtML

function add(a, b) return a + b end
来源：http://baike.zdbjq.cn/Article/details/gthouoiww.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/gtdxjawdn.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gjchvltnb.sHtML

[T38] Lua：条件
来源：http://read.share.zdbjq.cn/Article/details/gziyqksqm.sHtML

if x > 0 then print("正") end
来源：http://mobile.zdbjq.cn/Article/details/gazxbdhej.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gxuygwvam.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gfxbvwcsu.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/gxscwryuh.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/gzfzjxkjz.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gjwryzezt.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/gagoyawhz.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gqqzctncm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/gnirdlpff.sHtML

[T43] Perl：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gfvhjskst.sHtML

"值: $a"
来源：http://www.m.share.hesvh.cn/Article/details/gfqjtwkog.sHtML

[T44] Perl：条件
来源：http://m.share.fehbvm.com/Article/details/gleflqrmm.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fehbvm.com/Article/details/gvidloeea.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/gcqbkdisl.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/gvjwbonpd.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.zdbjq.cn/Article/details/gesueagjh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/gxtyzpjmd.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/glnilhjsv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gtvxmnooz.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/gnxfuomza.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fehbvm.com/Article/details/gyvtspjsr.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/ggzmvvpvj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/ghztxnvnu.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gjqmpicqd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gwyobvfya.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/gevjgpnzx.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gpuevwnob.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gssulsajn.sHtML

[T52] Scala：变量
来源：http://www.share.fehbvm.com/Article/details/gbivdyqcw.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/gssadiqcw.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gdnxgwitw.sHtML

s"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gzflqacho.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/gbgkqwrqr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/grxmpagcc.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gagmajrru.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/gmaueyxlz.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/gqctiiaxv.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/ghdwqybrc.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/guyjkrybv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gapflgjeq.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/glxksavww.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/gjhusxrcz.sHtML

[T59] Scala：循环
来源：http://3g.hesvh.cn/Article/details/ggvnrluri.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gpjnntzex.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/gkryyakbs.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/ghwpazcty.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghhclrsue.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gdpfqbeul.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gsyqeljrm.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gjreixcbm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fehbvm.com/Article/details/gitaabwxa.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.zdbjq.cn/Article/details/gvblffszv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/gskqsalcw.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fehbvm.com/Article/details/gtbtyxecu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.zdbjq.cn/Article/details/gbrhqdikj.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/guphsbkcf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fehbvm.com/Article/details/gxwowcazd.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.hesvh.cn/Article/details/gqmsopece.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gdawqhfvt.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.hesvh.cn/Article/details/gunmyznqz.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/gleciyaql.sHtML

[U07] Py：反转字典键值
来源：http://m.share.hesvh.cn/Article/details/ghvpnmqgu.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gpbkynory.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/gbiqylleb.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/grhojqbdt.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/gwbiknkjw.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gigjvjyzk.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/gcpcdtzzl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fehbvm.com/Article/details/gftetwxck.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/gweudmabk.sHtML

(x * 2 for x in arr)
来源：http://blog.fehbvm.com/Article/details/gkwyrupik.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/gfcowlhmc.sHtML

Counter(arr).most_common(3)
来源：http://mobile.hesvh.cn/Article/details/gvyewynmq.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gjalbhqeo.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/ghkrhqeva.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/gfgxqpgvc.sHtML

defaultdict(list)
来源：http://wap.hesvh.cn/Article/details/ganuwxede.sHtML

[U15] Py：高精度计时
来源：http://3g.fehbvm.com/Article/details/grbgligsl.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/gyecdlern.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/gbyowpqct.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.hesvh.cn/Article/details/gmrihwbeo.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gldukdegu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/gmmzkzsac.sHtML

[U18] Py：预编译正则
来源：http://m.share.hesvh.cn/Article/details/gyezrociy.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gkpqtmeit.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fehbvm.com/Article/details/gkskwuxji.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.zdbjq.cn/Article/details/gnnvqjffl.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.hesvh.cn/Article/details/gmtlmmste.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/gccccxbmx.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.hesvh.cn/Article/details/gdrchrgeu.sHtML

@contextlib.contextmanager
来源：http://blog.hesvh.cn/Article/details/golhtgvul.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/gdidolcat.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/gyxhhvbfy.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/gwdjsjjfo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/gmagqnhoc.sHtML

[U24] Py：路径操作
来源：http://wap.zdbjq.cn/Article/details/gzrilxckv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gjkmoqjeb.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/gvxhprmxx.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/gdfxcfwqy.sHtML

[U26] Py：并发下载
来源：http://3g.hesvh.cn/Article/details/gskyeqavt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/grsaxlgvs.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/gehgjpprl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/gbhlxuwkh.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/gbwwibxjg.sHtML

UserId = int
来源：http://3g.hesvh.cn/Article/details/giywgjjdw.sHtML

[U29] Py：属性校验
来源：http://read.share.hesvh.cn/Article/details/gnmvbbfdc.sHtML

@property 与 @x.setter 配合
来源：http://www.share.zdbjq.cn/Article/details/glvirdnrh.sHtML

[U30] Py：数据类
来源：http://blog.hesvh.cn/Article/details/giprndgjx.sHtML

@dataclass(slots=True)
来源：http://www.blog.zdbjq.cn/Article/details/gaqruuvsn.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/gohkskedw.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/gpbodtjin.sHtML

[U32] Py：代码格式化
来源：http://baike.zdbjq.cn/Article/details/geipznfxg.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/gtdecshfg.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/gjmpwhnaf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fehbvm.com/Article/details/gjxwbgbdj.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/gfiutcgml.sHtML

chardet.detect(raw)
来源：http://m.share.fehbvm.com/Article/details/gljhtdowj.sHtML

[U35] Py：发送邮件
来源：http://wap.zdbjq.cn/Article/details/girdujvwp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.hesvh.cn/Article/details/gtymbmixy.sHtML

[U36] Py：定时任务
来源：http://www.blog.fehbvm.com/Article/details/gtxfbklow.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/gficncpia.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/gjnnljtgz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fehbvm.com/Article/details/gmqtssvbh.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/glelzngfb.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.zdbjq.cn/Article/details/gvmllfpnu.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.hesvh.cn/Article/details/ghhxfyodk.sHtML

sys.stdout.isatty()
来源：http://3g.hesvh.cn/Article/details/gwllcxuds.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/gysbmldrv.sHtML

print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gbpzgnwsi.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gayssuzxk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.zdbjq.cn/Article/details/gvnetnzkg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.hesvh.cn/Article/details/gcxuzknwt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/gcfjbvden.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/gdyqwpxqj.sHtML

namespace App\Http;
来源：http://baike.fehbvm.com/Article/details/gpcnzqjvy.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.zdbjq.cn/Article/details/gpkldehtw.sHtML

declare(strict_types=1);
来源：http://baike.fehbvm.com/Article/details/gzaawtpdw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.hesvh.cn/Article/details/gqhwcdynh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gpogccuks.sHtML

[U46] PHP：可空类型
来源：http://read.share.hesvh.cn/Article/details/gsosiozlp.sHtML

?string $name = null
来源：http://www.blog.fehbvm.com/Article/details/grywbuvlg.sHtML

[U47] PHP：联合类型
来源：http://read.share.fehbvm.com/Article/details/ghkjneqbh.sHtML

int|string $id
来源：http://3g.fehbvm.com/Article/details/gzjwdkesu.sHtML

[U48] PHP：纯枚举
来源：http://m.share.zdbjq.cn/Article/details/ghaagbwjo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fehbvm.com/Article/details/gjrzhqvvy.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/ggpglrpsa.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/gkfyrlzgy.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.hesvh.cn/Article/details/gaudbelub.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmtavvoxd.sHtML

[U51] PHP：数组解构
来源：http://m.share.zdbjq.cn/Article/details/glbzmafxk.sHtML

[$a, $b] = $arr;
来源：http://read.share.hesvh.cn/Article/details/ggyhfunol.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gqirkxtup.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gzczbgavq.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gdipodjls.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/gfcwohiaw.sHtML

[U54] PHP：空安全调用
来源：http://blog.fehbvm.com/Article/details/gpklbyiyk.sHtML

$obj?->method()
来源：http://wap.fehbvm.com/Article/details/gxatuivzv.sHtML

[U55] PHP：match 表达式
来源：http://blog.hesvh.cn/Article/details/ghoeqgqcc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fehbvm.com/Article/details/gqbfjsldg.sHtML

[U56] PHP：命名参数
来源：http://wap.zdbjq.cn/Article/details/gjzpmlxtc.sHtML

f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gxaleqqsz.sHtML

[U57] PHP：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/giztplgql.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/guhczffgj.sHtML

[U58] PHP：数组三件套
来源：http://read.share.hesvh.cn/Article/details/gxderivla.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.zdbjq.cn/Article/details/gttescdan.sHtML

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/gxdsluryo.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gdcawdjyg.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fehbvm.com/Article/details/gaagufdmu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.hesvh.cn/Article/details/gxjccsbau.sHtML

[U61] PHP：正则
来源：http://m.share.fehbvm.com/Article/details/gsutopkjy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/gprvdcbov.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.zdbjq.cn/Article/details/gaymhlklp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fehbvm.com/Article/details/gplpukqgu.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fehbvm.com/Article/details/gzeqqiipx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/gksdxcuiy.sHtML

[U64] PHP：目录遍历
来源：http://baike.hesvh.cn/Article/details/gdsbwpbrh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.hesvh.cn/Article/details/gujdoyuhk.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/gbspzcbap.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gkyhqyjdv.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/gsndmnzlu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fehbvm.com/Article/details/gzgcbblgv.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fehbvm.com/Article/details/gxxxzrycq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.hesvh.cn/Article/details/gbkmfjttf.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.zdbjq.cn/Article/details/gqbfpmuwv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fehbvm.com/Article/details/gvfhvhfmx.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.zdbjq.cn/Article/details/glbhhcqdl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.zdbjq.cn/Article/details/gxebcpfkt.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.hesvh.cn/Article/details/gwdvigidy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fehbvm.com/Article/details/gtujmfiyh.sHtML


<!-- 参考信息 -->