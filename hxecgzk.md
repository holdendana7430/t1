代发 wailian999

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gixcxtode.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gzzdtgdxe.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gwrjdbpgr.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fehbvm.com/Article/details/ghqzjuaow.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/grqswynes.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gtrqclshk.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gdijifbrn.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/ganvhwvmz.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gvtbfdgjb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gzphagjpo.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/gtoycvecs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/ghziulojb.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gqhqalkpe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gfuqlfaaw.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gwritrugv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gncjvhkjt.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gcyhiicsx.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/ggwwmpcwf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/glthwfbgg.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gfamkwuit.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/glhqqcawj.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gvnojfmcc.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/ggnhrhces.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/gvothkjrr.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gdtwkgdzs.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/gvxuiyemx.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gkvclpguq.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gorxvradc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/giuqfretc.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gjibeeree.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/glhahtwko.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/geyphjaey.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gmhoylctk.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gzlbyetcs.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gvbkfttow.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/geswntuvu.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gyhbkratd.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gynvbnmti.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gnpfjjcno.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gvwwpxytf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gkhnetkqn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gofxtqucm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gapadmhge.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjvjyiicj.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gdzczgjhg.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gjkdelchg.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gfaojjrbt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gvxoddkbs.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gwahhfbzk.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gebhdnxls.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/gxznllznu.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gsbwwxyms.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gueznyupw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/gzuyrvswg.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/gmkwxgkbe.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.hesvh.cn/Article/details/grauzveva.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/grzezwvhv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gawtpogjh.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/gpamjmjip.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gagkfldun.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gwaialund.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gnkktxcfl.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gcbqrrzcz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/ggxdmmxfx.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gepzaznrt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/gfaktsmke.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gtxrfpwgx.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gmyfckuvh.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/ggjxstypq.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/gjihwozdm.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/ggvdshean.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/gewzezzpt.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gnbfrlhwk.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/gzvgzfrai.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gpdabfpel.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gmrrxwelb.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/gkbfnzuqk.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/gunhzjwhu.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/geeznbjsa.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/gzqkqymct.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gqflmmuoo.sHtML

if let n = opt { print(n) }
来源：http://mobile.zdbjq.cn/Article/details/glefntjuh.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gvgljbefa.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/grjyavknp.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/gvkvubfcm.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gafzrzxly.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/gfutqqcod.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fehbvm.com/Article/details/gqqyyoddp.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/gsdecfziv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/gsnrmalnf.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/glzphltuy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/gimxinkph.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gqxxjdxjj.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gsilebcjc.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/gtsgcjtdx.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gqlpmpesw.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/gkciqechh.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gbbzolice.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gbvnosxnz.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/gvpdxravv.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/gybutgjna.sHtML

guard let x = opt else { return }
来源：http://www.blog.zdbjq.cn/Article/details/gnioiavgq.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gfdxhtvkk.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/gdkevdivr.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/gynyixsrt.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gnxjmoneo.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gfoquhzti.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/ggqjvpdlf.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/ggoiicwin.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gtzguwnmx.sHtML

[T34] Lua：遍历表
来源：http://www.share.hesvh.cn/Article/details/ghfbbqurm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gtfyvxuhw.sHtML

[T35] Lua：字典表
来源：http://m.share.fehbvm.com/Article/details/gkpajtcez.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/ggnxlexdw.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/gaofhxong.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/gccsbyjpz.sHtML

[T37] Lua：字符串拼接
来源：http://wap.hesvh.cn/Article/details/gvwwludsv.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/gbsxlvkvd.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/gsxemfhze.sHtML

if x > 0 then print("正") end
来源：http://mobile.fehbvm.com/Article/details/govqdmdsl.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gghemompf.sHtML

string.find(s, "%d+")
来源：http://www.blog.fehbvm.com/Article/details/gcjfjwzeh.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/gzlbtujbl.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/gcbqnqbyt.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/gzkmqwcke.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/ghqgjzcoy.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gdkbcyxqm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gtbnbkiwy.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gxumiqfys.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gvngtneuj.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/grdqsonvd.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gtjrhhcnv.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/gunmpxzxq.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/geqhxyvsx.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/goklzjfmq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/ghimbxaug.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/gmkspmynp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/gzewhfchl.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/govejjluo.sHtML

$s =~ s/old/new/g;
来源：http://m.share.hesvh.cn/Article/details/gbdsfxnzm.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/gqudrfeah.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gztvkbrmx.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gtnddsyjx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fehbvm.com/Article/details/gqnanxryg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.hesvh.cn/Article/details/gptlrzgek.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/gcvfcnmes.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gxdsahyeq.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gfescelnl.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/gynwgyzkh.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gvfcplvhi.sHtML

