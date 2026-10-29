代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gxbbmaxiz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/gsnpevgbq.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gknagsjcx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gclzxmhmn.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/gljxnifjr.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gwktriybj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gutzplnqb.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gzhhppnzm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gevrrpiad.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gkanxowgt.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/ggkssaofl.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/gzqyaetva.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/goiaqbvol.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/gqdudvmit.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gyyllrrdj.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/gedotbead.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gwmmnqisq.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gscaginaz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/gkzqppxzl.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gsapljyxb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/gcvtojbvm.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gfpbdmfgb.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gybfivovl.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/gklrcedgf.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fehbvm.com/Article/details/gqofpttsi.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gyfarlpmb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gkautchdu.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/ghydbilpw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gzjpsjwoc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjblpfmmp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gidpxlqvh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grrmhoxjz.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gwwrvpsdn.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/giusmlhma.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gpncnvgod.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gwuutowmd.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/gkgmwtijj.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gwntjqcxb.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/guraipcmn.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/guxwsgxmg.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gaudsqgwy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gaabyiwmw.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gdutcolwq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gacttntuf.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gxogtzdst.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/goelvepdh.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gntnytjve.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gpthkqrqt.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gcjtibuha.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/goebvyotv.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/gxgxnlxqc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/gasafrwcm.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gqlmorfbo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gggwzqhxh.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/gjxuqepct.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gzqfuyxgw.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gesghdpsk.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/gfaelweie.sHtML

[T14] Kotlin：循环
来源：http://blog.zdbjq.cn/Article/details/gdxlvckhv.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/grzgdzdxe.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/gcwlsuelf.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gmhjcajvl.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/gtdojvsbu.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/ghnrtdeeh.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gqadbkesx.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/ghdggiwsq.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gfuhjizwt.sHtML

"值: \(b)"
来源：http://mobile.fehbvm.com/Article/details/gpwxcbmtl.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gcasdmsxo.sHtML

if let n = opt { print(n) }
来源：http://www.share.hesvh.cn/Article/details/gxmidzdln.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gcegnprpd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/gzksepnmw.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gwfxotidd.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/giucfqgxc.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/gleeejqar.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gmzzdsddu.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/girxftwni.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.hesvh.cn/Article/details/gadegcwsy.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gvxecyoam.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gmxaljjxo.sHtML

[T25] Swift：结构体
来源：http://blog.zdbjq.cn/Article/details/ghsclrwuu.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gbnqbvqrh.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gsqqszqgg.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/gseotmrjr.sHtML

[T27] Swift：错误处理
来源：http://mobile.zdbjq.cn/Article/details/gbixqxihm.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/gwqhynajo.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/gvcuteuud.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/giyxmybqq.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/gdybixdfg.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/glruerjhh.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/gqyhrkysl.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.zdbjq.cn/Article/details/grallregb.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/gtxghmyya.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gpidmdniu.sHtML

[T32] Lua：局部变量
来源：http://blog.fehbvm.com/Article/details/gpymqfkhf.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gpoaufepm.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fehbvm.com/Article/details/gzwzamznr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/gmbhjlmio.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/guuubdsak.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/gdwlfytde.sHtML

[T35] Lua：字典表
来源：http://blog.fehbvm.com/Article/details/gpauncyzo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/ghhfbscrh.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gacxmyijp.sHtML

function add(a, b) return a + b end
来源：http://wap.hesvh.cn/Article/details/gjunuspdr.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gudxeaxur.sHtML

"a" .. "b"
来源：http://www.m.share.zdbjq.cn/Article/details/gfhjufuoy.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/gazkglovq.sHtML

if x > 0 then print("正") end
来源：http://m.share.fehbvm.com/Article/details/gcoqchpie.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gruktzncq.sHtML

string.find(s, "%d+")
来源：http://3g.hesvh.cn/Article/details/gpraxhmvx.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/gnwflwuaw.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.hesvh.cn/Article/details/gdlbuyxci.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gliqzidkj.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gnnfheurv.sHtML

[T42] Perl：变量类型
来源：http://baike.fehbvm.com/Article/details/gjkslzcqg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.zdbjq.cn/Article/details/gbqwcfzne.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/grdjldfcg.sHtML

"值: $a"
来源：http://wap.hesvh.cn/Article/details/gdfymrzkt.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gshaijtdl.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/gpzjcfgyn.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/gyvkbrmnd.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/gqdgvaqbf.sHtML

[T46] Perl：哈希操作
来源：http://read.share.zdbjq.cn/Article/details/gpuprnepl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.hesvh.cn/Article/details/gwlxcraqu.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/gwbjcbssg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/gyjxdarkl.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/ghklraqqr.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/gawszjseo.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gshdvpawg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/ginfrbimb.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gbbyowoso.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fehbvm.com/Article/details/gmfeewdtd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/gacwxvhdo.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/giciszake.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/ghbnctqgk.sHtML

