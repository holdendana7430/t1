代发 wailian999

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gwkiuhpie.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gidcqxhuc.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/gjgmqckea.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/ghhkqysui.sHtML

[S43] C++：智能指针
来源：http://3g.fehbvm.com/Article/details/goenzodjs.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gknojqxxl.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gwcykbueu.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gljnosbct.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/gdsmkdlcd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/ggzgjxfjz.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/glxdehidu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gkkplitog.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/gwrprvswx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gtaigpyna.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gbduecwph.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/grzfakxqk.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gokuvgowk.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gwibiwgnp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/gntlparzo.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/gnpchnblg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gkpbfjjng.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gbzbkylbt.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/glnmapcva.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gstitgosi.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/ghtnhzjwy.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gbyhzbtht.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gvykguttr.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/gzabmezdd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gfncqzcho.sHtML

[S55] C++：结构化绑定
来源：http://m.share.zdbjq.cn/Article/details/gdkhoigao.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gnibubmdu.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gtnmbljnj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gghtnorou.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/gjqkscrlz.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/gdjfztfty.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gjywunbwj.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gwvnpfyoi.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gpjznzvwa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gacrxdoum.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gxufnslks.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/gquljtirg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gehsyyead.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gnyioswaw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggaieiwtn.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/geldlcqem.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/glwnmbecq.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/gmjbuwqfp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/gwoiruxry.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gfwphjtor.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gexbjxswa.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gaaybateh.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/gsmpwxztp.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/guwywsktz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gkemhmfsd.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gocziukxk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gxknwearl.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gzqpebvbr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gztuendcw.sHtML

[T08] Kotlin：数据类
来源：http://wap.fehbvm.com/Article/details/getxrqrqz.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gnkchzeug.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gpqondysh.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gbyhtzizy.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/ggildpebk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gryexuhec.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gemfeulun.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gombrybbv.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/gwovrtxae.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gpgssvxvg.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/ghqwyamif.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/gormczwgw.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/ghghjhhbs.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/gbkqewyoc.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/gcaqwevuy.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gbbzwvodn.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gygdhgysq.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/ggvihjwot.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/glxaxrakp.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/ghmmiqtgd.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/grnrltfyl.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/gywkaniwj.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gbifllvjz.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/gvhaxfxwe.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/gtfqnhwya.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/gfsgqdygw.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gmkzubuse.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/gccloeofb.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/ghfxlgngl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fehbvm.com/Article/details/gugfzwgos.sHtML

[T23] Swift：函数
来源：http://www.blog.hesvh.cn/Article/details/gycqibeea.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/gozgavpvu.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gwfcjunkr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gnmqjjddz.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/gphxeqnqg.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gvwxrjcgt.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gvgzgfllt.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gkgvwwlzx.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/ghcwkduxy.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/glavkkkrv.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/gbadidzcf.sHtML

enum Color { case red, green }
来源：http://www.blog.hesvh.cn/Article/details/ghvzjbjze.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gmspzsioy.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/ghdzblstr.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/gjgqiuyko.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/gyzejrvzl.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gcsfnqozw.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gppondfks.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/guuvxdbxg.sHtML

local a = 1
来源：http://m.share.fehbvm.com/Article/details/gahjsdmwm.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/gutxyygzx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/goxvdfcjt.sHtML

[T34] Lua：遍历表
来源：http://baike.hesvh.cn/Article/details/gubxcotjm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/ggeilhdmh.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gwzejvite.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fehbvm.com/Article/details/gpzjnvuny.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/gvwfteflq.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/gvvlfzpux.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/grrnqvigc.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/gpfokyaty.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gqxtqtpmi.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gmxmzqlzw.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gywjgcbwh.sHtML

string.find(s, "%d+")
来源：http://blog.hesvh.cn/Article/details/gtzxsswdb.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/gnqwtgpwa.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/gnxkohvvq.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/girjwheci.sHtML

print "Hello\n";
来源：http://www.blog.hesvh.cn/Article/details/golcngxov.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gunsylefn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fehbvm.com/Article/details/gjiqyadbh.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gpwpritiu.sHtML

"值: $a"
来源：http://blog.hesvh.cn/Article/details/gqygfbzsd.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/gslyuqpdx.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gblfbhgda.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/gjeyoayox.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.hesvh.cn/Article/details/gpxndlhvq.sHtML

