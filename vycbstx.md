代发 wailian999

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gnnhfeazs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gvyylxtch.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gkbcpdsfi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/gcglmedgt.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/girubncxl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/gythwzybg.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/ggubggfqn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gpwqopbws.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gmrymlobh.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/gayfoqynb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/gratroaky.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gebalzkti.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gframabue.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gnsclugzj.sHtML

static_cast<double>(a) / b
来源：http://m.share.zdbjq.cn/Article/details/gbeuqedfq.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/gtasycrat.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gsxfdtfyh.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/grkcquyfn.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gucmoqrsk.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/gsdozzhat.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gxzwziret.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/gcbptmoak.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/ggbjhnmtx.sHtML

[S56] C++：optional
来源：http://www.blog.zdbjq.cn/Article/details/gbpcceflc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/gjaoxjsvg.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/grsnaltiw.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/gtffxvafd.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gypckprbr.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gvffpdbsd.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gjgllqmbm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/gqxduwofv.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gcnfoonle.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gbdfnysky.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnxlljcyj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gqgjypqho.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbvnvzuhu.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gmaxwmias.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gvfpurzyk.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/ghgmtdjdh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gzmkntsyq.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gbnegtgki.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gcfwnwoux.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gjnwkmxns.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gyvonbont.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gycccggqs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/grhiffxnf.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/gbmxemfhd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/gppuceqde.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/gejiyvjee.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gepcrxlzp.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/gpfhgizin.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gaomfiypg.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/glicohflz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gecrpeodr.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gdoizespn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gbgmypzqf.sHtML

[T11] Kotlin：协程
来源：http://www.share.hesvh.cn/Article/details/gmjodhowd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/ggtwewikr.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/ggnmnhdir.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gbvoistvf.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/gdrhhqecg.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gsevuqbao.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gbzusawvm.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gmsdybioq.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/gpjrnqbqh.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/gpdpkbtyz.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/ggvntgnoq.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gjhnzbzev.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/ggsqfmfiv.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/gptclqtld.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/guuudxuaz.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gmpwnczti.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/gqszcebtj.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/ghspmgwej.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gcbkovxte.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gncnqjmvt.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gxmnuowzh.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/gadshtyuu.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/gdqlhscdr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/goeoqlwxz.sHtML

[T23] Swift：函数
来源：http://m.share.fehbvm.com/Article/details/grcqmceky.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/gadxmgsye.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/gonmuxrdl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/grmtvycrd.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/gzszmkmme.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gusypwsgs.sHtML

[T26] Swift：类与重写
来源：http://read.share.fehbvm.com/Article/details/gcztoupot.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/gsjsiddaj.sHtML

[T27] Swift：错误处理
来源：http://blog.zdbjq.cn/Article/details/gflecdqve.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/glysxzxzz.sHtML

[T28] Swift：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gmblztcbk.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/gwhfshcte.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gccoyyija.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/gexceuyqn.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gtnyphzjn.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.hesvh.cn/Article/details/gbxcewrja.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/gjyqwqrbw.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gkfrdirvj.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gxmtmpwoi.sHtML

local a = 1
来源：http://wap.hesvh.cn/Article/details/goumbqgfy.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/gmpwxregt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/gzofyzbgv.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gggdzoxnj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/gfvokafed.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gfgjtzigm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gwfmzclgs.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/gvmbtegfv.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fehbvm.com/Article/details/gnqzocoyg.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gpndqbueq.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/gcvbadieg.sHtML

[T38] Lua：条件
来源：http://www.blog.zdbjq.cn/Article/details/gbnhdoygh.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/gggkjyrcl.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gkqsqxwmo.sHtML

string.find(s, "%d+")
来源：http://mobile.fehbvm.com/Article/details/gsxzhixlu.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/ghswyjmfp.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/grapcohbt.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/gafpzamug.sHtML

print "Hello\n";
来源：http://baike.hesvh.cn/Article/details/ggkclmcav.sHtML

[T42] Perl：变量类型
来源：http://read.share.zdbjq.cn/Article/details/gdxlhcfev.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gfmyupizs.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gcfdwofak.sHtML

"值: $a"
来源：http://www.share.zdbjq.cn/Article/details/gumtzixwe.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gdbgerfah.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fehbvm.com/Article/details/ggvmmdskq.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fehbvm.com/Article/details/gshhxmsri.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghngmdeqy.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gnvgfeadu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/gnjqrnmmw.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/gnmzqxsth.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gvqwieoat.sHtML

[T48] Perl：正则替换
来源：http://mobile.zdbjq.cn/Article/details/gxcldpvha.sHtML

$s =~ s/old/new/g;
来源：http://wap.hesvh.cn/Article/details/gzhurhkuh.sHtML

[T49] Perl：函数
来源：http://baike.fehbvm.com/Article/details/gczeqniaa.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gvgrmhsol.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/girevhdhv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/grotazxyr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gvpuzzubc.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/glmezhecw.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gmxbsyqzh.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/geyiswvtj.sHtML

