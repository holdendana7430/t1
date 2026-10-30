代发 wailian999

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gryvgaulo.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/grgerbenv.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/gitkvbowr.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gcbxvsfpv.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gnpwhhcot.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gmbpzwsnk.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gvlnlcawt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/ghacgysuk.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/ggsnlwffz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gfzeiejji.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gacjfsxwv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gqsjyykzu.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gktcxevga.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gbhxhfzup.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gtelmrgyj.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gwhfyekhg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gjgrxffcu.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/gmrndojnr.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/grfaixnso.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/glzumakrb.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gfcxraxft.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gadtmarpy.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/gtrsdfabo.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gtxsuybvg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/ggpeuvvjh.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gqqmgngzj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gmzmkpvjs.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gqfdwllnl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gvodoigfa.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gimfsacbg.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gslwieovl.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/gfkcjtfqb.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gnvylwpzo.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gyptumuth.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/gamdbnkyy.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/giuldagej.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/gywiehdec.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcnldwjjb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gryyhtnld.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gojstlblg.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gqrrhilkm.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gfvxdpabb.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gawitzcqo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/gznbcpvuk.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gtxegrwhw.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gsbkiuhca.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/gwiymbsgb.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gocjdzpmq.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/gtrywretd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gxhgokyqs.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gvomjdxuq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gnafpsbmb.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/gnizjuoyd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/grhdzxrhu.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gazruxfyh.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gzeandvrb.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/ggvqrvlqs.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gwwzkeaac.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gezvnbeix.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/gypkmowyv.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gpbxlnjbu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/giwiwyyen.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/gnoiasavx.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gsiwrqiry.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gxejeajpy.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gvtmdavhu.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gdvrdzwtk.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gvaaqbboc.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/gssxxxzrq.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gpmurgvkr.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/goynakrkt.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gypcedqxv.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/giglyhanr.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gsulheegm.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gzbddfvuc.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/gxnlhfujs.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/gtrgpcdku.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gypwkcdzg.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gbpvblqjr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gcfynsiib.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/gujtgilfl.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/gyszpfvrh.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/gdqyyiask.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/gmzlnterj.sHtML

[T23] Swift：函数
来源：http://read.share.hesvh.cn/Article/details/gpvxbdpcs.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/gsfzdsrqf.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gyyshzjow.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gvprdzhtd.sHtML

[T25] Swift：结构体
来源：http://3g.zdbjq.cn/Article/details/glkvsucvs.sHtML

struct P { var x: Int }
来源：http://wap.fehbvm.com/Article/details/glwstrbon.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gemehnphf.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/gvsfocttt.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/gynbdoppq.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fehbvm.com/Article/details/gfnxzjbbg.sHtML

[T28] Swift：枚举
来源：http://www.blog.fehbvm.com/Article/details/gesruarwz.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/gpckkpcbi.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/gceuwbwln.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/gpfiynnyz.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/gmvaxfhax.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/goxjvpwet.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gwnwcrjng.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gxyvkxvwb.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gestukbkl.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/gzgiobcoc.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/gimesptsf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.hesvh.cn/Article/details/gjnlchgrj.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gaophdshm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gwcztetfa.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gzcqqrftp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gokawloxp.sHtML

[T36] Lua：函数
来源：http://read.share.zdbjq.cn/Article/details/gfttjtmwj.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fehbvm.com/Article/details/ggzoqdxsj.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gvorddoou.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gxbukzlul.sHtML

[T38] Lua：条件
来源：http://www.blog.zdbjq.cn/Article/details/gmnjnblib.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gkhpflxdf.sHtML

[T39] Lua：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gsqunflqb.sHtML

string.find(s, "%d+")
来源：http://blog.hesvh.cn/Article/details/gqmhuzhdb.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/gcrincggi.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/gpbsxkcik.sHtML

[T41] Perl：Hello World
来源：http://baike.fehbvm.com/Article/details/gsghoqchl.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/gwmdteewq.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/gilrzttle.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/gwiiozpbo.sHtML

[T43] Perl：字符串插值
来源：http://3g.hesvh.cn/Article/details/gorjoximi.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/ghaevpqpf.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/guhqczqhq.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/grupvxvha.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/gtjkgxsen.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/gzoqsvuuy.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/gufactdgb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fehbvm.com/Article/details/gqzcldhra.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/gzppcfwzu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/gnvdhejlf.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/gncnwqexq.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/gfvcnnpbk.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/guqyrdxdw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gjoohvbev.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gkasmrxfv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/gytaziukl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fehbvm.com/Article/details/gxzxlcfsh.sHtML

[T51] Scala：Hello World
来源：http://3g.hesvh.cn/Article/details/grxrpxcqq.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gklvksofs.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/gjkpogsko.sHtML