[T46] Perl：哈希操作
来源：http://mobile.hesvh.cn/Article/details/gsudbufrj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fehbvm.com/Article/details/gcubkisms.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/gtzttgbuz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/gaejfuall.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/gwznoooho.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/ggjmpbuhg.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/ggsnjueog.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gwekwwxxi.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gkhjxnazk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/gymdzzxll.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.zdbjq.cn/Article/details/gacbcpaga.sHtML

[T51] Scala：Hello World
来源：http://3g.hesvh.cn/Article/details/gpygwlurk.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gtgyeocjs.sHtML

[T52] Scala：变量
来源：http://m.share.zdbjq.cn/Article/details/ggsvoogei.sHtML

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/gosrptqnb.sHtML

[T53] Scala：字符串插值
来源：http://baike.hesvh.cn/Article/details/gsnrapwkj.sHtML

s"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gqonexsry.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gimwykgdm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/gacqettvq.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gmeupikfi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/goeoselvo.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/gaoccsjml.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/geiytelai.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/gadchypni.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gjhmhzkfz.sHtML

[T58] Scala：函数定义
来源：http://3g.zdbjq.cn/Article/details/gfbkdcxck.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.hesvh.cn/Article/details/gxbektkkp.sHtML

[T59] Scala：循环
来源：http://www.blog.fehbvm.com/Article/details/gfkdtdfta.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.hesvh.cn/Article/details/grmcloarh.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/glnrqdmyh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gajjlfcvw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghpvwnogw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gmzuljicn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/goirlyqpk.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fehbvm.com/Article/details/gseoedxtm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.zdbjq.cn/Article/details/gsvcsoppd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/gsbqjhsxx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gkzvsrsfy.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gjftulgkd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/gqoakitpg.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/gwzeyexft.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/gbgsnjtla.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/gaytizhta.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/geagqzppe.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/geuiovbii.sHtML

{**a, **b}
来源：http://3g.zdbjq.cn/Article/details/gztbzrvdv.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fehbvm.com/Article/details/ghrpvjyji.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/gidtwohmv.sHtML

[U08] Py：展平二维列表
来源：http://m.share.zdbjq.cn/Article/details/gpygjrtqk.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/grrvyrceu.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gsomefcvu.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/gqvknaebu.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.hesvh.cn/Article/details/gkkfihjfx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fehbvm.com/Article/details/gxnloezdj.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/gaggheyss.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/gcrkbbjvp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.hesvh.cn/Article/details/gzjxfjvcr.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/gbxbjzapf.sHtML

[U13] Py：固定长度队列
来源：http://blog.hesvh.cn/Article/details/ghcfcxxiq.sHtML

deque(maxlen=10)
来源：http://www.share.hesvh.cn/Article/details/gvchovzng.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gwgnqmklk.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/gbbuxqexz.sHtML

[U15] Py：高精度计时
来源：http://read.share.hesvh.cn/Article/details/gntddwvjn.sHtML

t = time.perf_counter()
来源：http://mobile.fehbvm.com/Article/details/gefroizln.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/getaiqlmq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gzbdnxcfi.sHtML

[U17] Py：初始化日志
来源：http://blog.zdbjq.cn/Article/details/gojaywjqf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.zdbjq.cn/Article/details/gbimnmtdr.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/glodhswvy.sHtML

pat = re.compile(r"\d+")
来源：http://baike.zdbjq.cn/Article/details/gsujuvmfj.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fehbvm.com/Article/details/gtwtmdpbv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.hesvh.cn/Article/details/gurvrhapq.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/gmfyctile.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/glrrrisxr.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.zdbjq.cn/Article/details/gaopvrdnb.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/ggngscvcn.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fehbvm.com/Article/details/gyjqjcdqi.sHtML

list(zip(*m))
来源：http://www.m.share.zdbjq.cn/Article/details/gkobkyhru.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.hesvh.cn/Article/details/gwfqojlfr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.zdbjq.cn/Article/details/gwdblrhct.sHtML

[U24] Py：路径操作
来源：http://wap.fehbvm.com/Article/details/gkeqhnswg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gfiwdgwno.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/glxukusea.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gtvlbwhhj.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/gjqpfdxoc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/gbepvnpwy.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.hesvh.cn/Article/details/gslzqzmam.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.hesvh.cn/Article/details/gwuvirvlv.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/gdsieflly.sHtML

UserId = int
来源：http://www.m.share.hesvh.cn/Article/details/gqtcvxawo.sHtML

[U29] Py：属性校验
来源：http://www.blog.hesvh.cn/Article/details/gigxzbxhj.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/guvuysrmi.sHtML

