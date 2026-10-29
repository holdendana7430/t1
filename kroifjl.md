代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gwxfdjjjr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gptzgcrra.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gtpjtdqbc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gxxiqavwf.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/giihaxzgv.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/gvyqyyjdd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/gafxhhudh.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gdfnizotf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gzqydtzxw.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/gwafmgydl.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gdbbupbck.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/grcnxznjp.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gtlnufpev.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/ghwytfcyt.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gybwfkwxl.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gxarzqatu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gpwzrwxje.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gsqitinrn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gjtvajzii.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gzioqnddw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/gzfifwwnu.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/ggaanlcov.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gtogauocm.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/gejtfoido.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.hesvh.cn/Article/details/gstgvyxhe.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/gvfaxmwcq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/gigovnmuk.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gjnzrxyjr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gqgsxhrco.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grwigsxeb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gshgsstmg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grqgwkglt.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gwmmbwvqr.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/ginarfxdi.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gmlaqwekh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gtjxgqlrm.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/gsvzkezxs.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gecngzkrf.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gcispsjeb.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gaofqozhi.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gsbpswaba.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/gxdqzsdym.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/giphyszfc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/giwlytfwk.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gbuvowecs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/grszmfljq.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/giyxsyaky.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/ghtvpslpk.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gczskasyb.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/gvshrqtrc.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/gpuplpria.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gnwkwqabn.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/gntmbofsm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gjwjcluye.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/gkygkewla.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gzkptksxt.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/glhponesf.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gkmyewxfc.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gucepwnab.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/gnskkjbaz.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gymyaktio.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gbiwrvmti.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/genvrcwwy.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/ggktmudec.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/gbzcgczyn.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/grrjjsqnp.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/gimpwuyxu.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gwqpsfnli.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/govelmdzv.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/gxjdndzwl.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/gjlobzxfc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/gojlkzbnv.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/gpidsneei.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/gsjfwedmm.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/gljwegbtd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gamgrjxdx.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/ghliokqky.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.hesvh.cn/Article/details/gxyfyzafe.sHtML

[T24] Swift：闭包
来源：http://www.blog.fehbvm.com/Article/details/gtjnobajz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/goufvcxap.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/glgpmedah.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gcktctjcd.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/gicemezav.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/gkbiersxq.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/ggfaukvdm.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/gykmddtap.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gilaxfmbq.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/guwqmzdwa.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gnthgbdtk.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/gvedxfvdu.sHtML

[T30] Swift：协议
来源：http://www.share.zdbjq.cn/Article/details/gjoptqemf.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/groglhvyq.sHtML

[T31] Lua：Hello World
来源：http://m.share.fehbvm.com/Article/details/gmdrwdgxy.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/grnyfretj.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gauvzbojx.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gopqhjuds.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/gqlosgmzm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/gfiavcdxx.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gdwuxxpcw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/gckvckfev.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/giefpjxvu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gukrvczxp.sHtML

[T36] Lua：函数
来源：http://baike.hesvh.cn/Article/details/gprmuerdw.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/gpxnyaqch.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gkdhyqdrm.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/gkmlpskai.sHtML

[T38] Lua：条件
来源：http://read.share.fehbvm.com/Article/details/gbnatdnjm.sHtML

if x > 0 then print("正") end
来源：http://m.share.hesvh.cn/Article/details/gmvazaobn.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/gehljkprs.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gwtbsfwvc.sHtML

[T40] Lua：元表
来源：http://wap.zdbjq.cn/Article/details/gendpnzql.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/gqmwzwsqs.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gfflmxgez.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gwlavlikn.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gqmdwnxnm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.zdbjq.cn/Article/details/gjkleayll.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/gbvbgqfcl.sHtML

"值: $a"
来源：http://blog.hesvh.cn/Article/details/glcgqbxtn.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/gztbfvrfo.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/gomxfeihr.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/gxhvpyehr.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gsdslitty.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gkxulyfaj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gqfgvwfla.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/griramkrr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/gystgzqzk.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/gjzlexaqy.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/gjypgufyg.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/gokenrjhu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gouyubiar.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gawqqzhqz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/gpqkmbxyq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/ghtufvaey.sHtML

[T51] Scala：Hello World
来源：http://baike.zdbjq.cn/Article/details/ggxsiumww.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/ghxzcafqa.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/giuexwdie.sHtML

val a = 1;  var b = 2
来源：http://wap.fehbvm.com/Article/details/gahgujnvs.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/glitgpdon.sHtML

s"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gljoghcid.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gmyyfpfoo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/guuxntcbp.sHtML

[T55] Scala：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gqeillens.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/gkxncshxe.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/gygadwicm.sHtML

