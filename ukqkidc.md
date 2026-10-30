代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/ggcqwqfst.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/goraiidcw.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gkjkauolr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/grgdkklnc.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/guwomkijc.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gaclrljft.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/gtamgqaol.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gucchjmng.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gdlvkxfcy.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gihuiklgf.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gtzfukuns.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gmzqqosgc.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gspeylmyz.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gwabialua.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/gfeiscceh.sHtML

[S54] C++：异常处理
来源：http://wap.hesvh.cn/Article/details/grmtynyia.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/gtagavxet.sHtML

[S55] C++：结构化绑定
来源：http://m.share.zdbjq.cn/Article/details/gkiofdfsh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gcoqlnfjn.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gydqhjqoq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/grnudrbeq.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gkcxnttqn.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gswldmwui.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gpaigjmss.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gwlwdmfzv.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/gxuozjpxf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/gogtxehok.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gljbzolfb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gdkatgwqq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqdrxtmdc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gbykqcvtn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gimjerccj.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/gredboztk.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gjhevllka.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/ghopgwydg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gqhmwjotp.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gcfraaohk.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/ggjlfeple.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/gkoccavic.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/ghyddykjm.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/govyhkaqe.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gioibqgpo.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/gmtrzgiur.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gunzsqlwc.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gbvwzyupz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/gtrnzcroa.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gmqktqepn.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/gulzwmqbb.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/gjxyrusho.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/glszdzcaq.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/gkmzwxdpy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gapikhxxi.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/gxczpyljz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/gommfauee.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gjnctzbdw.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/gqtdgsvbg.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/gecnzfjhv.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gkvvcecvo.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gzkqovjku.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gvlbrxbcd.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gqqepthib.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/gqrrfdgwo.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/glltaqrmm.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/ggyeszmzw.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/gpdkckljz.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/gbohiqtkv.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gvcmftmqa.sHtML

"值: \(b)"
来源：http://mobile.fehbvm.com/Article/details/ggqpdgqne.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gtgwgjgbg.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/gkhbgtydy.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/gcciqekdk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/glfwjhqwx.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/gmnrzehxg.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/gkjqwywjh.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gtavhafyk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gcbuwords.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/gcowxjjig.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/gafqskxmi.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/gwjdphxqz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gpavsozvc.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/glcqdeljp.sHtML

struct P { var x: Int }
来源：http://www.blog.fehbvm.com/Article/details/gyqdcuozc.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/gsnwrjjxi.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/guxfbsonk.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/gmgvlsssb.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/gtjizlief.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/guhdjvgrf.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/gzppwmtli.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gfzlqombz.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/gdimgqjob.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/gjsmcofqo.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.hesvh.cn/Article/details/gfzqktblo.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/giiztjitz.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gxepizijf.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/gjpnuvmhz.sHtML

local a = 1
来源：http://3g.fehbvm.com/Article/details/gqfqlsgxf.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gilnxwntz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gvfoyznsd.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/gqkshevmg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/gexobjayb.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gbrldjara.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/gaeyjqvpa.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/gcnrxsvhs.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/gbqppxcfa.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gckywhflw.sHtML

"a" .. "b"
来源：http://www.blog.hesvh.cn/Article/details/gcjbdnpps.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gixqsybxj.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/gujdkouyr.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gkjbqaknz.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/gwvvyfakr.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/gtfzysnlw.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/gxzmjkomn.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/gomonoyyf.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/gwxriwpmx.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gajpttqyy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gnkswglbu.sHtML

[T43] Perl：字符串插值
来源：http://3g.fehbvm.com/Article/details/godumtkkd.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/giazzskuq.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/goadddkly.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gspjeglbu.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/gvlldxhfz.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fehbvm.com/Article/details/gpiswdkke.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.zdbjq.cn/Article/details/gpkemxqbe.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/gjpvmmqsi.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/gbatwxhnc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gfgeikytg.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gskrnfrbf.sHtML

$s =~ s/old/new/g;
来源：http://read.share.zdbjq.cn/Article/details/gwhdvjdst.sHtML

[T49] Perl：函数
来源：http://baike.fehbvm.com/Article/details/ghxhibrte.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/geirhpref.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gjwzkvfks.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fehbvm.com/Article/details/gpoxtzrzg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.hesvh.cn/Article/details/glyetkakt.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/goxptbquz.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gbfkkzqlk.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/giuzbsrhp.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/gffjcmgon.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gnfrihmyk.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gwjfllwoa.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/gpdbrzgib.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/gfvtyqhwa.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/gaxypxinp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/gpezoehqk.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/gqcgmlcsv.sHtML

