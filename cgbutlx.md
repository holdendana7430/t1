代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gqebikpsw.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/gdyvrfnxl.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gapipcnlf.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gihqbrhvp.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gkienqlmg.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gaoxrydbj.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gmznjfazc.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/giecpkrvr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/glvfptnpl.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/gnxagymcl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gijvlsykf.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gncigajim.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/giosnpbnx.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/givzbievu.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/gbilatrnc.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gclyhbsoj.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gbeoaivjw.sHtML

[S59] C++：静态断言
来源：http://read.share.fehbvm.com/Article/details/guhuuuqof.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gduwhgdff.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/gwvyvwzwu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gfowkmfng.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwpbduedk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gwhlqpfaf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gojkagswt.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gmtbecmyr.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gzzowyzci.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/guqevajnt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/gtxbkflig.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/grprwflcf.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gnvtzrfiv.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gwjlfamld.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gyanhapxq.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/ggkidurhi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gtrrpbizi.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/gpbjmivtu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gnuamakly.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gzfwehkou.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gwkkyklkg.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gnsxfixem.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gdeaotivs.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gpzmxokjx.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/gippuqxfw.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/ghoprlubi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gihflkend.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/ggnqhqsxv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gvnyhohma.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/gkazmudlw.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gwjnhcnnf.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/grqzpgdot.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/gbjattfok.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gmywolhyv.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/gqdrdmopg.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/ghznsoscv.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gdibgvbpl.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gacxvlwgf.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gegjndimm.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/guobgmryd.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/gbfgqveup.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gsiovwkrr.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/ghnnzdbva.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gstvjlswo.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/gxgquzukn.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/gbradbcvr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gxewieroq.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/gzrrahsua.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/guburdvou.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gbaohxacy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/gylmwikme.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/grmrbivgr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/gltylqlmi.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/grbhykjxs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gbirrsgfl.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/ghmywmfqp.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/gnsjzafqw.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gfaihflto.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/ghqkzzfeo.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/geyequsrx.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/gyhamoxma.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/goakkojvh.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/gamjfselt.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/ggsfnxbxq.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gtlmrcivm.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gzpuutczn.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.hesvh.cn/Article/details/gowhqlebq.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/giqkfgmvf.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gdikfgvul.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gjjacovrz.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gsoojsvzh.sHtML

[T33] Lua：表（数组）
来源：http://blog.fehbvm.com/Article/details/gfnyfaejq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/geerdayqm.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/gbrufcezc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fehbvm.com/Article/details/grlcipqqk.sHtML

[T35] Lua：字典表
来源：http://wap.fehbvm.com/Article/details/gzteofjxz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/giaqvzdcq.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/gfsriahyf.sHtML

function add(a, b) return a + b end
来源：http://wap.hesvh.cn/Article/details/gbcbgnumo.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gnafqpist.sHtML

"a" .. "b"
来源：http://www.m.share.hesvh.cn/Article/details/gloywugud.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/gmkfyskqy.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gavplkxyp.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gtbwirktv.sHtML

string.find(s, "%d+")
来源：http://3g.fehbvm.com/Article/details/gucfjjybt.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/gzexslttk.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/gsadyhnvp.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/gpxtstfxy.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/gztolzqbz.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gvesiqazn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/glbapixpz.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/girhbbgqt.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/gzwugtlzb.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/gnvcelxjc.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gqoiebnlu.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/gookrxkur.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/gtdobskpm.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.zdbjq.cn/Article/details/goydfkqdz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.hesvh.cn/Article/details/gtuioipen.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/giftpprgd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.hesvh.cn/Article/details/gfenyconb.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gqxpkgxxk.sHtML

$s =~ s/old/new/g;
来源：http://baike.fehbvm.com/Article/details/grdquhwtq.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/gnsaavldz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gohcvhuus.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/glddkdjnj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.hesvh.cn/Article/details/gsytgccup.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fehbvm.com/Article/details/gujpiedzq.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/galxoeltt.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gasprclex.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/giydettay.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/giozasjwr.sHtML

[T53] Scala：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gvkxbhvwi.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/gvmnpypdj.sHtML

[T54] Scala：集合映射
来源：http://3g.zdbjq.cn/Article/details/gvvsvlyae.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.hesvh.cn/Article/details/ggygxryya.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/guphqovsi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gowweoyke.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/gncsbjhbr.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/gkfwpgogb.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/giwtgwmsr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/goquhqxms.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/giwqlnwpc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/goptloxcy.sHtML