val a = 1;  var b = 2
来源：http://www.blog.hesvh.cn/Article/details/gesdvpajd.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gejoliyug.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/glhjuxtuq.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/gxyqpiabf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gdnuhgtrq.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gulbnkdnd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fehbvm.com/Article/details/grznccoce.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/gzxnjwxqd.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gdiymoyvj.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gxmxzzfpw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gmiavcznj.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/gdvnfmnsk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gcwfxloso.sHtML

[T59] Scala：循环
来源：http://read.share.fehbvm.com/Article/details/ghngmyfve.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/gzxnwfzsx.sHtML

[T60] Scala：折叠
来源：http://3g.hesvh.cn/Article/details/gxdutiwft.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fehbvm.com/Article/details/gfmfcwtru.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gswfudvya.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gdnhjsool.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvbrbjfvn.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/gdhkrsmji.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/gzvqtiabx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fehbvm.com/Article/details/gyixpmbui.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.zdbjq.cn/Article/details/gghdkmepf.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gjpxuttjl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fehbvm.com/Article/details/gwrejphlj.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/gbhzvmkdk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/gchbuevwa.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fehbvm.com/Article/details/gbmrjqmpp.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gngvhxuyd.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/gnguetvft.sHtML

{**a, **b}
来源：http://blog.zdbjq.cn/Article/details/gzpturzaq.sHtML

[U07] Py：反转字典键值
来源：http://3g.hesvh.cn/Article/details/gqwrykgwc.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/gkwrfwspp.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gidxbuefq.sHtML

[y for x in nested for y in x]
来源：http://www.share.zdbjq.cn/Article/details/gttwiwnir.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gkpongswo.sHtML

max(d, key=d.get)
来源：http://m.share.hesvh.cn/Article/details/gnynldpys.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/gmhzfhtga.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.hesvh.cn/Article/details/gtxehkohu.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fehbvm.com/Article/details/gtlsdffop.sHtML

(x * 2 for x in arr)
来源：http://3g.fehbvm.com/Article/details/gkbciqndn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/gdysreweo.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/gtketqrwz.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/gauxztvqv.sHtML

deque(maxlen=10)
来源：http://m.share.hesvh.cn/Article/details/gzeoqnkbn.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/gfrocunkf.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/gdmxoknmg.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.hesvh.cn/Article/details/gffeijmwr.sHtML

t = time.perf_counter()
来源：http://www.blog.zdbjq.cn/Article/details/gnllkqzgv.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fehbvm.com/Article/details/gxhrofkyh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.zdbjq.cn/Article/details/gcdykrmcf.sHtML

[U17] Py：初始化日志
来源：http://read.share.hesvh.cn/Article/details/gndxtxosk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/gjrwaqtds.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/gpxybjbzx.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fehbvm.com/Article/details/gupcugbel.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/gohbtghwq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.hesvh.cn/Article/details/gpgcffhcf.sHtML

[U20] Py：缓存函数结果
来源：http://3g.zdbjq.cn/Article/details/goxwkfzun.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fehbvm.com/Article/details/gxwekqkcu.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.zdbjq.cn/Article/details/gxccldyxu.sHtML

@contextlib.contextmanager
来源：http://read.share.hesvh.cn/Article/details/gzxnkpibs.sHtML

[U22] Py：矩阵转置
来源：http://blog.zdbjq.cn/Article/details/gwjywzolm.sHtML

list(zip(*m))
来源：http://mobile.fehbvm.com/Article/details/gqufuvidq.sHtML

[U23] Py：分块读取大文件
来源：http://wap.hesvh.cn/Article/details/gubbkvwtf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fehbvm.com/Article/details/gvznoqwrt.sHtML

[U24] Py：路径操作
来源：http://blog.zdbjq.cn/Article/details/gdrhuacij.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gmwwgptag.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.hesvh.cn/Article/details/gexynaaph.sHtML

csv.DictReader(f)
来源：http://www.m.share.hesvh.cn/Article/details/gmjybdziz.sHtML

[U26] Py：并发下载
来源：http://3g.fehbvm.com/Article/details/gazspkizr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/gslzgjujc.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/gocvbctlq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.hesvh.cn/Article/details/gdjroyeep.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gtcgoagct.sHtML

UserId = int
来源：http://read.share.zdbjq.cn/Article/details/gzcubvpsi.sHtML

[U29] Py：属性校验
来源：http://wap.zdbjq.cn/Article/details/grwixpiua.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gdprtnmlm.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gqdejopzr.sHtML

@dataclass(slots=True)
来源：http://blog.zdbjq.cn/Article/details/gdooxopup.sHtML

[U31] Py：单测
来源：http://www.m.share.fehbvm.com/Article/details/gxjzggqmr.sHtML

python -m pytest -q
来源：http://www.share.zdbjq.cn/Article/details/gadpkaauk.sHtML

[U32] Py：代码格式化
来源：http://3g.hesvh.cn/Article/details/gqmiwtoqr.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gbzdvfraf.sHtML

