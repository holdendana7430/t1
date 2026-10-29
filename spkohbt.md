代发 wailian999

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gpqvhcuve.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gqyyakwsn.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gpdrqzqde.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/gtdyyqmyy.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/gvpldsdff.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/gvsferxjr.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/gxqgwwklx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/ghyjkznmo.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gmkazynkj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/guciqjvfa.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gdbqqtezd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gdvlamnia.sHtML

while (std::getline(in, line)) { }
来源：http://baike.hesvh.cn/Article/details/gdqewlbfv.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gxdrbajsp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gluvwjhvx.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gopdqnufa.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gyshauvnl.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/ggfkghfmf.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gltehprqe.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gsoiwarwj.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gptkbkgch.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gvsbruwbj.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gyjyhsavk.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/gncflkmqb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/giufseldx.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/gozhnliyo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/gvqqziklw.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/gxuaraicq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gxdstovmj.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gvrjrayjs.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/grmtjitwi.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/glftxyjzh.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gdejnaytu.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/goxjigvxo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/gdwsiskmb.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gdmcsbevm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/gfpmkmvil.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjcrhqibi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gjwoxwstx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gezumvmni.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gplvwaysu.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/ghocvcscm.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gbphlbdwr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/gkpjvconi.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/gjlnvwaky.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gotictlny.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gkijgibpp.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gfkaakwpi.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gcbuipqwb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/gcijdpvvl.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gwlxxjvxe.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/gsgkqcwpn.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gfkmyymma.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/gdnxenpwf.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gqyeukcmr.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/gljkbeiga.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gvvqlvqlj.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/ghhwsldsx.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gwhzeumqj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gkkzgmsbl.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/gznkfdsid.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gpfnfqejd.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/gfshltfxc.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/grfjsqzjh.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/gadowfbdc.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/ggqozqomr.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/giwjhhcdi.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/gjkiiboqb.sHtML

[T15] Kotlin：接口
来源：http://blog.hesvh.cn/Article/details/gxzafpgxg.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/gzctoeprm.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gxoxqpctp.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/ghcwmanqc.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/gtppoopxr.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/gvhmenvgg.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/ghnblmkzt.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/gbuatlleu.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/ggazoqqzb.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/ggndfyzmr.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/gjuhwxzag.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.hesvh.cn/Article/details/gycalpdda.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/gucgfnsyn.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/geyezjstn.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gmyebipmq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gehsxgils.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/gmgjjegum.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gzvfvkerl.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/gbxnehjuj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gjikrigag.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gznslofuo.sHtML

struct P { var x: Int }
来源：http://www.blog.fehbvm.com/Article/details/gbndwirtz.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/gtpgjbavs.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/ghwlqllet.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gsmhxsvhd.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/glgmvfspx.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/gesgaqltr.sHtML

enum Color { case red, green }
来源：http://blog.zdbjq.cn/Article/details/gwnlgrcyc.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/grjmegyum.sHtML

guard let x = opt else { return }
来源：http://read.share.zdbjq.cn/Article/details/godqytgaz.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/gpbgawlok.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gylfogdlf.sHtML

[T31] Lua：Hello World
来源：http://m.share.fehbvm.com/Article/details/gorvdkmcu.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/glbwbirkl.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gyeokhvrh.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/giutxqvlv.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/gdwrqkndp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/ggwzbnwxt.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/ggvpnywrb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gjgfmvyow.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/glwcfpnyl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/gdaeisinw.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/gywjixtvl.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gcuxkiyzm.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/ggnurvrhd.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gcjftyskf.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/glfjwqhou.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/gkdqoaigf.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gtvmajoit.sHtML

string.find(s, "%d+")
来源：http://3g.fehbvm.com/Article/details/geybbaffa.sHtML

[T40] Lua：元表
来源：http://read.share.fehbvm.com/Article/details/gsqvtqijv.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gqhmjrjls.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/giiyoqlrn.sHtML

print "Hello\n";
来源：http://mobile.zdbjq.cn/Article/details/gntzwllkb.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/gmaqsnvww.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/gwauaivzc.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/gjwmkabmb.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/goidadjep.sHtML

[T44] Perl：条件
来源：http://read.share.hesvh.cn/Article/details/ggtzmlgym.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fehbvm.com/Article/details/gjxyycnin.sHtML

[T45] Perl：数组遍历
来源：http://m.share.zdbjq.cn/Article/details/gwopnzzjl.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/gohyngqmi.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gbrlyngre.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.hesvh.cn/Article/details/gvczpeuna.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gejwetkdn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gzpoqxsrr.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/gywiewfug.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gsgxzvkab.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/gomwfagww.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gsqpwwxqo.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/goodcibhi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/gtytetgkk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gkbczoqne.sHtML