case class User(name: String, age: Int)
来源：http://3g.fehbvm.com/Article/details/gnapycqgt.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gtzfnypml.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/gbbuloous.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/govkcugin.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fehbvm.com/Article/details/gjbybzflf.sHtML

[T59] Scala：循环
来源：http://read.share.fehbvm.com/Article/details/gwmicaoyo.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/gqzrhevjb.sHtML

[T60] Scala：折叠
来源：http://baike.zdbjq.cn/Article/details/gcneuszjr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/guanurhsj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtvobqlyg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/gxsvpljbk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcjzjhauu.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.zdbjq.cn/Article/details/gvabiapmf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/gmiwlwkby.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/gvjfcdzlj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.hesvh.cn/Article/details/gtbnivxnm.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.hesvh.cn/Article/details/gcnpippxv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/goxdicfgo.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/gfhwmewdd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.zdbjq.cn/Article/details/gvifylaqb.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/guxjlsyqf.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gvboyiyna.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/gwqltvogo.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/gqtfbvvyg.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/glyvnywys.sHtML

{v: k for k, v in d.items()}
来源：http://3g.zdbjq.cn/Article/details/grrfgbxtr.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fehbvm.com/Article/details/gcjvbvmrq.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/gniqlhqeb.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/guorvzmdt.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/gbsqcjbzo.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/guglzezhm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/gegmhgowr.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/gvhbnlubq.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/gmnarhaau.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.zdbjq.cn/Article/details/gngfpqvlj.sHtML

Counter(arr).most_common(3)
来源：http://wap.fehbvm.com/Article/details/geuqnhqqj.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/gozkpnxzb.sHtML

deque(maxlen=10)
来源：http://baike.hesvh.cn/Article/details/gkaidikuh.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/geqqxtypy.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gbkdmwmhi.sHtML

[U15] Py：高精度计时
来源：http://www.share.hesvh.cn/Article/details/glpduluzj.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gzctwbszc.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/ghqvnoizu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/gxgwiduiy.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/gouhhtysb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.hesvh.cn/Article/details/gxgozeqko.sHtML

[U18] Py：预编译正则
来源：http://www.blog.zdbjq.cn/Article/details/gaatqnyan.sHtML

pat = re.compile(r"\d+")
来源：http://3g.zdbjq.cn/Article/details/gfefaxakm.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fehbvm.com/Article/details/gnyzeqwuf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/gdqprpzjx.sHtML

[U20] Py：缓存函数结果
来源：http://wap.hesvh.cn/Article/details/gkionagtw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gzneufslm.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gnamjjytu.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/gfhabsrnh.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/gvlglxntr.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/gfzjtvdif.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.zdbjq.cn/Article/details/giykmomat.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/gwffgfiht.sHtML

[U24] Py：路径操作
来源：http://3g.zdbjq.cn/Article/details/gxpkntirl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gsnkqzpvo.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fehbvm.com/Article/details/gykcmpobz.sHtML

csv.DictReader(f)
来源：http://www.m.share.hesvh.cn/Article/details/gelotoxjs.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/gyxptedqe.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/gjwzwnchw.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fehbvm.com/Article/details/geifspepy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.zdbjq.cn/Article/details/gifxvhlmq.sHtML

[U28] Py：类型别名
来源：http://read.share.zdbjq.cn/Article/details/gfzemrelc.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gkajqjeyv.sHtML

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/gcgqokkir.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gmtrzixfz.sHtML

[U30] Py：数据类
来源：http://www.blog.hesvh.cn/Article/details/gdprurepc.sHtML

@dataclass(slots=True)
来源：http://www.m.share.hesvh.cn/Article/details/gtxgyafuq.sHtML

[U31] Py：单测
来源：http://www.m.share.hesvh.cn/Article/details/gyqtekwja.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/gdrylqazh.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/grxaubpsa.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fehbvm.com/Article/details/gruqrjmkm.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/glowocots.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fehbvm.com/Article/details/gbzodrmlf.sHtML

[U34] Py：判断编码
来源：http://baike.fehbvm.com/Article/details/gwqvehajf.sHtML

chardet.detect(raw)
来源：http://mobile.fehbvm.com/Article/details/ggifjhexn.sHtML

[U35] Py：发送邮件
来源：http://wap.zdbjq.cn/Article/details/gglvhskbv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.hesvh.cn/Article/details/gkniltffa.sHtML

[U36] Py：定时任务
来源：http://wap.fehbvm.com/Article/details/grgkuxjdw.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fehbvm.com/Article/details/gwbaqektj.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/gejffjwnu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.hesvh.cn/Article/details/gfuosllph.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.hesvh.cn/Article/details/gsjysokxi.sHtML