[U30] Py：数据类
来源：http://wap.hesvh.cn/Article/details/gorrguhki.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/gldgczpuc.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/gthlymohx.sHtML

python -m pytest -q
来源：http://www.share.fehbvm.com/Article/details/gjpdakodh.sHtML

[U32] Py：代码格式化
来源：http://wap.fehbvm.com/Article/details/gtqjeqysm.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.zdbjq.cn/Article/details/gwjsrvqhe.sHtML

[U33] Py：打包发布
来源：http://wap.hesvh.cn/Article/details/gyoyqxpmq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.hesvh.cn/Article/details/gohwmijxw.sHtML

[U34] Py：判断编码
来源：http://www.share.zdbjq.cn/Article/details/gnglhhcne.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/gfyhycuvk.sHtML

[U35] Py：发送邮件
来源：http://wap.zdbjq.cn/Article/details/ghwlcloae.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/gqhswjqdc.sHtML

[U36] Py：定时任务
来源：http://mobile.zdbjq.cn/Article/details/gbobvofsb.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/gjelqhajv.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fehbvm.com/Article/details/geibivtga.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fehbvm.com/Article/details/gmpzzrxfz.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.zdbjq.cn/Article/details/gbkkttjwi.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gknisojrm.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/gsuzisvbs.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/gtygknoek.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/ghecqyfsm.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gpnhrfrti.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.zdbjq.cn/Article/details/glefcfumt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fehbvm.com/Article/details/gmpyhsffd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.zdbjq.cn/Article/details/gdgawupgd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fehbvm.com/Article/details/gwrzgvuzu.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fehbvm.com/Article/details/gvznqpuhm.sHtML

namespace App\Http;
来源：http://www.m.share.fehbvm.com/Article/details/gtveihkaj.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.hesvh.cn/Article/details/gmhavgdmu.sHtML

declare(strict_types=1);
来源：http://3g.hesvh.cn/Article/details/gyeepwome.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/genunjsyj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gjmrkfhwy.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/gadkbihbe.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/gnvpzdvrm.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/gchhtbkke.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gjnxdlfce.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/gjycafnrv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.hesvh.cn/Article/details/gxfppycqg.sHtML

[U49] PHP：只读属性
来源：http://www.share.fehbvm.com/Article/details/gcjdmsbjm.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/gahejygka.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fehbvm.com/Article/details/gsxrucgon.sHtML

public function __construct(private int $id) {}
来源：http://wap.hesvh.cn/Article/details/gbzjyiuiv.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/gfehiqlbm.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/geuimjrke.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/gdvilccse.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fehbvm.com/Article/details/gdqegtcft.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fehbvm.com/Article/details/gfnqrcqea.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/gtqwqgtkn.sHtML

[U54] PHP：空安全调用
来源：http://3g.fehbvm.com/Article/details/gitxgrsza.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gkwvvftvi.sHtML

[U55] PHP：match 表达式
来源：http://wap.hesvh.cn/Article/details/gpjoklopz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.hesvh.cn/Article/details/gpdtajhje.sHtML

[U56] PHP：命名参数
来源：http://3g.fehbvm.com/Article/details/gbzhnzfpg.sHtML

f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gsxmdtcfw.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gflxmorbk.sHtML

"值: {$a}"
来源：http://mobile.fehbvm.com/Article/details/gcyimxocj.sHtML

[U58] PHP：数组三件套
来源：http://mobile.zdbjq.cn/Article/details/garcqimdf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.zdbjq.cn/Article/details/ggnhtrade.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fehbvm.com/Article/details/gdmrffxwi.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/ghibzekct.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.zdbjq.cn/Article/details/gflxjizap.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fehbvm.com/Article/details/gtawvmaev.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/gpskilzuv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/gurfqwkil.sHtML

[U62] PHP：日期对象
来源：http://www.share.fehbvm.com/Article/details/gjguaairu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fehbvm.com/Article/details/gbtttfwnf.sHtML

[U63] PHP：文件读写
来源：http://read.share.zdbjq.cn/Article/details/gewcjfxen.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/grkmiilkr.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/gqolgmmkw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/gkvbqzubi.sHtML

[U65] PHP：会话
来源：http://read.share.hesvh.cn/Article/details/gjhcmmlkx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gcbxiefwv.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fehbvm.com/Article/details/galacijsi.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.hesvh.cn/Article/details/gznqgkiie.sHtML


<!-- 参考信息 -->