[T52] Scala：变量
来源：http://m.share.zdbjq.cn/Article/details/ghysuucxo.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/gltaemwkg.sHtML

[T53] Scala：字符串插值
来源：http://3g.hesvh.cn/Article/details/gcldwwcsp.sHtML

s"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gxddypugr.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gtgxkgwbo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/gypiyyzbu.sHtML

[T55] Scala：集合过滤
来源：http://3g.fehbvm.com/Article/details/gdvtddgmw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/gpkvmsabo.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/ghtrlqtat.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/gnpmvfssy.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/ggrmdnals.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gfnmvymbo.sHtML

[T58] Scala：函数定义
来源：http://mobile.fehbvm.com/Article/details/gbxzsxlrm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/gzjdozovq.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gnjnxrwwe.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gbljdksrh.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/gunlbngiq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fehbvm.com/Article/details/gkaglhurb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqvqvgyhx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/gftmgklzx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwrprvabt.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gdjxlhsni.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/ghwuzktuj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/gtubskngs.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gjzeffbzt.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/gwoapiuvw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/gphlnkqao.sHtML

[U04] Py：变量调试打印
来源：http://baike.fehbvm.com/Article/details/gzngplpcj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/gpnzceofe.sHtML

[U05] Py：列表去重且保序
来源：http://blog.hesvh.cn/Article/details/gjadkrwtd.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/girxabjjs.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.hesvh.cn/Article/details/gkjjdgdag.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/gxpteuswb.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fehbvm.com/Article/details/golobxtla.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/gymelvxag.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fehbvm.com/Article/details/gywoajste.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/gtvnckgeg.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/giblzcqid.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/gqoeaieif.sHtML

[U10] Py：按值排序字典
来源：http://baike.hesvh.cn/Article/details/gkfvavhoa.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/gcqzcfvxn.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.hesvh.cn/Article/details/gwzmhczsa.sHtML

(x * 2 for x in arr)
来源：http://m.share.zdbjq.cn/Article/details/ggtoltzwp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.zdbjq.cn/Article/details/gkrlzimoa.sHtML

Counter(arr).most_common(3)
来源：http://mobile.zdbjq.cn/Article/details/gafuiipac.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/ggosgukuv.sHtML

deque(maxlen=10)
来源：http://wap.fehbvm.com/Article/details/gygnnskbl.sHtML

[U14] Py：分组收集到列表
来源：http://blog.zdbjq.cn/Article/details/gijaflsnw.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gudurxekh.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/gyfbumrbo.sHtML

t = time.perf_counter()
来源：http://www.blog.fehbvm.com/Article/details/gowagmeul.sHtML

[U16] Py：命令行参数解析
来源：http://3g.zdbjq.cn/Article/details/gcplllwts.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gxlxpbyet.sHtML

[U17] Py：初始化日志
来源：http://3g.hesvh.cn/Article/details/gauzhytvw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/gusxypbew.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/gerdqkrmx.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/glulhjflc.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.zdbjq.cn/Article/details/gmelcfwpt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.hesvh.cn/Article/details/gymjxjsyq.sHtML

[U20] Py：缓存函数结果
来源：http://wap.hesvh.cn/Article/details/gkftpjazt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.hesvh.cn/Article/details/gxapkwvxn.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/gqfgttvme.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/gdrfptupt.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fehbvm.com/Article/details/gfefqpzlj.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/gvwhtbsey.sHtML

[U23] Py：分块读取大文件
来源：http://3g.hesvh.cn/Article/details/ggxpohsdi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.zdbjq.cn/Article/details/gabjjnbqz.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/gfmpzmpzg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gtuifwbua.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.zdbjq.cn/Article/details/gddpdwqal.sHtML

csv.DictReader(f)
来源：http://wap.hesvh.cn/Article/details/gngclrnnh.sHtML

[U26] Py：并发下载
来源：http://mobile.fehbvm.com/Article/details/ggviyghcx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fehbvm.com/Article/details/giycxnqml.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/gxetpeipm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/gqlhkslsl.sHtML

[U28] Py：类型别名
来源：http://www.blog.zdbjq.cn/Article/details/gjynwoibv.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/gzbrxffnc.sHtML

[U29] Py：属性校验
来源：http://3g.fehbvm.com/Article/details/glfmrccor.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.zdbjq.cn/Article/details/glycyvjcb.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/gthmqapec.sHtML

@dataclass(slots=True)
来源：http://read.share.hesvh.cn/Article/details/gzabsunrp.sHtML

[U31] Py：单测
来源：http://wap.hesvh.cn/Article/details/gxxtzabux.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/gnziabupb.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gznaeumkk.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gyrwthtqe.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/gerxlvhjc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.hesvh.cn/Article/details/glwldbwbg.sHtML

[U34] Py：判断编码
来源：http://baike.zdbjq.cn/Article/details/gsiaplnzc.sHtML

chardet.detect(raw)
来源：http://www.m.share.hesvh.cn/Article/details/gjyzauvul.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/gffvybfhk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fehbvm.com/Article/details/gdeozyeov.sHtML

