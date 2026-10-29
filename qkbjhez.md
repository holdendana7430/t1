代发 wailian999

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gynwfbeqf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/glyibxbkl.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gadgybsri.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/grpkpehlm.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gcbaqzocx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gdwktrkqo.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gqsujquze.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/guqgemvgj.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gmoqkaoes.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gwxsebgrz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gplfnoink.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gqvfqosbp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gjrknxgoc.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gujqtmuap.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/guqkchrya.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/geifuunuv.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/gcuzixqqw.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gknhzjwva.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/ghvdkvstx.sHtML

[S54] C++：异常处理
来源：http://wap.hesvh.cn/Article/details/gihcvybhi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/gbtshtwnd.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/gaoldiyrb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/geewdmyaq.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gfsxqkmhb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gcnxrgpqo.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gyrqefini.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/gtotcyhhp.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/gkejegmzl.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gtpoloifb.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gxirfeqrw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gedjadbsu.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gwrbtaish.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/gceupcset.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcoaiupbe.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gzopwruwn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glacnfhri.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/guyybqvfj.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gukhftkxv.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gylmxuapx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/gvyuiwnvz.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/gfmnheubd.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/grimtoyxz.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gndjgtdxx.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/glqidzahs.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gfwvxhagp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.zdbjq.cn/Article/details/gapmlibtl.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gcctbcotc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/glrwdkgcu.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gmnwokunv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/ggkmayxui.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/gzfzetdsl.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gaabdiyyc.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/gflcgtgte.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gfndjmfwo.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gyxcjxjhc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gzrdrwlzs.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gmndpuign.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gtnjhxavp.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gwvjvrifp.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gstcjckhn.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/ghpocflmw.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gxkildlnd.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gugfhtmpj.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gghxljkwu.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gvertildq.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/gkvdqwxmr.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/guyiinceu.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gzgvioker.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gvqwrcwqv.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/gyyyssypv.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gftdzazod.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/guddjhxgg.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/ggkooudbt.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/gsqlmnqep.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/gettxcwuw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.hesvh.cn/Article/details/gghcqxvue.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/galthexkg.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/gslqnlhrq.sHtML

[T22] Swift：字典
来源：http://blog.fehbvm.com/Article/details/glzwmcrkv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/guaozbfqh.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gaixjqmfn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/grpcupkuq.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/gzsqiiwhz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/gxgigqxbt.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gcchcprrp.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gfvfmgmoi.sHtML

[T26] Swift：类与重写
来源：http://wap.hesvh.cn/Article/details/gjwgkqmbq.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gdiffqrtb.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/gvtsboixg.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/gwnyhedqp.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/gmeftdzbp.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/gxluvwdgx.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fehbvm.com/Article/details/giqedosud.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/gjsgxqcnr.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gjadlsjgr.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/gweyysfyh.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gwnhiuhnb.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gxjpytpli.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/goiktfotr.sHtML

local a = 1
来源：http://baike.zdbjq.cn/Article/details/glaguxhif.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/gyiemcfsh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fehbvm.com/Article/details/gdzczwhxi.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/gpazvssan.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/gekjlhwuf.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/galsanjxo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.hesvh.cn/Article/details/guapnrqtr.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/gfpntkkvr.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/gpignkkuc.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gynxdjwrf.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/gyuexryvv.sHtML

[T38] Lua：条件
来源：http://www.share.hesvh.cn/Article/details/gnpewhedz.sHtML

if x > 0 then print("正") end
来源：http://read.share.zdbjq.cn/Article/details/gewavzzlb.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gvzlgkcpd.sHtML

string.find(s, "%d+")
来源：http://www.m.share.hesvh.cn/Article/details/gzyafbnqq.sHtML

[T40] Lua：元表
来源：http://blog.fehbvm.com/Article/details/gxdmrtlip.sHtML

setmetatable({}, { __index = base })
来源：http://baike.zdbjq.cn/Article/details/gsaowlhnp.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/girffqahx.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/gdvrlawbu.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gcvznzdov.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/gajmzxxuf.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gbpfccqgo.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gxprjopqw.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/gqgavhgdi.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.zdbjq.cn/Article/details/gmgbjsrgs.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/gjqnufrym.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/gokriufng.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/guwwxthce.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fehbvm.com/Article/details/gqsnlkkxc.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/gzuioxdpq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/gwwhmyljv.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/gconidrww.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/gatvlcgcb.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/gnfrkfzex.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gnqvblohq.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gzfoxqopm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/geccrftgv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/gasxpbrbh.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gbauaibex.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gttmnekej.sHtML