[T51] Scala：Hello World
来源：http://blog.fehbvm.com/Article/details/gptyyovtn.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gicvznint.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/gleljgatv.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/gyodrdxbt.sHtML

[T53] Scala：字符串插值
来源：http://wap.hesvh.cn/Article/details/gwxublhcu.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gxvyuxacl.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/gfwogmvnd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/gebegijgf.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gzsqlsecl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.zdbjq.cn/Article/details/gmqffzift.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gfzadyytd.sHtML

case class User(name: String, age: Int)
来源：http://www.share.hesvh.cn/Article/details/gkuazpnln.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/ghbhwlain.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/ghbmdhoxn.sHtML

[T58] Scala：函数定义
来源：http://mobile.zdbjq.cn/Article/details/gwylyhvcz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/gwshystco.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gfluigldj.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gllvradrs.sHtML

[T60] Scala：折叠
来源：http://www.blog.zdbjq.cn/Article/details/grlhjxyih.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/guofmouzr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gloqmkzyk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gnagdeegq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnznslcxl.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/gkjnphvau.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/gcmehpqkh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/gzewxksvg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/gybevmlxh.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.zdbjq.cn/Article/details/gficfphmm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/gvlsvbean.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/gaozfxjcl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/gkympgycx.sHtML

[U05] Py：列表去重且保序
来源：http://3g.hesvh.cn/Article/details/gaiaikksw.sHtML

list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gjosubbuh.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gxkcfxgwz.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/gjxxgeali.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/gphvuatam.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/gzpyajkge.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/geldmgqav.sHtML

[y for x in nested for y in x]
来源：http://baike.zdbjq.cn/Article/details/goavixvaw.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/ggupyxquw.sHtML

max(d, key=d.get)
来源：http://www.m.share.zdbjq.cn/Article/details/ghkcqdfjw.sHtML

[U10] Py：按值排序字典
来源：http://3g.fehbvm.com/Article/details/gysqumsmn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.zdbjq.cn/Article/details/gheuthucc.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fehbvm.com/Article/details/golbkllvl.sHtML

(x * 2 for x in arr)
来源：http://www.blog.zdbjq.cn/Article/details/gzapieocf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/gcyjrgjlz.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/gpwkyydsf.sHtML

[U13] Py：固定长度队列
来源：http://read.share.zdbjq.cn/Article/details/gznvlnkqi.sHtML

deque(maxlen=10)
来源：http://m.share.zdbjq.cn/Article/details/gtyxtopfe.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.hesvh.cn/Article/details/gfptuulyx.sHtML

defaultdict(list)
来源：http://blog.fehbvm.com/Article/details/gnwcitzna.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/gkdmasjnf.sHtML

t = time.perf_counter()
来源：http://www.blog.zdbjq.cn/Article/details/gimetkjrp.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/gtpadfbrh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/gnbvpexjp.sHtML

[U17] Py：初始化日志
来源：http://baike.hesvh.cn/Article/details/gppuujhrz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/gxiaeyxjg.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/gstrtcbpc.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gjfhmegcu.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fehbvm.com/Article/details/gofetchvp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.hesvh.cn/Article/details/gpbzzucom.sHtML

[U20] Py：缓存函数结果
来源：http://wap.hesvh.cn/Article/details/gservmmlg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/gfhzpyovv.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/gkldgsxtw.sHtML

@contextlib.contextmanager
来源：http://blog.hesvh.cn/Article/details/gnomqvbuu.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fehbvm.com/Article/details/gocxgyhle.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gxlqjboeb.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/gwbhhkzct.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fehbvm.com/Article/details/grepnbuzx.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/gfdqocmgi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/guqfppyhc.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.hesvh.cn/Article/details/gdhsezhyn.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gcfonyeyt.sHtML

[U26] Py：并发下载
来源：http://www.share.fehbvm.com/Article/details/gboauxjio.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gdytenpzk.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/ggnvulbhv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/gfybspbzw.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/gbrayezmb.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/gvqxfwmeu.sHtML

[U29] Py：属性校验
来源：http://baike.fehbvm.com/Article/details/guyknoebh.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gnfbrzmfb.sHtML

[U30] Py：数据类
来源：http://wap.fehbvm.com/Article/details/gxhwuaniq.sHtML

@dataclass(slots=True)
来源：http://read.share.hesvh.cn/Article/details/gdbmvrnub.sHtML

[U31] Py：单测
来源：http://read.share.fehbvm.com/Article/details/gqakvfudj.sHtML

python -m pytest -q
来源：http://read.share.zdbjq.cn/Article/details/gdugxhilf.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gmhpppbvg.sHtML

