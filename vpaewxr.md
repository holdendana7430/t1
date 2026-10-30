代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gtgdfnkgh.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gfqixsrzs.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gfngjishs.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gocmqzrjy.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gaztfmdqh.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/gnkjtbder.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gpgpiylit.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gtzvxecxx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gecmgudds.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gakrthpfu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/gswwxcckq.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/gzjcvjzqu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gogsbijad.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gibzonzuo.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/gmxnyxgjy.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gjmzmftwa.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/guademdyd.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/gayabyrse.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gyoockmid.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gokgukddk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gcsldtuhd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzplwifwj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gsnverprv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwvkbmnxn.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gcnnvdzfk.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/genptmgnc.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gxhihhqni.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gtqtheznn.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gxebxpnbp.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gjcqvwilb.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/gglvxicso.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gmhdbmext.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gaacdwmxn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/grprautjo.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gynmvzvhc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/glmrkuise.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/glalmypwi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gpuzzdobe.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gzjrexktp.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/guityaowm.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gvvrdmdhi.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gjtspjzml.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/grsdtjuaq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/gmkjsywvg.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/ggqbxjpwh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gvaobspgy.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/glzyztayp.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/ghtjorrdd.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gwnjrpkft.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gbjhaqlff.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gbpvjoomv.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gxgrcseyc.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/grjhjjepp.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gsyjwclpk.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/ghfkdhzaj.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gixbtrgue.sHtML

[T17] Swift：变量与常量
来源：http://m.share.hesvh.cn/Article/details/guntdmsud.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/gsaiaxtgu.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gxxplpukg.sHtML

"值: \(b)"
来源：http://mobile.fehbvm.com/Article/details/gvtsbhivd.sHtML

[T19] Swift：可选绑定
来源：http://www.share.hesvh.cn/Article/details/gixaiionq.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/gwbapqngj.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/gewotrjpr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gtjzqenet.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/geebqmpzp.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/gyftxtzvy.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/gurmsvgwy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/graneqjci.sHtML

[T23] Swift：函数
来源：http://m.share.zdbjq.cn/Article/details/gbbzeecyi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/gpmonwzse.sHtML

[T24] Swift：闭包
来源：http://wap.hesvh.cn/Article/details/gxcepenli.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gesregoli.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/gpwxoskaa.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gjdnpliuz.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gzcnrmyrb.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/ggsyjykej.sHtML

[T27] Swift：错误处理
来源：http://read.share.hesvh.cn/Article/details/gsjsjdsfb.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/gsqfmaiwk.sHtML

[T28] Swift：枚举
来源：http://3g.zdbjq.cn/Article/details/gyqtadxud.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/geqcyimix.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/giynrwuze.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/gzfctcgjw.sHtML

[T30] Swift：协议
来源：http://www.share.zdbjq.cn/Article/details/gcfsgegbf.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gkohzftfx.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gvusfmqzr.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gwnfhguyy.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gdbhybzel.sHtML

local a = 1
来源：http://wap.hesvh.cn/Article/details/gzqwjvshr.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/gsjoekqka.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/gsqjynjdd.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/gpueukbfh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gmrryzszp.sHtML

[T35] Lua：字典表
来源：http://read.share.fehbvm.com/Article/details/gvmasubmn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fehbvm.com/Article/details/gfewqqtzp.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/grldkwxsn.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/gknslvhlp.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gvhnucpwp.sHtML

"a" .. "b"
来源：http://www.m.share.zdbjq.cn/Article/details/gacflydpz.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/gppvxuhpa.sHtML

if x > 0 then print("正") end
来源：http://www.share.zdbjq.cn/Article/details/gfjeaxoyt.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gcgkcltkm.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/ggbiwzmuu.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/gnkqluhqf.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.hesvh.cn/Article/details/gbgpnigdh.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/ghczvckjl.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/gwrnsnnza.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/guunjysfr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/gdmwhlfwq.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/gegunvozk.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/gwnkygcrj.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/gyhsoabgu.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gcnebejxw.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/gefxviaph.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.zdbjq.cn/Article/details/grdfbufpx.sHtML

[T46] Perl：哈希操作
来源：http://m.share.zdbjq.cn/Article/details/gzjtrmogt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.hesvh.cn/Article/details/ghrycqlnt.sHtML

[T47] Perl：正则捕获
来源：http://www.share.zdbjq.cn/Article/details/gzbkalwex.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gamclqftd.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/gjlqktwvk.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/gkgoeyjyl.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/ghuqmshzu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/ginvdnkwj.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gygxreksh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/ggsajegnx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gacfvjblq.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/gmeajmljh.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gtlisvfli.sHtML

[T52] Scala：变量
来源：http://read.share.zdbjq.cn/Article/details/gjtnnjycs.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gzvowkiym.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gbfxsljnj.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gckehtzqq.sHtML