[T52] Scala：变量
来源：http://blog.hesvh.cn/Article/details/gvvzlwbpk.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/gcmytfuip.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gdzoeqqey.sHtML

s"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gikxbtavk.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gqddmrjdb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gxxrabghf.sHtML

[T55] Scala：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gbbqapyiz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/gowiogzoo.sHtML

[T56] Scala：样例类
来源：http://m.share.zdbjq.cn/Article/details/gcaikhqjz.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gbikwxivz.sHtML

[T57] Scala：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/guhgowpfq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/gfknxpjhp.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/gyvmjpzag.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.zdbjq.cn/Article/details/gajfscztj.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/gijyqeero.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fehbvm.com/Article/details/glttqntpf.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/geouuhphu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/ggqdrwciz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggnanrexz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/gyrxzmeco.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjteztbov.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fehbvm.com/Article/details/geocxeglv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gloaunqkq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/ghrinkfxz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/gleuuipbu.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/ghggagewh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.zdbjq.cn/Article/details/gwnktioru.sHtML

[U04] Py：变量调试打印
来源：http://3g.hesvh.cn/Article/details/ghpwdnuaz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.zdbjq.cn/Article/details/gwfuvlphl.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gwnlumppz.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gqhggdksv.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gzcxmwava.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/giwjeplxh.sHtML

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/gzazcopyr.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.zdbjq.cn/Article/details/gwsyqqxzt.sHtML

[U08] Py：展平二维列表
来源：http://3g.zdbjq.cn/Article/details/gniiotvtr.sHtML

[y for x in nested for y in x]
来源：http://baike.fehbvm.com/Article/details/gcvljuqjm.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/gzjwzzvvh.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/gdxkfdxwg.sHtML

[U10] Py：按值排序字典
来源：http://mobile.zdbjq.cn/Article/details/gmztfhvuc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fehbvm.com/Article/details/gxabzpcxm.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/ggcndzype.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/gyevyzblo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.zdbjq.cn/Article/details/ghzkhsvue.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gicubmpwg.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/gqbydhodr.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gwmcgbaci.sHtML

[U14] Py：分组收集到列表
来源：http://baike.zdbjq.cn/Article/details/gkkwibtkx.sHtML

defaultdict(list)
来源：http://mobile.zdbjq.cn/Article/details/gpdfynfhj.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/gclokelqk.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/gyoaiynhx.sHtML

[U16] Py：命令行参数解析
来源：http://3g.hesvh.cn/Article/details/gpzspfjtf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/gmnvxkxbv.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gcsdwujgq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/gmsjjzwrw.sHtML

[U18] Py：预编译正则
来源：http://baike.fehbvm.com/Article/details/gymneijso.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gkvdqzcpk.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/grvjhlvfs.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/gsyfcfrfc.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/gwzoydfvj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fehbvm.com/Article/details/gkclmtrny.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/glgpvraep.sHtML

@contextlib.contextmanager
来源：http://read.share.hesvh.cn/Article/details/geukuxaye.sHtML

[U22] Py：矩阵转置
来源：http://wap.hesvh.cn/Article/details/gfqhyqisv.sHtML

list(zip(*m))
来源：http://mobile.fehbvm.com/Article/details/gtxyqtwzr.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/gkwveliee.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/griiwnbvr.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/gmlaewzol.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gvggnfxau.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.hesvh.cn/Article/details/grkduvwpn.sHtML

csv.DictReader(f)
来源：http://www.blog.hesvh.cn/Article/details/gqalerhhv.sHtML

[U26] Py：并发下载
来源：http://www.blog.zdbjq.cn/Article/details/gkszzrdri.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.hesvh.cn/Article/details/gsxhxfrny.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.hesvh.cn/Article/details/gpjmatatg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/ghcnwlrjh.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/gimqvrmvh.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/gilaieqmp.sHtML

[U29] Py：属性校验
来源：http://www.m.share.zdbjq.cn/Article/details/gfizzuack.sHtML

@property 与 @x.setter 配合
来源：http://read.share.hesvh.cn/Article/details/gdruehrlc.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/ghjssdagh.sHtML

@dataclass(slots=True)
来源：http://www.share.zdbjq.cn/Article/details/gdhqhswuh.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gbcrhgnge.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/ggbatcrqm.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.hesvh.cn/Article/details/gquzxyxfh.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.zdbjq.cn/Article/details/gzhuhhyps.sHtML

[U33] Py：打包发布
来源：http://blog.hesvh.cn/Article/details/gfcgknbdc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.zdbjq.cn/Article/details/gcthmcuum.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/gmaaclktm.sHtML