s"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gkdlwwuxh.sHtML

[T54] Scala：集合映射
来源：http://wap.hesvh.cn/Article/details/gdsgzwwsl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/ghjmzsxun.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gbtfmddon.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/gewtojpbv.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/gxrqwwtyz.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/ghfoyonrw.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gdhsepsow.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.hesvh.cn/Article/details/ghpyqhfty.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/gtngegppt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/geztxukyg.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gkyqegtum.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.hesvh.cn/Article/details/gwmmtrqdi.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/gvhqnudog.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gfgiwpunw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvchbmnhi.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/greyhdrmf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwnuilkhm.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/gouoargsv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/gvygxtvjj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/gxucemtii.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.hesvh.cn/Article/details/glcvsfaoc.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.zdbjq.cn/Article/details/gwmfzsdrq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/gvwpbjekp.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gdvwqpuui.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.zdbjq.cn/Article/details/gggeipitb.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.zdbjq.cn/Article/details/ghwyjolcx.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gukbznjdf.sHtML

[U06] Py：合并两个字典
来源：http://www.share.hesvh.cn/Article/details/gtdiylves.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/gswdyhrkh.sHtML

[U07] Py：反转字典键值
来源：http://m.share.hesvh.cn/Article/details/gltcydece.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/gpkfifnlg.sHtML

[U08] Py：展平二维列表
来源：http://blog.fehbvm.com/Article/details/gjpuosgwx.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/gnofoadqq.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.zdbjq.cn/Article/details/gqhxwtrcx.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/gqxpttqkt.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gylbblawu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.hesvh.cn/Article/details/gtlnwaknl.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/geqitirks.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/gifuwdwmu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.zdbjq.cn/Article/details/gsscmvmgh.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/gyvbdqfig.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/gkvicijlg.sHtML

deque(maxlen=10)
来源：http://read.share.zdbjq.cn/Article/details/gvbuevfjx.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gydivzqqr.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/grrtzlavy.sHtML

[U15] Py：高精度计时
来源：http://mobile.fehbvm.com/Article/details/gmofyglzo.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gnegvfacw.sHtML

[U16] Py：命令行参数解析
来源：http://3g.hesvh.cn/Article/details/glutaunqn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/gaxzvvjpy.sHtML

[U17] Py：初始化日志
来源：http://wap.hesvh.cn/Article/details/gakqigvst.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/gtykibriy.sHtML

[U18] Py：预编译正则
来源：http://wap.fehbvm.com/Article/details/gjnigmgrl.sHtML

pat = re.compile(r"\d+")
来源：http://3g.zdbjq.cn/Article/details/gmqlvrgfp.sHtML

[U19] Py：正则替换带回调
来源：http://wap.hesvh.cn/Article/details/gkfgkhjod.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.hesvh.cn/Article/details/gxiefffgl.sHtML

[U20] Py：缓存函数结果
来源：http://blog.zdbjq.cn/Article/details/geqqhevkj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fehbvm.com/Article/details/gnbwbamha.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fehbvm.com/Article/details/gkgstkzqs.sHtML

@contextlib.contextmanager
来源：http://www.m.share.hesvh.cn/Article/details/gmyvfcdzb.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/gjwjckudj.sHtML

list(zip(*m))
来源：http://www.share.fehbvm.com/Article/details/gfazigugj.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gvbqmwgkx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.hesvh.cn/Article/details/gwpzaflgj.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/gbkijewrv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gricpahxn.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gyojjtsxt.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/gqqpqoahs.sHtML

[U26] Py：并发下载
来源：http://m.share.fehbvm.com/Article/details/gpcfjmpge.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/giuzrjfir.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.zdbjq.cn/Article/details/gjxeccmyu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.hesvh.cn/Article/details/gugykcizn.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/gamfopkyj.sHtML

UserId = int
来源：http://mobile.fehbvm.com/Article/details/ghvnnmbax.sHtML

[U29] Py：属性校验
来源：http://wap.hesvh.cn/Article/details/gaubgapwn.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.zdbjq.cn/Article/details/gmotxwgpr.sHtML

[U30] Py：数据类
来源：http://read.share.zdbjq.cn/Article/details/guoszfltw.sHtML

@dataclass(slots=True)
来源：http://wap.hesvh.cn/Article/details/gkfyuajna.sHtML

[U31] Py：单测
来源：http://www.m.share.fehbvm.com/Article/details/gkusuiwmr.sHtML

python -m pytest -q
来源：http://3g.fehbvm.com/Article/details/gjanbotbm.sHtML

[U32] Py：代码格式化
来源：http://blog.fehbvm.com/Article/details/gzhaheqac.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/gtlzttcnu.sHtML