[T54] Scala：集合映射
来源：http://www.share.hesvh.cn/Article/details/giffnizwg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/giievitjm.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gzxbwhvfk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/gsyulsmjt.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/gxjctleos.sHtML

case class User(name: String, age: Int)
来源：http://3g.fehbvm.com/Article/details/gposevfgu.sHtML

[T57] Scala：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gxdhlruls.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/gzqpmkzdf.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/gonpbudyn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.zdbjq.cn/Article/details/gqhnozzzd.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/ggmbwnfhm.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/gwglycftp.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/grmcsktmg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/gvsvtxvcr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/geyvoojba.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/ghbvjuuxd.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzrwgdmkz.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/gwagdpyud.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fehbvm.com/Article/details/gcxryxlfo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/gcoipjhpc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fehbvm.com/Article/details/gvpvplpbf.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gowjdjjpj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/gbifzmbkl.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/gzbkmecdt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/gfffnlpae.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/ghhzlstza.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gsqstoxcq.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/giisbnfpk.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/gidochqkt.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/givtlwjty.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/gvrikwshi.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/ghmxdojqm.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/gxbokglpu.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/gxadfsoos.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/gqpfhbfca.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/ginfelrba.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.zdbjq.cn/Article/details/gqvpdzbav.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/gkdhdbjpk.sHtML

(x * 2 for x in arr)
来源：http://baike.fehbvm.com/Article/details/godrinjdu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/giuaixqih.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/gpstandku.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.zdbjq.cn/Article/details/gnrgsflnq.sHtML

deque(maxlen=10)
来源：http://blog.zdbjq.cn/Article/details/gjspvubyk.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.hesvh.cn/Article/details/gxxaeogfi.sHtML

defaultdict(list)
来源：http://www.m.share.hesvh.cn/Article/details/gpgcublzh.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/gjvtwwofo.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/glflzuxwf.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/gldobnqvc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/ghdinrbbt.sHtML

[U17] Py：初始化日志
来源：http://3g.fehbvm.com/Article/details/gtxchhmdv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.hesvh.cn/Article/details/gsvwgzxau.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/ggoubgcrw.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/glxewrumj.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/gmbskojag.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/goyoppagx.sHtML

[U20] Py：缓存函数结果
来源：http://wap.zdbjq.cn/Article/details/gvfxwjxxd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/gdxgrmmdd.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.zdbjq.cn/Article/details/grzdcvwxw.sHtML

@contextlib.contextmanager
来源：http://baike.zdbjq.cn/Article/details/gunueqrjc.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/gthkdyatg.sHtML

list(zip(*m))
来源：http://wap.fehbvm.com/Article/details/gvshgodtg.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/gimtmgdzu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/gdmronscg.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/gvpwmadrp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gcbwyvdsj.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fehbvm.com/Article/details/gouekeazv.sHtML

csv.DictReader(f)
来源：http://wap.hesvh.cn/Article/details/ggndizbzp.sHtML

[U26] Py：并发下载
来源：http://3g.hesvh.cn/Article/details/gqaefojky.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.zdbjq.cn/Article/details/gvrvhcfat.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/goczqxrud.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/gplwzfavy.sHtML

[U28] Py：类型别名
来源：http://www.share.hesvh.cn/Article/details/gnrqnwkkp.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/gycgupxzc.sHtML

[U29] Py：属性校验
来源：http://3g.fehbvm.com/Article/details/gusjhdhuu.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fehbvm.com/Article/details/gmrohxksn.sHtML

[U30] Py：数据类
来源：http://wap.fehbvm.com/Article/details/gqwfwiefy.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gbuwwmcdk.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/gwksnxjav.sHtML

python -m pytest -q
来源：http://3g.hesvh.cn/Article/details/gjaisryte.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/gqjhsiknr.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/gyroldouc.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/geqqtpmiq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/gikcvwlxq.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/glxfefaft.sHtML

chardet.detect(raw)
来源：http://wap.fehbvm.com/Article/details/ggpwotave.sHtML

[U35] Py：发送邮件
来源：http://m.share.hesvh.cn/Article/details/gilekkmgi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/glzsbgqgc.sHtML

[U36] Py：定时任务
来源：http://www.m.share.hesvh.cn/Article/details/glhdtyvwb.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fehbvm.com/Article/details/givhntojq.sHtML

[U37] Py：读写 Excel
来源：http://www.share.zdbjq.cn/Article/details/gsttbvkpt.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.zdbjq.cn/Article/details/grboplcjp.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.hesvh.cn/Article/details/gdhlwfxjt.sHtML

Path(__file__).resolve().parent
来源：http://wap.fehbvm.com/Article/details/gcqpmyftn.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/gbmkvmxup.sHtML

sys.stdout.isatty()
来源：http://3g.hesvh.cn/Article/details/griuuikoa.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fehbvm.com/Article/details/gdtdabqkd.sHtML