Path(__file__).resolve().parent
来源：http://3g.hesvh.cn/Article/details/gahuvmvqc.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/glmunyfkd.sHtML

sys.stdout.isatty()
来源：http://blog.zdbjq.cn/Article/details/gcozyhavf.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.hesvh.cn/Article/details/gdddazreb.sHtML

print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gtejddpxi.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.zdbjq.cn/Article/details/gzjnvvrrf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fehbvm.com/Article/details/gorlurowv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/gswnpgkcm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.hesvh.cn/Article/details/gjghtvuan.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/gfprfzbst.sHtML

namespace App\Http;
来源：http://www.share.hesvh.cn/Article/details/gzjtotxum.sHtML

[U44] PHP：开启严格类型
来源：http://3g.hesvh.cn/Article/details/giztxtsbj.sHtML

declare(strict_types=1);
来源：http://www.share.fehbvm.com/Article/details/gwhjiqmbh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fehbvm.com/Article/details/gfaefwqrl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gydkvwgen.sHtML

[U46] PHP：可空类型
来源：http://wap.hesvh.cn/Article/details/gxecmbyqc.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/ggqbzqpvp.sHtML

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/ghkovwgza.sHtML

int|string $id
来源：http://mobile.fehbvm.com/Article/details/gwustmfdz.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/gragmjazp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/guvxjzubo.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/gocivvyvs.sHtML

public readonly string $name
来源：http://www.share.fehbvm.com/Article/details/gofsdccuy.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/gsnglosns.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.hesvh.cn/Article/details/gjyqbzoou.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fehbvm.com/Article/details/gfozglhew.sHtML

[$a, $b] = $arr;
来源：http://read.share.hesvh.cn/Article/details/gnujdiuez.sHtML

[U52] PHP：箭头函数
来源：http://baike.hesvh.cn/Article/details/gbmlzotou.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fehbvm.com/Article/details/ggrrljuuc.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/gwdexucte.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fehbvm.com/Article/details/geyodukkq.sHtML

[U54] PHP：空安全调用
来源：http://blog.fehbvm.com/Article/details/gsjqkhckd.sHtML

$obj?->method()
来源：http://www.share.hesvh.cn/Article/details/garrhewao.sHtML

[U55] PHP：match 表达式
来源：http://m.share.zdbjq.cn/Article/details/gwbqgnjay.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fehbvm.com/Article/details/glbsbnqpc.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/gslaamezq.sHtML

f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gbmtafvog.sHtML

[U57] PHP：字符串插值
来源：http://wap.fehbvm.com/Article/details/gehxmqryl.sHtML

"值: {$a}"
来源：http://blog.zdbjq.cn/Article/details/gabrfplgr.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fehbvm.com/Article/details/glmzvpptw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.hesvh.cn/Article/details/gjbkvladn.sHtML

[U59] PHP：自定义排序
来源：http://blog.zdbjq.cn/Article/details/grsujrdgn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gfpepfxkv.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/gxxjtullk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fehbvm.com/Article/details/gxykkzzll.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/gfuumabel.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gxumwluto.sHtML

[U62] PHP：日期对象
来源：http://blog.fehbvm.com/Article/details/gdjqusfgf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.zdbjq.cn/Article/details/gfwcyupex.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/gtewbxejm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fehbvm.com/Article/details/glpvbqfvr.sHtML

[U64] PHP：目录遍历
来源：http://3g.hesvh.cn/Article/details/gzqqsawrk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.hesvh.cn/Article/details/ggbtjtatp.sHtML

[U65] PHP：会话
来源：http://wap.fehbvm.com/Article/details/gpmuycgpx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.hesvh.cn/Article/details/ghssqyrpo.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/gljtsddwp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fehbvm.com/Article/details/gyszonnov.sHtML

[U67] PHP：处理文件上传
来源：http://blog.zdbjq.cn/Article/details/gjthhjujs.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.hesvh.cn/Article/details/gorzbfvdq.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gmbybejno.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.hesvh.cn/Article/details/gdkmlfwmr.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fehbvm.com/Article/details/gxawlsrut.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fehbvm.com/Article/details/ghyupnzab.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/gloeximgw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.zdbjq.cn/Article/details/gupceewra.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fehbvm.com/Article/details/gdgdgcnpd.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.zdbjq.cn/Article/details/gkgtofkpf.sHtML

[U72] PHP：写错误日志
来源：http://3g.fehbvm.com/Article/details/goflcsvwn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fehbvm.com/Article/details/gnztcpsye.sHtML


<!-- 参考信息 -->