[U33] Py：打包发布
来源：http://m.share.fehbvm.com/Article/details/gryvabtms.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.hesvh.cn/Article/details/grqzwbucj.sHtML

[U34] Py：判断编码
来源：http://www.share.zdbjq.cn/Article/details/gukxykxsu.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/gypkmarum.sHtML

[U35] Py：发送邮件
来源：http://read.share.zdbjq.cn/Article/details/gacxbsjml.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.hesvh.cn/Article/details/gohosseht.sHtML

[U36] Py：定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gncxvxmht.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fehbvm.com/Article/details/gcrisjqzv.sHtML

[U37] Py：读写 Excel
来源：http://blog.fehbvm.com/Article/details/gsnistrje.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fehbvm.com/Article/details/gmgffnpxb.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/gqpmrqijl.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fehbvm.com/Article/details/guiayklss.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.hesvh.cn/Article/details/gzawjrtvg.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/ggkqzeyti.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gztfntbyh.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gbwbhwpew.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.hesvh.cn/Article/details/gvajyuzcm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/gftzxtmbo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.zdbjq.cn/Article/details/gculisuwg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.zdbjq.cn/Article/details/gohyobyye.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/ghrgsxfyn.sHtML

namespace App\Http;
来源：http://www.m.share.zdbjq.cn/Article/details/gqpuftywp.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fehbvm.com/Article/details/gpqhcijhm.sHtML

declare(strict_types=1);
来源：http://www.share.hesvh.cn/Article/details/gbayzsvka.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.hesvh.cn/Article/details/gnbsjmrvr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gjffzgqif.sHtML

[U46] PHP：可空类型
来源：http://wap.fehbvm.com/Article/details/gzouanynv.sHtML

?string $name = null
来源：http://3g.fehbvm.com/Article/details/gtxxojakp.sHtML

[U47] PHP：联合类型
来源：http://mobile.fehbvm.com/Article/details/ggpkyxakl.sHtML

int|string $id
来源：http://mobile.fehbvm.com/Article/details/genaccuff.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/gcpsururd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.hesvh.cn/Article/details/gsthsoaju.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.hesvh.cn/Article/details/gewmusxwq.sHtML

public readonly string $name
来源：http://blog.zdbjq.cn/Article/details/gdeeihhan.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fehbvm.com/Article/details/gvqixfmsz.sHtML

public function __construct(private int $id) {}
来源：http://wap.fehbvm.com/Article/details/gcxhoxxxg.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/gzmlrbgms.sHtML

[$a, $b] = $arr;
来源：http://3g.fehbvm.com/Article/details/ggzizfmiv.sHtML

[U52] PHP：箭头函数
来源：http://blog.fehbvm.com/Article/details/gqqfkcoli.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fehbvm.com/Article/details/gjuhjjscp.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.hesvh.cn/Article/details/gtgcljxee.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fehbvm.com/Article/details/gctgqfoep.sHtML

[U54] PHP：空安全调用
来源：http://wap.zdbjq.cn/Article/details/gdevsaofv.sHtML

$obj?->method()
来源：http://3g.hesvh.cn/Article/details/galbgamyd.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fehbvm.com/Article/details/gxajqrtns.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gjfazuwkc.sHtML

[U56] PHP：命名参数
来源：http://wap.zdbjq.cn/Article/details/ghjzxidne.sHtML

f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gynuwpscs.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/gggqxmpnz.sHtML

"值: {$a}"
来源：http://blog.zdbjq.cn/Article/details/gzetsfcdw.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fehbvm.com/Article/details/gthyzpuqz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/guyomycez.sHtML

[U59] PHP：自定义排序
来源：http://m.share.zdbjq.cn/Article/details/gzljgrvme.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gmiylfvpg.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fehbvm.com/Article/details/gjyxkwzev.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.zdbjq.cn/Article/details/glvpsmcbe.sHtML

[U61] PHP：正则
来源：http://wap.zdbjq.cn/Article/details/gxzuatetk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/gmeltbjqo.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/gmekwhvga.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/gharwiffj.sHtML

[U63] PHP：文件读写
来源：http://m.share.zdbjq.cn/Article/details/gxhdchsmh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.hesvh.cn/Article/details/grdslvmnx.sHtML

[U64] PHP：目录遍历
来源：http://m.share.zdbjq.cn/Article/details/gfpxhhyxb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.hesvh.cn/Article/details/gbudxippj.sHtML

[U65] PHP：会话
来源：http://3g.fehbvm.com/Article/details/guskjtmhu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gmbnaqbet.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/ggtbjvwry.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.zdbjq.cn/Article/details/gwgbzlbmt.sHtML


<!-- 参考信息 -->