print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/grqxpvszr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fehbvm.com/Article/details/gmetiebsg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.hesvh.cn/Article/details/glhbdnflu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gsblgfbbs.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.hesvh.cn/Article/details/gqapdesou.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/gmvaiyccs.sHtML

namespace App\Http;
来源：http://www.share.zdbjq.cn/Article/details/gzpesukwx.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gpkivzhdh.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/gdyttwjhx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.hesvh.cn/Article/details/gscfmgefx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gqffpparz.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/ghgyaxcxb.sHtML

?string $name = null
来源：http://www.share.hesvh.cn/Article/details/gvghisrbo.sHtML

[U47] PHP：联合类型
来源：http://m.share.zdbjq.cn/Article/details/gblnqxkoc.sHtML

int|string $id
来源：http://www.m.share.fehbvm.com/Article/details/gpljaqjjf.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.hesvh.cn/Article/details/gzdieymkn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fehbvm.com/Article/details/guwqtvxmh.sHtML

[U49] PHP：只读属性
来源：http://m.share.hesvh.cn/Article/details/gylpbctmh.sHtML

public readonly string $name
来源：http://m.share.fehbvm.com/Article/details/gmnpcxltq.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.hesvh.cn/Article/details/gwgoppjnq.sHtML

public function __construct(private int $id) {}
来源：http://mobile.zdbjq.cn/Article/details/gxkvcrvyb.sHtML

[U51] PHP：数组解构
来源：http://3g.fehbvm.com/Article/details/gplezlfqs.sHtML

[$a, $b] = $arr;
来源：http://read.share.zdbjq.cn/Article/details/gmmauuqsk.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/gbayooslp.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.zdbjq.cn/Article/details/gtgnmaezg.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fehbvm.com/Article/details/gpgwuyexz.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.hesvh.cn/Article/details/gxsgctggd.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fehbvm.com/Article/details/gdtdvurxp.sHtML

$obj?->method()
来源：http://baike.zdbjq.cn/Article/details/gxlgkpyco.sHtML

[U55] PHP：match 表达式
来源：http://read.share.zdbjq.cn/Article/details/gvysiboqc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/gvkijnwca.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/gqmswdlsm.sHtML

f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gpzsqrrqd.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gyzdteypo.sHtML

"值: {$a}"
来源：http://www.share.fehbvm.com/Article/details/gncjpiprg.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/ghytwpaxv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.zdbjq.cn/Article/details/gqzbtoate.sHtML

[U59] PHP：自定义排序
来源：http://m.share.zdbjq.cn/Article/details/gxlsrixpa.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gtszdpwjd.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fehbvm.com/Article/details/gixaxjgrk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fehbvm.com/Article/details/gtrpwquyc.sHtML

[U61] PHP：正则
来源：http://www.blog.hesvh.cn/Article/details/girmqsxlh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/ghzgpwzkl.sHtML

[U62] PHP：日期对象
来源：http://mobile.fehbvm.com/Article/details/gwhorkmev.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fehbvm.com/Article/details/gdosfohvm.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.zdbjq.cn/Article/details/gtikhjhxs.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fehbvm.com/Article/details/gbtkpqjem.sHtML

[U64] PHP：目录遍历
来源：http://blog.zdbjq.cn/Article/details/gbffdpykx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/gdebstkgh.sHtML

[U65] PHP：会话
来源：http://read.share.hesvh.cn/Article/details/gkhdvitvs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gezggzxyu.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.zdbjq.cn/Article/details/gwczlmfyb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fehbvm.com/Article/details/gpenrnalv.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/gkjbfzkau.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/glspdnxir.sHtML

[U68] PHP：PDO 连接
来源：http://blog.hesvh.cn/Article/details/gepxxgqrl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.zdbjq.cn/Article/details/gdecnxfbn.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/gqilufeze.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.zdbjq.cn/Article/details/gtmrcnbcv.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.zdbjq.cn/Article/details/gwsjjgoxf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.hesvh.cn/Article/details/gmkuwrdvn.sHtML

[U71] PHP：抛出异常
来源：http://baike.fehbvm.com/Article/details/gxzqglxfq.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gmdlfetks.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/gobiemlkp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fehbvm.com/Article/details/gqgpfzagd.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fehbvm.com/Article/details/ggyajxozn.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.hesvh.cn/Article/details/ghcauewds.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.hesvh.cn/Article/details/ggriqutrx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.zdbjq.cn/Article/details/ghqvomhkn.sHtML

[U75] PHP：依赖注入
来源：http://mobile.zdbjq.cn/Article/details/gupamfrlb.sHtML

composer require psr/container
来源：http://mobile.fehbvm.com/Article/details/gfqblldhk.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.hesvh.cn/Article/details/gwtljfxqy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.hesvh.cn/Article/details/grmcrggun.sHtML


<!-- 参考信息 -->