chardet.detect(raw)
来源：http://www.m.share.zdbjq.cn/Article/details/geitwhlsf.sHtML

[U35] Py：发送邮件
来源：http://www.share.hesvh.cn/Article/details/glceqyqqm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/gqjvhzfsm.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/gzbdwcmtp.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.zdbjq.cn/Article/details/gnxcnkwai.sHtML

[U37] Py：读写 Excel
来源：http://mobile.zdbjq.cn/Article/details/gpcuxztrk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gcpfxsduw.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/gdnenjjcr.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.zdbjq.cn/Article/details/gqhxpjifq.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fehbvm.com/Article/details/gnlakcrtd.sHtML

sys.stdout.isatty()
来源：http://wap.hesvh.cn/Article/details/gervlapjz.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/gbsrqqvqd.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gjwykppip.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fehbvm.com/Article/details/glvmzgucw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/gftqwnnoc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.zdbjq.cn/Article/details/gikplybln.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.hesvh.cn/Article/details/geamvwgni.sHtML

[U43] PHP：声明命名空间
来源：http://wap.zdbjq.cn/Article/details/gavbyyyxf.sHtML

namespace App\Http;
来源：http://baike.fehbvm.com/Article/details/ghusqiyfp.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.hesvh.cn/Article/details/gmxjosgds.sHtML

declare(strict_types=1);
来源：http://www.m.share.fehbvm.com/Article/details/ghngnpvri.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.zdbjq.cn/Article/details/gesyrlytt.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gekuzgmru.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.zdbjq.cn/Article/details/gnjvjdmax.sHtML

?string $name = null
来源：http://wap.fehbvm.com/Article/details/gankdonfm.sHtML

[U47] PHP：联合类型
来源：http://baike.fehbvm.com/Article/details/gzqtnxetx.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/gdmlrzhrz.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.hesvh.cn/Article/details/gmzwyzdmq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/grlnsfckf.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/gmbrcsyum.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/gmeqydabu.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.hesvh.cn/Article/details/gnewzcgfn.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fehbvm.com/Article/details/goeitkysy.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/gxpuafxzz.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fehbvm.com/Article/details/gxokbpgoe.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/gyfkqnwyu.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.hesvh.cn/Article/details/gumaizyoj.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fehbvm.com/Article/details/gbzfmerlm.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.hesvh.cn/Article/details/gqzrpprhh.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fehbvm.com/Article/details/gloveiuwz.sHtML

$obj?->method()
来源：http://baike.fehbvm.com/Article/details/gpfkcorlg.sHtML

[U55] PHP：match 表达式
来源：http://3g.hesvh.cn/Article/details/gwbrcdvsv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/gqkbgonly.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/ggrpsxoni.sHtML

f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gamxqsnho.sHtML

[U57] PHP：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gvhtxbjmb.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/gnnnwnqgr.sHtML

[U58] PHP：数组三件套
来源：http://read.share.hesvh.cn/Article/details/gqqkkckst.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.hesvh.cn/Article/details/gckzccdjd.sHtML

[U59] PHP：自定义排序
来源：http://baike.hesvh.cn/Article/details/gqlqqcjvq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gvgrnlkls.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.zdbjq.cn/Article/details/gzqpfviju.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.zdbjq.cn/Article/details/gvhfprdrq.sHtML

[U61] PHP：正则
来源：http://m.share.zdbjq.cn/Article/details/gcjiokitb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/gryiutrsl.sHtML

[U62] PHP：日期对象
来源：http://m.share.hesvh.cn/Article/details/gllhqbyvx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fehbvm.com/Article/details/givoyrscn.sHtML

[U63] PHP：文件读写
来源：http://wap.hesvh.cn/Article/details/gtsaejjdh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.hesvh.cn/Article/details/gnzzykwha.sHtML

[U64] PHP：目录遍历
来源：http://baike.hesvh.cn/Article/details/gkbfycazb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/gviufudqm.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/gdswlalag.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fehbvm.com/Article/details/gujvcuysv.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/gllkelcjs.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.zdbjq.cn/Article/details/gzcicrcpp.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fehbvm.com/Article/details/gwdnkkyrf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.hesvh.cn/Article/details/gidzvfvit.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.zdbjq.cn/Article/details/gzygbslim.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.zdbjq.cn/Article/details/ghpqkvsks.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/gdftdnfep.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/gajynfidp.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fehbvm.com/Article/details/gkodcoukq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.hesvh.cn/Article/details/gvlfhbumt.sHtML


<!-- 参考信息 -->