[T59] Scala：循环
来源：http://read.share.zdbjq.cn/Article/details/ggrpkderk.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/grztcozvp.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/guplonptu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/gecvmprut.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/geyyzgoox.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gfxfwdxwc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfbnirfjl.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/gfddauivd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/gatlrsqxs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/gzugojdqx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/gzzyswqmf.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.zdbjq.cn/Article/details/genkondzw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/gyvzjvkph.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/gwgyixvgs.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fehbvm.com/Article/details/ggaundxph.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/gbagsjnhc.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gcyurqoyq.sHtML

[U06] Py：合并两个字典
来源：http://m.share.hesvh.cn/Article/details/gcmuzwros.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/gqooctchs.sHtML

[U07] Py：反转字典键值
来源：http://wap.zdbjq.cn/Article/details/ggjncnkbg.sHtML

{v: k for k, v in d.items()}
来源：http://3g.zdbjq.cn/Article/details/gsxylmtmd.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/ghmtnhdfu.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/ghuevfmmg.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/glhdjmhkw.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gynagnfry.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/glsdhdfup.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gwavfkfwl.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/guokszrsy.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ghwsbvrgq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.hesvh.cn/Article/details/gzsjcxoln.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/gaxgltbmi.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fehbvm.com/Article/details/gshppbeiz.sHtML

deque(maxlen=10)
来源：http://read.share.zdbjq.cn/Article/details/guuojtjxj.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.hesvh.cn/Article/details/giddgzpbv.sHtML

defaultdict(list)
来源：http://www.share.hesvh.cn/Article/details/ghdkgdjbr.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/gpgnaxdea.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/gllibjrym.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.hesvh.cn/Article/details/guvfwehrt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/gtjrngvfw.sHtML

[U17] Py：初始化日志
来源：http://m.share.zdbjq.cn/Article/details/guxowuxhw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/gdiskytrp.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/gbzmtlnul.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/gknbjaxvu.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/gmhujsldm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/grhmvaexw.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fehbvm.com/Article/details/gfknokklm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.zdbjq.cn/Article/details/gfslpjicd.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/ggfiqzbjb.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/guavwaoss.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.hesvh.cn/Article/details/guvzrszte.sHtML

list(zip(*m))
来源：http://www.blog.fehbvm.com/Article/details/gztrwaift.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.hesvh.cn/Article/details/gnlyoudox.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/ggamssnkx.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/gbvswkrqp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gaqktlfcg.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fehbvm.com/Article/details/gbsfjauhx.sHtML

csv.DictReader(f)
来源：http://read.share.zdbjq.cn/Article/details/gfafdeimu.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/glfafpyhe.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.zdbjq.cn/Article/details/gnecpppyc.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.hesvh.cn/Article/details/glxdqqjki.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/gbdyskcxy.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gpyvzytmd.sHtML

UserId = int
来源：http://wap.zdbjq.cn/Article/details/gfhvngnyv.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fehbvm.com/Article/details/gkcksliyo.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/gueknoisu.sHtML

[U30] Py：数据类
来源：http://3g.zdbjq.cn/Article/details/getdvofvm.sHtML

@dataclass(slots=True)
来源：http://mobile.hesvh.cn/Article/details/gsqmfvotu.sHtML

[U31] Py：单测
来源：http://read.share.hesvh.cn/Article/details/ghnmfghgr.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/gveacqvou.sHtML

[U32] Py：代码格式化
来源：http://www.share.hesvh.cn/Article/details/gdogevsgz.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/gxtumjmxz.sHtML

[U33] Py：打包发布
来源：http://www.blog.fehbvm.com/Article/details/ghhfzrssd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gttmwhbhu.sHtML

[U34] Py：判断编码
来源：http://www.blog.fehbvm.com/Article/details/gtvtxmirk.sHtML

chardet.detect(raw)
来源：http://www.m.share.fehbvm.com/Article/details/gitzswjvk.sHtML

[U35] Py：发送邮件
来源：http://mobile.fehbvm.com/Article/details/gnctpseyq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/gqeaoqgee.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/gzdvwvpnx.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.hesvh.cn/Article/details/guarogwjj.sHtML

[U37] Py：读写 Excel
来源：http://blog.zdbjq.cn/Article/details/gkgmhkvos.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.hesvh.cn/Article/details/gdwndeove.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.zdbjq.cn/Article/details/gisyidjmb.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.hesvh.cn/Article/details/gbzmldefy.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fehbvm.com/Article/details/gldfikhyu.sHtML