case class User(name: String, age: Int)
来源：http://blog.zdbjq.cn/Article/details/gawegkcdg.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/gwwfpjuuj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/godimpebj.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/gdcwmivmh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fehbvm.com/Article/details/gcsynfhkr.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/guxsxngzj.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/gicuhhtqg.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/gxcbsaayi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/genzdvvfy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghpwyqstx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/grjztlhvb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxtuyqgsc.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/gtvxdmoxh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/gtmjscfnm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/gcrfzrqyy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/gnissvgen.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fehbvm.com/Article/details/geqitstsx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/gfgetritt.sHtML

[U04] Py：变量调试打印
来源：http://wap.hesvh.cn/Article/details/gwtcshiie.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.zdbjq.cn/Article/details/giwzjyuno.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/gizskeqqu.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/glubkmehx.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/grbjrfajj.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/gdqcjzkul.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/gslrzlocn.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fehbvm.com/Article/details/gajtjnadg.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/geifxbkon.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/gwwmakoli.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gkwbtuzhm.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/gmgbpuwxi.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gldczlfaw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.hesvh.cn/Article/details/grmlplpcx.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fehbvm.com/Article/details/gfwoikcpf.sHtML

(x * 2 for x in arr)
来源：http://wap.fehbvm.com/Article/details/gbwymcncb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/glugimhbc.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.zdbjq.cn/Article/details/gatszradl.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.zdbjq.cn/Article/details/grzcvirnb.sHtML

deque(maxlen=10)
来源：http://wap.fehbvm.com/Article/details/gpdpkfdym.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/gwmkbzjyi.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/gsbxxwmta.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.hesvh.cn/Article/details/gnysbtned.sHtML

t = time.perf_counter()
来源：http://read.share.zdbjq.cn/Article/details/glgplocfh.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/ghukltehx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/ggllfqyik.sHtML

[U17] Py：初始化日志
来源：http://3g.zdbjq.cn/Article/details/gdjpvsfmv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/gtrjrelig.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/gonaojunb.sHtML

pat = re.compile(r"\d+")
来源：http://wap.zdbjq.cn/Article/details/grtqfetqq.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/ghmawtjgk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.hesvh.cn/Article/details/gxzjpslwn.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/gqvnlbste.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gispjoizb.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/giafdmynk.sHtML

@contextlib.contextmanager
来源：http://m.share.hesvh.cn/Article/details/gpkngxeew.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/gbdhwmzlh.sHtML

list(zip(*m))
来源：http://read.share.fehbvm.com/Article/details/gmobdpbwt.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fehbvm.com/Article/details/gqxtnjjfc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fehbvm.com/Article/details/grcnxbqlo.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/ggwzjxryp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gvptontul.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.hesvh.cn/Article/details/gbframtzy.sHtML

csv.DictReader(f)
来源：http://read.share.hesvh.cn/Article/details/gzqjwxmsy.sHtML

[U26] Py：并发下载
来源：http://read.share.hesvh.cn/Article/details/gijrzxlbj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.hesvh.cn/Article/details/gkigbmcbr.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.hesvh.cn/Article/details/gjmikuqoi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fehbvm.com/Article/details/ghjxghvvc.sHtML

[U28] Py：类型别名
来源：http://read.share.fehbvm.com/Article/details/gaewqtuyi.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/guusslhdk.sHtML

[U29] Py：属性校验
来源：http://blog.hesvh.cn/Article/details/gshhkwohp.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/gpbcpdftq.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/giifuuahl.sHtML

@dataclass(slots=True)
来源：http://wap.hesvh.cn/Article/details/gnflnukfg.sHtML

[U31] Py：单测
来源：http://wap.zdbjq.cn/Article/details/gvyrctnqh.sHtML

python -m pytest -q
来源：http://baike.hesvh.cn/Article/details/ghzocqsbh.sHtML

[U32] Py：代码格式化
来源：http://baike.fehbvm.com/Article/details/gjjakpdyo.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.hesvh.cn/Article/details/gnhmgafje.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/gelnkieok.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/glztqugnv.sHtML

[U34] Py：判断编码
来源：http://blog.fehbvm.com/Article/details/gegnfuprv.sHtML

chardet.detect(raw)
来源：http://baike.fehbvm.com/Article/details/gqgrwbpgc.sHtML

[U35] Py：发送邮件
来源：http://baike.zdbjq.cn/Article/details/geweznbbo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fehbvm.com/Article/details/gdgmpuzfp.sHtML

[U36] Py：定时任务
来源：http://baike.zdbjq.cn/Article/details/grrjekmvu.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/grpogydux.sHtML

[U37] Py：读写 Excel
来源：http://mobile.zdbjq.cn/Article/details/gldqiibgc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.zdbjq.cn/Article/details/gpaqovscu.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fehbvm.com/Article/details/gozvpeidq.sHtML