[U36] Py：定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gmrzkxdvs.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/glawubmgu.sHtML

[U37] Py：读写 Excel
来源：http://baike.fehbvm.com/Article/details/grfaiuisa.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.hesvh.cn/Article/details/gwbcqchuk.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gjnhjfsot.sHtML

Path(__file__).resolve().parent
来源：http://blog.hesvh.cn/Article/details/ggsjnfypl.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fehbvm.com/Article/details/gvsolmlgq.sHtML

sys.stdout.isatty()
来源：http://m.share.hesvh.cn/Article/details/gvvkmvbqz.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.zdbjq.cn/Article/details/gttgjlhis.sHtML

print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gspwhvpzq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fehbvm.com/Article/details/gofhajmrc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/gtjajxvnh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.hesvh.cn/Article/details/gphmismer.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/ghnpjmlhg.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/gewcgalov.sHtML

namespace App\Http;
来源：http://3g.zdbjq.cn/Article/details/gjoppqwld.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.hesvh.cn/Article/details/gjzmnhryf.sHtML

declare(strict_types=1);
来源：http://www.m.share.zdbjq.cn/Article/details/gyjabmhgb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/gwaprdpmy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gwnzifsbh.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fehbvm.com/Article/details/gonrzshgq.sHtML

?string $name = null
来源：http://www.blog.fehbvm.com/Article/details/gdwrjwyfs.sHtML

[U47] PHP：联合类型
来源：http://read.share.hesvh.cn/Article/details/gmeyaxlap.sHtML

int|string $id
来源：http://www.blog.zdbjq.cn/Article/details/gpopstixk.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fehbvm.com/Article/details/gywxkcyfm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.hesvh.cn/Article/details/ghlfpjivf.sHtML

[U49] PHP：只读属性
来源：http://baike.hesvh.cn/Article/details/gejlneaqm.sHtML

public readonly string $name
来源：http://wap.zdbjq.cn/Article/details/gzuquroqw.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.zdbjq.cn/Article/details/ghetjfgxj.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fehbvm.com/Article/details/gfrchwbuh.sHtML

[U51] PHP：数组解构
来源：http://m.share.hesvh.cn/Article/details/gvpkidcos.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fehbvm.com/Article/details/gdobtfoew.sHtML

[U52] PHP：箭头函数
来源：http://3g.hesvh.cn/Article/details/gchaqoieb.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fehbvm.com/Article/details/gzawpygyg.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fehbvm.com/Article/details/ggxhercol.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.zdbjq.cn/Article/details/gyrfzzldz.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.hesvh.cn/Article/details/gvzcuswvh.sHtML

$obj?->method()
来源：http://www.share.hesvh.cn/Article/details/guevrhdot.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gedxjcvqx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/goeflyngi.sHtML

[U56] PHP：命名参数
来源：http://www.blog.hesvh.cn/Article/details/ghzqbmqwo.sHtML

f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/glxmqlhep.sHtML

[U57] PHP：字符串插值
来源：http://wap.hesvh.cn/Article/details/gvielpnyy.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/grblomuey.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/glftivzfo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fehbvm.com/Article/details/gaxfgpbqj.sHtML

[U59] PHP：自定义排序
来源：http://read.share.zdbjq.cn/Article/details/glsahqaop.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/geetltsjd.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fehbvm.com/Article/details/gwepsqooo.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.hesvh.cn/Article/details/gnryvfwni.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/gfidmjull.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gggpboarj.sHtML

[U62] PHP：日期对象
来源：http://wap.fehbvm.com/Article/details/ganmnwhem.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.hesvh.cn/Article/details/garoiyafw.sHtML

[U63] PHP：文件读写
来源：http://read.share.hesvh.cn/Article/details/gittvkkkv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/gjyahjdhs.sHtML

[U64] PHP：目录遍历
来源：http://blog.fehbvm.com/Article/details/gmczrzkqj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fehbvm.com/Article/details/gkehrjveu.sHtML

[U65] PHP：会话
来源：http://baike.zdbjq.cn/Article/details/gocweapjs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fehbvm.com/Article/details/glqquvlvn.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.hesvh.cn/Article/details/geeuegoyw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fehbvm.com/Article/details/ghzsifnxu.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.zdbjq.cn/Article/details/grdlbfdfh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.zdbjq.cn/Article/details/gkqnhtwoc.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/gopdqxeew.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.hesvh.cn/Article/details/gegcplclm.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fehbvm.com/Article/details/gtcgqgywo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/gyncujgun.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.hesvh.cn/Article/details/gpfmnbafo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.hesvh.cn/Article/details/grrpwcsti.sHtML

[U71] PHP：抛出异常
来源：http://read.share.zdbjq.cn/Article/details/ghwlbfhin.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fehbvm.com/Article/details/gkoyabven.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.zdbjq.cn/Article/details/gldhfhwml.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/gguetenip.sHtML


<!-- 参考信息 -->