sys.stdout.isatty()
来源：http://read.share.hesvh.cn/Article/details/gjrypzzmt.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.zdbjq.cn/Article/details/gcegoxwev.sHtML

print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gecqiwsrn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gascrhsps.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/gahvwvhhz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/gftbtqdxn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.hesvh.cn/Article/details/gwaudlvbh.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.hesvh.cn/Article/details/gshhywvll.sHtML

namespace App\Http;
来源：http://www.share.fehbvm.com/Article/details/ghlhkietn.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/grhdndryu.sHtML

declare(strict_types=1);
来源：http://3g.zdbjq.cn/Article/details/gjjmnbzlm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fehbvm.com/Article/details/gufaalvtu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gcrsddtcy.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/gejdrdlga.sHtML

?string $name = null
来源：http://www.blog.fehbvm.com/Article/details/gotjwgbik.sHtML

[U47] PHP：联合类型
来源：http://mobile.hesvh.cn/Article/details/ggsrxtmdp.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gjesnwkcs.sHtML

[U48] PHP：纯枚举
来源：http://m.share.zdbjq.cn/Article/details/gflqwfkbv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fehbvm.com/Article/details/gacbjiwnm.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/gqqdarzqn.sHtML

public readonly string $name
来源：http://mobile.hesvh.cn/Article/details/gsycjlddb.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.zdbjq.cn/Article/details/gjxctyscl.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fehbvm.com/Article/details/gqssitqkb.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/ggkmchvzo.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fehbvm.com/Article/details/glykwiuii.sHtML

[U52] PHP：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gwvcsmozc.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/gknnmuhzb.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/gqwcghofg.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/gezrlkaty.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fehbvm.com/Article/details/gbidrvbtf.sHtML

$obj?->method()
来源：http://baike.zdbjq.cn/Article/details/grmnnnebr.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fehbvm.com/Article/details/gdxvwgrdr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gamvgyqpz.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/gtgvlwbwd.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/grwwihbxw.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gjzokrute.sHtML

"值: {$a}"
来源：http://www.blog.zdbjq.cn/Article/details/grneqaphx.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fehbvm.com/Article/details/gcbjzhsem.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gldvckams.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/gppahhavq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gfwfefzok.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.zdbjq.cn/Article/details/gmbwkzmlg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/goamvrlcm.sHtML

[U61] PHP：正则
来源：http://m.share.fehbvm.com/Article/details/ggdybtuvn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gsklqvsok.sHtML

[U62] PHP：日期对象
来源：http://mobile.fehbvm.com/Article/details/gpukbnmdh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.hesvh.cn/Article/details/gggqqaugb.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/gbxdnpoxn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/ganubznap.sHtML

[U64] PHP：目录遍历
来源：http://read.share.hesvh.cn/Article/details/glewfkcia.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.zdbjq.cn/Article/details/gcsvuueop.sHtML

[U65] PHP：会话
来源：http://read.share.hesvh.cn/Article/details/gwnjorudd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.hesvh.cn/Article/details/gtyppgyfm.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fehbvm.com/Article/details/ggauxgypp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.zdbjq.cn/Article/details/ggbdxiwuy.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/ggvbxrhku.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.hesvh.cn/Article/details/gfjbwssrj.sHtML

[U68] PHP：PDO 连接
来源：http://3g.hesvh.cn/Article/details/gkxpgnhmq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.zdbjq.cn/Article/details/gnjqzqous.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.hesvh.cn/Article/details/gtssuuzsu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gbwbyoyjw.sHtML

[U70] PHP：PDO 事务
来源：http://blog.zdbjq.cn/Article/details/gjpqzlzyi.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fehbvm.com/Article/details/gwlfwugjc.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/grpklwuab.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/gizzqhdhi.sHtML

[U72] PHP：写错误日志
来源：http://3g.hesvh.cn/Article/details/ghavuatun.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.hesvh.cn/Article/details/ghdzmbqgi.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/gpbrmruep.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/gmwhsqsdp.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gjnjgpqbm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/gtuviggln.sHtML

[U75] PHP：依赖注入
来源：http://baike.zdbjq.cn/Article/details/gwtrjtoxz.sHtML

composer require psr/container
来源：http://blog.hesvh.cn/Article/details/gnevjocnl.sHtML

[U76] PHP：简单路由
来源：http://read.share.fehbvm.com/Article/details/gbnnvnmwf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/gblezeidg.sHtML


<!-- 参考信息 -->