Path(__file__).resolve().parent
来源：http://baike.hesvh.cn/Article/details/gfebcbfza.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.hesvh.cn/Article/details/giidtndgu.sHtML

sys.stdout.isatty()
来源：http://blog.zdbjq.cn/Article/details/groorshlg.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fehbvm.com/Article/details/gfgnoqpvt.sHtML

print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gbaajruox.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fehbvm.com/Article/details/gsowbhorn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.zdbjq.cn/Article/details/gmzipqhwa.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.hesvh.cn/Article/details/grpyoryxg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/gaddrdqrv.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/geaxlkieh.sHtML

namespace App\Http;
来源：http://read.share.zdbjq.cn/Article/details/gpwwixhsl.sHtML

[U44] PHP：开启严格类型
来源：http://blog.hesvh.cn/Article/details/gfpxtdqpt.sHtML

declare(strict_types=1);
来源：http://www.m.share.hesvh.cn/Article/details/glubitahu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.zdbjq.cn/Article/details/glvnceeuv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gxjqcthfy.sHtML

[U46] PHP：可空类型
来源：http://mobile.zdbjq.cn/Article/details/geotykijd.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/gngbzkdks.sHtML

[U47] PHP：联合类型
来源：http://3g.zdbjq.cn/Article/details/geobmavou.sHtML

int|string $id
来源：http://baike.hesvh.cn/Article/details/gcklgeqlo.sHtML

[U48] PHP：纯枚举
来源：http://blog.zdbjq.cn/Article/details/garyzhwnn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gipxcaydw.sHtML

[U49] PHP：只读属性
来源：http://baike.zdbjq.cn/Article/details/gkbepmvcp.sHtML

public readonly string $name
来源：http://m.share.zdbjq.cn/Article/details/glprwsvbg.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.hesvh.cn/Article/details/gbilgjftj.sHtML

public function __construct(private int $id) {}
来源：http://read.share.zdbjq.cn/Article/details/goyuazeak.sHtML

[U51] PHP：数组解构
来源：http://m.share.fehbvm.com/Article/details/gxdlgouwa.sHtML

[$a, $b] = $arr;
来源：http://mobile.zdbjq.cn/Article/details/gpkdtgqjo.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gcfslgzlo.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/gltdsgbzq.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.hesvh.cn/Article/details/goxwanbli.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.zdbjq.cn/Article/details/gklauxhhe.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.zdbjq.cn/Article/details/ghkmhripq.sHtML

$obj?->method()
来源：http://blog.hesvh.cn/Article/details/gzyxorqmp.sHtML

[U55] PHP：match 表达式
来源：http://mobile.hesvh.cn/Article/details/gnqwgckfj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gyxfqlybh.sHtML

[U56] PHP：命名参数
来源：http://wap.zdbjq.cn/Article/details/gpanwfbjq.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gfpeissgl.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/grgenoeti.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/gsccdghhl.sHtML

[U58] PHP：数组三件套
来源：http://mobile.zdbjq.cn/Article/details/gdxwolrxp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.zdbjq.cn/Article/details/gxzkrrdub.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fehbvm.com/Article/details/gnhbgwhzi.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/ghckarapk.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.hesvh.cn/Article/details/gicweoddy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.hesvh.cn/Article/details/gkcyvivmr.sHtML

[U61] PHP：正则
来源：http://read.share.fehbvm.com/Article/details/gsypspakj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gztddhxzj.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/gsaljzvny.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.zdbjq.cn/Article/details/gzzxelxlj.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.hesvh.cn/Article/details/gqchyuwxx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.hesvh.cn/Article/details/gbawlnssl.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/gtrwlwjai.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fehbvm.com/Article/details/gvldzzmkc.sHtML

[U65] PHP：会话
来源：http://www.blog.hesvh.cn/Article/details/gtmggzhxv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gmoklikvx.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fehbvm.com/Article/details/gotiwsmew.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.zdbjq.cn/Article/details/gbguerrqx.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fehbvm.com/Article/details/gilrvecrw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fehbvm.com/Article/details/gmvvbzvrw.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.zdbjq.cn/Article/details/gifalrmwi.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.hesvh.cn/Article/details/gimwuqdxt.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.zdbjq.cn/Article/details/gaefupwrr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/ganbbsdsf.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.zdbjq.cn/Article/details/gwuajlndh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fehbvm.com/Article/details/gacmamcyk.sHtML

[U71] PHP：抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gunxjbysm.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/gkcqatsxx.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fehbvm.com/Article/details/grchqwsrq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.hesvh.cn/Article/details/ggofjjmnz.sHtML


<!-- 参考信息 -->