ruff format . && ruff check --fix .
来源：http://wap.zdbjq.cn/Article/details/gpfbjhhem.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/ghyfricuy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.hesvh.cn/Article/details/gfowyzkov.sHtML

[U34] Py：判断编码
来源：http://3g.hesvh.cn/Article/details/gmlrkmjvx.sHtML

chardet.detect(raw)
来源：http://blog.fehbvm.com/Article/details/gczymstcr.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gujprsqqb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.zdbjq.cn/Article/details/gfezvyoss.sHtML

[U36] Py：定时任务
来源：http://read.share.zdbjq.cn/Article/details/gcvitgycr.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.hesvh.cn/Article/details/grkrfiwau.sHtML

[U37] Py：读写 Excel
来源：http://www.share.hesvh.cn/Article/details/gnxpfhjqq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/gvurlbzkq.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.zdbjq.cn/Article/details/gyvjnhqlf.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fehbvm.com/Article/details/gnsguvfpu.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/gueidfmhu.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/gtksunhya.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fehbvm.com/Article/details/gjqpuzizo.sHtML

print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gdtxiziza.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.hesvh.cn/Article/details/gvctohvco.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/ghujmaubu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fehbvm.com/Article/details/gjtkjrtxq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/gaqxdmpng.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.hesvh.cn/Article/details/gezshxnld.sHtML

namespace App\Http;
来源：http://wap.fehbvm.com/Article/details/ggfzjvyby.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/gdmmxrkre.sHtML

declare(strict_types=1);
来源：http://read.share.hesvh.cn/Article/details/gdnyfksbe.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.zdbjq.cn/Article/details/gayblxmhw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/guohrtuuv.sHtML

[U46] PHP：可空类型
来源：http://www.share.hesvh.cn/Article/details/gvovmlqat.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/gufjshjgy.sHtML

[U47] PHP：联合类型
来源：http://read.share.zdbjq.cn/Article/details/gkdoenfus.sHtML

int|string $id
来源：http://blog.hesvh.cn/Article/details/gdjuybnog.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/grvceooei.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/gxjekyjme.sHtML

[U49] PHP：只读属性
来源：http://www.blog.hesvh.cn/Article/details/gjbdbawpc.sHtML

public readonly string $name
来源：http://mobile.hesvh.cn/Article/details/gsecflihj.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.zdbjq.cn/Article/details/goghgstad.sHtML

public function __construct(private int $id) {}
来源：http://3g.fehbvm.com/Article/details/gcubcbrup.sHtML

[U51] PHP：数组解构
来源：http://read.share.zdbjq.cn/Article/details/gwvedcsbv.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/grhaukdig.sHtML

[U52] PHP：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gmtepgwqq.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/ganrudhyg.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fehbvm.com/Article/details/gbeahaahx.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.hesvh.cn/Article/details/gtrzdmtwc.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/gqouszzmg.sHtML

$obj?->method()
来源：http://mobile.zdbjq.cn/Article/details/ggcpeymtd.sHtML

[U55] PHP：match 表达式
来源：http://3g.hesvh.cn/Article/details/gqorsrjxg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fehbvm.com/Article/details/ghvqqfbib.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/gtylidtxf.sHtML

f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gqhancnpn.sHtML

[U57] PHP：字符串插值
来源：http://blog.fehbvm.com/Article/details/gwpatydtb.sHtML

"值: {$a}"
来源：http://baike.zdbjq.cn/Article/details/gdntxowqj.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/gjafhvxzb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.zdbjq.cn/Article/details/gnentwuzp.sHtML

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/goqlzvcyg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gemkfmmbh.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/gnugmqchu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fehbvm.com/Article/details/gtkayvqvb.sHtML

[U61] PHP：正则
来源：http://www.blog.hesvh.cn/Article/details/gwizisroq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/guorfilob.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.zdbjq.cn/Article/details/grudufhvh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fehbvm.com/Article/details/gwhrecznc.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/gozpevuvq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.hesvh.cn/Article/details/gruhdshdb.sHtML

[U64] PHP：目录遍历
来源：http://blog.zdbjq.cn/Article/details/grzlbpfyw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.zdbjq.cn/Article/details/gzkhaaxyo.sHtML

[U65] PHP：会话
来源：http://baike.zdbjq.cn/Article/details/gemghrbfl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gvpajeaur.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/gzvkdhmdv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.hesvh.cn/Article/details/gvobqswpg.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fehbvm.com/Article/details/gwgxougct.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.hesvh.cn/Article/details/giymntncz.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.zdbjq.cn/Article/details/gouvqusoi.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/guwkxrjvc.sHtML


<!-- 参考信息 -->