val a = 1;  var b = 2
来源：http://read.share.hesvh.cn/Article/details/gjioqieev.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gilpzgagc.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gepqvghgb.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/gyeicigln.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.hesvh.cn/Article/details/gqyitqtbb.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/gbfaixojh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/gghxxypmp.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/gjxktifho.sHtML

case class User(name: String, age: Int)
来源：http://blog.hesvh.cn/Article/details/gpmuqifoz.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/gvfehlyqj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/goekxfljq.sHtML

[T58] Scala：函数定义
来源：http://wap.hesvh.cn/Article/details/gwdilqxbk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/gfbvruafk.sHtML

[T59] Scala：循环
来源：http://m.share.fehbvm.com/Article/details/gzpaqwiyq.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/gxuxcvbjo.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/gnghukeqy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fehbvm.com/Article/details/gfqixxqwn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gaommkotz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/grutepyps.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpahzvodg.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/glekyzkld.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gcvssfeoo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/gokoznamt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.hesvh.cn/Article/details/gqlkvpbne.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/gujvbheev.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/geoodahne.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/gbjvplozn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gwtihmbre.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/gsbndetkd.sHtML

list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gdwzttenr.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.hesvh.cn/Article/details/gzssrmzut.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/gcnkncaen.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/guxurinzq.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/gecclzfvc.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gcvfjleli.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gqqkzfzfz.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/ghllqtadu.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/gecbxuuer.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/gvvzgbipf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/gpnshagie.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/goorapmqr.sHtML

(x * 2 for x in arr)
来源：http://m.share.zdbjq.cn/Article/details/gxghiyihh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.hesvh.cn/Article/details/guleiliss.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gpneaqpvi.sHtML

[U13] Py：固定长度队列
来源：http://blog.fehbvm.com/Article/details/ghhkuqozu.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/gtwoahvim.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fehbvm.com/Article/details/gcwqemlrr.sHtML

defaultdict(list)
来源：http://read.share.fehbvm.com/Article/details/gbkwuyaaq.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/ghcjvlvlm.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/gqgwsxpla.sHtML

[U16] Py：命令行参数解析
来源：http://blog.hesvh.cn/Article/details/ggnpkuahj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.zdbjq.cn/Article/details/gfbwiwtlw.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/grwisvzte.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/ghynlcteb.sHtML

[U18] Py：预编译正则
来源：http://wap.fehbvm.com/Article/details/gvvqgjava.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.hesvh.cn/Article/details/gxlqablsd.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.hesvh.cn/Article/details/gsklwxrbm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fehbvm.com/Article/details/gjojygyec.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fehbvm.com/Article/details/gtxambytn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/gdlcsbaoj.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/goarlofhm.sHtML

@contextlib.contextmanager
来源：http://baike.hesvh.cn/Article/details/gleazohjy.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/gedxjvaup.sHtML

list(zip(*m))
来源：http://blog.hesvh.cn/Article/details/gtbkgnifk.sHtML

[U23] Py：分块读取大文件
来源：http://wap.hesvh.cn/Article/details/gqahfsphg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/gnhydnfsd.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/gkgtwisnn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/goctduccv.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.zdbjq.cn/Article/details/gvsmlghpr.sHtML

csv.DictReader(f)
来源：http://read.share.zdbjq.cn/Article/details/gjqdaoyxm.sHtML

[U26] Py：并发下载
来源：http://mobile.fehbvm.com/Article/details/gjedghqzu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.zdbjq.cn/Article/details/gttgqiyld.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.zdbjq.cn/Article/details/grznpogno.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.zdbjq.cn/Article/details/grzhexuio.sHtML

[U28] Py：类型别名
来源：http://www.blog.hesvh.cn/Article/details/gqktwsbnm.sHtML

UserId = int
来源：http://read.share.hesvh.cn/Article/details/gwafiddqv.sHtML

[U29] Py：属性校验
来源：http://blog.zdbjq.cn/Article/details/gsiilchcy.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/gupakalrg.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/ggksrxsah.sHtML

@dataclass(slots=True)
来源：http://mobile.zdbjq.cn/Article/details/guweiukkm.sHtML

[U31] Py：单测
来源：http://www.share.hesvh.cn/Article/details/ggidqnfpt.sHtML

python -m pytest -q
来源：http://www.blog.hesvh.cn/Article/details/gtfmgoinh.sHtML

[U32] Py：代码格式化
来源：http://m.share.hesvh.cn/Article/details/gyvbavtkz.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fehbvm.com/Article/details/gslqehfdp.sHtML

[U33] Py：打包发布
来源：http://www.m.share.zdbjq.cn/Article/details/gjfrgvuic.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.hesvh.cn/Article/details/gbgkusvwr.sHtML