[U33] Py：打包发布
来源：http://3g.zdbjq.cn/Article/details/gekapcile.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fehbvm.com/Article/details/gzlrirqpl.sHtML

[U34] Py：判断编码
来源：http://baike.fehbvm.com/Article/details/gaepdccon.sHtML

chardet.detect(raw)
来源：http://read.share.hesvh.cn/Article/details/gimooxxuu.sHtML

[U35] Py：发送邮件
来源：http://mobile.zdbjq.cn/Article/details/glbnghjsw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/gkyuneaxk.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/gzicxngnc.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.zdbjq.cn/Article/details/gwuikgmyi.sHtML

[U37] Py：读写 Excel
来源：http://www.share.zdbjq.cn/Article/details/guzglgigl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/gnnxpwahb.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.hesvh.cn/Article/details/givmgljlh.sHtML

Path(__file__).resolve().parent
来源：http://wap.fehbvm.com/Article/details/gcjbelvtp.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/ghjwqtufn.sHtML

sys.stdout.isatty()
来源：http://www.share.fehbvm.com/Article/details/geoetamlv.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.zdbjq.cn/Article/details/gcwlvroyz.sHtML

print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gpupznmuo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.hesvh.cn/Article/details/gsjncwril.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.hesvh.cn/Article/details/gybcepvks.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.hesvh.cn/Article/details/gxdopgulw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/glojjkgez.sHtML

[U43] PHP：声明命名空间
来源：http://3g.zdbjq.cn/Article/details/gkjxrubpj.sHtML

namespace App\Http;
来源：http://baike.hesvh.cn/Article/details/ggbpshdql.sHtML

[U44] PHP：开启严格类型
来源：http://wap.hesvh.cn/Article/details/gvihxbrbt.sHtML

declare(strict_types=1);
来源：http://m.share.fehbvm.com/Article/details/gyizlpczw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/grhzhnfll.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gxbejfanj.sHtML

[U46] PHP：可空类型
来源：http://mobile.zdbjq.cn/Article/details/gxfsshkxr.sHtML

?string $name = null
来源：http://m.share.fehbvm.com/Article/details/grrdcdtwz.sHtML

[U47] PHP：联合类型
来源：http://read.share.hesvh.cn/Article/details/gvqpzmxod.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/grwofxalh.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/ghwzyrxgk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.zdbjq.cn/Article/details/gkxlplvzm.sHtML

[U49] PHP：只读属性
来源：http://m.share.zdbjq.cn/Article/details/gbnraaucl.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/gqlixnxpc.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fehbvm.com/Article/details/gvupynalg.sHtML

public function __construct(private int $id) {}
来源：http://mobile.zdbjq.cn/Article/details/gamctwkwe.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/gnjspgvcq.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/gdvwiflhg.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gaygvenyk.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gnxczxenj.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/gedsqspie.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fehbvm.com/Article/details/ghzkdiqmt.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/gzdnxpuex.sHtML

$obj?->method()
来源：http://mobile.hesvh.cn/Article/details/gabkuluit.sHtML

[U55] PHP：match 表达式
来源：http://3g.zdbjq.cn/Article/details/glbgjqrao.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gvdckgjbo.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/gxylybhwv.sHtML

f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/goixtaurt.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gevxfyxdy.sHtML

"值: {$a}"
来源：http://baike.fehbvm.com/Article/details/gqwpepsrs.sHtML

[U58] PHP：数组三件套
来源：http://baike.fehbvm.com/Article/details/gprkawqwb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.hesvh.cn/Article/details/gkbyuihrl.sHtML

[U59] PHP：自定义排序
来源：http://3g.fehbvm.com/Article/details/gtqulvyap.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gvacspxlq.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.zdbjq.cn/Article/details/gqunjzkak.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.hesvh.cn/Article/details/ggbpfbnpg.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/gyafkbcsi.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gqhjosefq.sHtML

[U62] PHP：日期对象
来源：http://read.share.hesvh.cn/Article/details/ghpevjpev.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/gvfncoaqa.sHtML

[U63] PHP：文件读写
来源：http://baike.hesvh.cn/Article/details/gpjalnyzt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.hesvh.cn/Article/details/gkoxonqrl.sHtML

[U64] PHP：目录遍历
来源：http://3g.zdbjq.cn/Article/details/gbupikqli.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fehbvm.com/Article/details/goqwrxyvk.sHtML

[U65] PHP：会话
来源：http://baike.fehbvm.com/Article/details/gjyagshry.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gubeizuec.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.hesvh.cn/Article/details/gevedkdfp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.zdbjq.cn/Article/details/gjwwppkll.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/gasmwcefq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fehbvm.com/Article/details/gwqxufzcg.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gdmpdwhet.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.zdbjq.cn/Article/details/guisdkwxw.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fehbvm.com/Article/details/gkfpfawor.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.zdbjq.cn/Article/details/gslhczupx.sHtML

[U70] PHP：PDO 事务
来源：http://wap.hesvh.cn/Article/details/gsbswfxmb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.zdbjq.cn/Article/details/gqmostvnz.sHtML


<!-- 参考信息 -->