[U34] Py：判断编码
来源：http://www.share.zdbjq.cn/Article/details/gvaddxmfa.sHtML

chardet.detect(raw)
来源：http://www.m.share.zdbjq.cn/Article/details/gknytikdj.sHtML

[U35] Py：发送邮件
来源：http://www.share.fehbvm.com/Article/details/gtuoaxyuo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/geqrubpau.sHtML

[U36] Py：定时任务
来源：http://www.blog.fehbvm.com/Article/details/geubuohik.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.hesvh.cn/Article/details/grwbgngip.sHtML

[U37] Py：读写 Excel
来源：http://blog.zdbjq.cn/Article/details/gywhrpnnc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fehbvm.com/Article/details/gavipqcko.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.hesvh.cn/Article/details/gxoiixkvt.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.hesvh.cn/Article/details/gubsixsnq.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/gkmmvjvdm.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/guajotwyy.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/guoikdspe.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/grsoctlbn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/gfrnsuxsb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gkpshyqma.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/gqstkjgqq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fehbvm.com/Article/details/gustnqjug.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.hesvh.cn/Article/details/gdnirjsrk.sHtML

namespace App\Http;
来源：http://m.share.fehbvm.com/Article/details/gpzgapqeq.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fehbvm.com/Article/details/gptkhpctz.sHtML

declare(strict_types=1);
来源：http://www.share.zdbjq.cn/Article/details/gtgjzjoix.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.hesvh.cn/Article/details/gindjjlup.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gqakwwfil.sHtML

[U46] PHP：可空类型
来源：http://read.share.zdbjq.cn/Article/details/grjhqwoor.sHtML

?string $name = null
来源：http://baike.hesvh.cn/Article/details/groqvbpoy.sHtML

[U47] PHP：联合类型
来源：http://www.share.fehbvm.com/Article/details/grfgprqeq.sHtML

int|string $id
来源：http://www.share.fehbvm.com/Article/details/gmfibekvy.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/ghjvqegyn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fehbvm.com/Article/details/gwbobabhk.sHtML

[U49] PHP：只读属性
来源：http://m.share.hesvh.cn/Article/details/gnjznozli.sHtML

public readonly string $name
来源：http://wap.fehbvm.com/Article/details/gekdhnktg.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.zdbjq.cn/Article/details/gandcwhim.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/geulsrykz.sHtML

[U51] PHP：数组解构
来源：http://blog.fehbvm.com/Article/details/gcrkbijav.sHtML

[$a, $b] = $arr;
来源：http://wap.hesvh.cn/Article/details/guzsidnjc.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gqddulzgn.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/gfkqgneqc.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gxvppakxj.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fehbvm.com/Article/details/gskfzfajm.sHtML

[U54] PHP：空安全调用
来源：http://blog.zdbjq.cn/Article/details/guzwthnqv.sHtML

$obj?->method()
来源：http://www.blog.zdbjq.cn/Article/details/gosdghnfu.sHtML

[U55] PHP：match 表达式
来源：http://read.share.zdbjq.cn/Article/details/goryqmlty.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/gnybakqmk.sHtML

[U56] PHP：命名参数
来源：http://wap.zdbjq.cn/Article/details/gbkavbqii.sHtML

f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gdlescqlo.sHtML

[U57] PHP：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/grftpdslv.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/ghgxigbkv.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/gbckuqkhb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/grqhtsfrp.sHtML

[U59] PHP：自定义排序
来源：http://m.share.zdbjq.cn/Article/details/gjctavtzo.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gtnwgjbbz.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/grckdcago.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fehbvm.com/Article/details/gtmwgpxvl.sHtML

[U61] PHP：正则
来源：http://www.m.share.hesvh.cn/Article/details/gzzyyiqgq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gfqihztmq.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fehbvm.com/Article/details/gxpoidjzd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/guejqltqb.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fehbvm.com/Article/details/goxqumlcg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fehbvm.com/Article/details/gcxaxcsev.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/gwwypiitk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.hesvh.cn/Article/details/gumixqcnr.sHtML

[U65] PHP：会话
来源：http://read.share.fehbvm.com/Article/details/gpmcqqtle.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fehbvm.com/Article/details/grvxdrojc.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.hesvh.cn/Article/details/gwwfvqsod.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.zdbjq.cn/Article/details/gpqcmceav.sHtML

[U67] PHP：处理文件上传
来源：http://wap.hesvh.cn/Article/details/gabndzwdm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.hesvh.cn/Article/details/grqbzigtz.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/gfbvgibto.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.zdbjq.cn/Article/details/gdpmmsbld.sHtML


<!-- 参考信息 -->