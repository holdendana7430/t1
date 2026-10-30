代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gffnndzxc.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/gmeulhyas.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/gwwmjdrcl.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/gqbalpnmk.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/guucpbqme.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/goviwzhyt.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gavtnklur.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gblhbdipx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gsjfkytsy.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/gcrkerbth.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gdilpqnym.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gamjatfbx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fehbvm.com/Article/details/gtzfwhnrr.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/gvcjuoudk.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gifjqmohm.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gqpyctnzv.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/ggiquadue.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gcldkrmlk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/gkzcdcwrd.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gcrnpmyay.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/godjaiypw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqxoxxtec.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gjewotmxv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glcoojehs.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/ghjjnywgc.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/godgilkvs.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/gitonkcuf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gzivkrwur.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gclyveedj.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gcujbqnoa.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/ghcqhrfpe.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/gyysadthq.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gcncwgsxf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/gcrhcidzz.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gbufkqkiu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/gycefvmaj.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gmwjcovmy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gawildyjr.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gnehxstbu.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/gvwsnvqbb.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/ggwqwjagl.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gobnyxalg.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/glhhsphgn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gmqnyelql.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/gnvtjvksi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/gbwzjclan.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/glmsfpsmq.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gzanufdpf.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/gfouczoyb.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/gtougdrvc.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/gggrpjvnv.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/gyvcnalfm.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gcgbdxajp.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gwgofrztz.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/guatgkgiy.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gyrcluqlx.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/gwbpkbzro.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/geqnojzti.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gnqxdrgrl.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gpirlfyui.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/guwakbrfi.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/glaoqppmk.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gfizurqfo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/gekrwktwb.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/gybwggbgj.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/gmvvbugxf.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/givukymek.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/grhthqdqg.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/gpegoxnkm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/gsdddzgck.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/gyadjnebs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gefhblibn.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gxvubjiiy.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/glkdkrmhy.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/gmnhguhdk.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/gpyygxdjs.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gqqaxrcvj.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gdhbrwqew.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/grjrlyjlt.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gjbnwhpmp.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gemlxrgki.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gbrxpmakz.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/ggdoezrhi.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/girmsrttl.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/gqymwjzgi.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/ghrbciqnh.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gcrvvrtyw.sHtML

local a = 1
来源：http://wap.hesvh.cn/Article/details/grqbpayns.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/ghbebcbia.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/geeixvmxl.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/gmtzjcfhj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gnprflpub.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/giqhojbni.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/gimpesgjc.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gqufbmiln.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/gmkpolwsr.sHtML

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/gelmfnvtw.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/ghhjwwldo.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/gfxtotbhl.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gfdwspnhg.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gvtqzyoxa.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/gmwdjdupj.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/gxxstqjqr.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/gkwkxczmv.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/gyhogezge.sHtML

print "Hello\n";
来源：http://www.blog.fehbvm.com/Article/details/gjpnziekz.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gzikgpnps.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/ghsecamos.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gzxfpmtas.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/gntoejfqg.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gtxwyltle.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gnrhczqzs.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/gwhvxbvwx.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghknpgynt.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/gkivrpqmq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/gkmyntcki.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/gdfndoeoz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.zdbjq.cn/Article/details/gvhgffvzb.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gbfyoehlk.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/gklqsdcux.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/gbuwkvqpx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gafiezzwl.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gzfzdiuaw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.hesvh.cn/Article/details/geljmiesi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gwsbkxqoj.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/ghbiwswub.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gceyikejg.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/gdsabvbfz.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/gyskcgnjp.sHtML

[T53] Scala：字符串插值
来源：http://wap.fehbvm.com/Article/details/gjczjjybs.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gawlhoaja.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/giihagtqf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/gbjpkctnj.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gzhxroeks.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.hesvh.cn/Article/details/gdfavlgzg.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/gjhazpcji.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/gyffatrun.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gabtldvny.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/gzemoxrlr.sHtML

[T58] Scala：函数定义
来源：http://baike.fehbvm.com/Article/details/gkaddlfqj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fehbvm.com/Article/details/ggfhwjacy.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gqnzicyjm.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/gqsuqxsip.sHtML

[T60] Scala：折叠
来源：http://baike.hesvh.cn/Article/details/gundqumfm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fehbvm.com/Article/details/gmtthaqaf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/greukowet.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gefazqvnm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggvcdzrhv.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fehbvm.com/Article/details/gocbdvxzk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/gsyrmouyr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gurngekbl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/gshfnzjza.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gpaidjkiz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/ghcrdxily.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gwfeszejt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/gwkpwwhaj.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.zdbjq.cn/Article/details/gyiawrjah.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gmsrbwcky.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/grzoyhefp.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/ggxlvtqgh.sHtML

[U07] Py：反转字典键值
来源：http://blog.hesvh.cn/Article/details/gtvvmcnsq.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/gagvahqrd.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gtnifsxca.sHtML

[y for x in nested for y in x]
来源：http://www.share.zdbjq.cn/Article/details/grnvsijdk.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/ggcocxlfm.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gyrlnfxiw.sHtML

[U10] Py：按值排序字典
来源：http://mobile.zdbjq.cn/Article/details/gqxvontrb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fehbvm.com/Article/details/groilyuxc.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/gguzyfoxt.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/ggtmsqwyj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.hesvh.cn/Article/details/gjifetlwv.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fehbvm.com/Article/details/gqumfegdo.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/gigxhobbe.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/giddfutud.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fehbvm.com/Article/details/gkvnwrgwi.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/gyijmcipl.sHtML

[U15] Py：高精度计时
来源：http://read.share.hesvh.cn/Article/details/gujzmjgef.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/gltkprggh.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/gjdbvethd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fehbvm.com/Article/details/gaatycohp.sHtML

[U17] Py：初始化日志
来源：http://baike.zdbjq.cn/Article/details/gxpgdvkob.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.hesvh.cn/Article/details/gwrrdbegy.sHtML

[U18] Py：预编译正则
来源：http://baike.hesvh.cn/Article/details/gqyqnecwa.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/getnmonot.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/gkarjdboo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/gjotyaftq.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.zdbjq.cn/Article/details/gdhnspxwk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/gxenzrrvg.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fehbvm.com/Article/details/gfqosuuxt.sHtML

@contextlib.contextmanager
来源：http://wap.hesvh.cn/Article/details/gxidrxfyq.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/ghndvnxtb.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gdvbxhzhd.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/gxnjtazhc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.hesvh.cn/Article/details/gtrsfwqci.sHtML

[U24] Py：路径操作
来源：http://3g.zdbjq.cn/Article/details/gxenkzxix.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gveacmjng.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/gdxetsxqg.sHtML

csv.DictReader(f)
来源：http://mobile.fehbvm.com/Article/details/gugshbxnv.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/gmuttmulq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/gkuxuwunv.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.zdbjq.cn/Article/details/gfhhoibmk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.zdbjq.cn/Article/details/gdegjnikz.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/gvfflruoi.sHtML

UserId = int
来源：http://www.m.share.zdbjq.cn/Article/details/gcqwrlyvf.sHtML

[U29] Py：属性校验
来源：http://www.share.zdbjq.cn/Article/details/gnhjysdak.sHtML

@property 与 @x.setter 配合
来源：http://3g.hesvh.cn/Article/details/gweyrtpcc.sHtML

[U30] Py：数据类
来源：http://baike.fehbvm.com/Article/details/gkpjbaxbh.sHtML

@dataclass(slots=True)
来源：http://blog.zdbjq.cn/Article/details/gezestcon.sHtML

[U31] Py：单测
来源：http://m.share.hesvh.cn/Article/details/ggkqphdhd.sHtML

python -m pytest -q
来源：http://mobile.zdbjq.cn/Article/details/gilijtduc.sHtML

[U32] Py：代码格式化
来源：http://wap.zdbjq.cn/Article/details/gcpdxvtob.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.zdbjq.cn/Article/details/gmjmcgmms.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/ghqecgpdo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/ghtpobfui.sHtML

[U34] Py：判断编码
来源：http://www.m.share.zdbjq.cn/Article/details/gdspkocqu.sHtML

chardet.detect(raw)
来源：http://m.share.hesvh.cn/Article/details/gjbsproyq.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/grjnmlcch.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.zdbjq.cn/Article/details/grnbqxjco.sHtML

[U36] Py：定时任务
来源：http://mobile.fehbvm.com/Article/details/gapaosykm.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.zdbjq.cn/Article/details/gdrfntnpv.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fehbvm.com/Article/details/grujghlze.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fehbvm.com/Article/details/gzeqxjurm.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.zdbjq.cn/Article/details/govyypalz.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fehbvm.com/Article/details/giwddkwwr.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/gpzkpjgjt.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/gsrgbnvcb.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.zdbjq.cn/Article/details/gvcynuftj.sHtML

print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gzrftibrc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.zdbjq.cn/Article/details/gcsjyxyqc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.hesvh.cn/Article/details/gfubsgxyo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/gnyyvskzd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fehbvm.com/Article/details/gathwbkss.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gvwemcpqd.sHtML

namespace App\Http;
来源：http://3g.hesvh.cn/Article/details/gruewadgb.sHtML

[U44] PHP：开启严格类型
来源：http://3g.zdbjq.cn/Article/details/gotcbmmax.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/gkraoszdy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.hesvh.cn/Article/details/gdqbfnlir.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/grfwkmdfk.sHtML

[U46] PHP：可空类型
来源：http://blog.zdbjq.cn/Article/details/gujhowuej.sHtML

?string $name = null
来源：http://www.share.zdbjq.cn/Article/details/gyafkdffe.sHtML

[U47] PHP：联合类型
来源：http://m.share.hesvh.cn/Article/details/geaumiwcr.sHtML

int|string $id
来源：http://wap.hesvh.cn/Article/details/gxbziglsl.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/gxkcmtuqn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/gnpozwtkz.sHtML

[U49] PHP：只读属性
来源：http://www.blog.hesvh.cn/Article/details/gajwlcctz.sHtML

public readonly string $name
来源：http://blog.hesvh.cn/Article/details/gxtsokdxx.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.hesvh.cn/Article/details/gpvuiwssz.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/gbejwoecq.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/ghlaqlxed.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/gbflbiejo.sHtML

[U52] PHP：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gdyfenofl.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gcpwibjek.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gldfzarje.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.zdbjq.cn/Article/details/gjffzfpcj.sHtML

[U54] PHP：空安全调用
来源：http://www.share.zdbjq.cn/Article/details/gozbnzkoz.sHtML

$obj?->method()
来源：http://read.share.hesvh.cn/Article/details/giviksegg.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/guenpcgsv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/glmmoxqnf.sHtML

[U56] PHP：命名参数
来源：http://wap.hesvh.cn/Article/details/gabieafql.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gpwkqeiul.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gunsciyez.sHtML

"值: {$a}"
来源：http://www.blog.zdbjq.cn/Article/details/gjabzxmbp.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/gzwvjopct.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fehbvm.com/Article/details/gvksndkbl.sHtML

[U59] PHP：自定义排序
来源：http://wap.hesvh.cn/Article/details/gzgibeyks.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gyndufelp.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/ghkwlsgaz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/gcqurtggu.sHtML

[U61] PHP：正则
来源：http://baike.hesvh.cn/Article/details/glpxpojgp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/gcuxwlzjj.sHtML

[U62] PHP：日期对象
来源：http://read.share.hesvh.cn/Article/details/ghmudvoxs.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/gsjhcmwhl.sHtML

[U63] PHP：文件读写
来源：http://www.blog.hesvh.cn/Article/details/gtszeoatf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.hesvh.cn/Article/details/gmkrjieok.sHtML

[U64] PHP：目录遍历
来源：http://blog.hesvh.cn/Article/details/gedsvfvoi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.hesvh.cn/Article/details/gzlucndyl.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/gamtuicuv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/gqtbatmej.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/gdfmykole.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.zdbjq.cn/Article/details/goomufgbj.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/gviilffsk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.zdbjq.cn/Article/details/gagbejwbu.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fehbvm.com/Article/details/gswccguid.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/gvhrygkkt.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fehbvm.com/Article/details/gbhlnrgsp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gfltxkogl.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/ggoywuxqv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.hesvh.cn/Article/details/gjyuaxrxk.sHtML

[U71] PHP：抛出异常
来源：http://3g.fehbvm.com/Article/details/ggwuqnxba.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.hesvh.cn/Article/details/gucarhazr.sHtML

[U72] PHP：写错误日志
来源：http://3g.hesvh.cn/Article/details/gvyepwwhi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.hesvh.cn/Article/details/gaarrhlia.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.zdbjq.cn/Article/details/gakdfwrdp.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.hesvh.cn/Article/details/gjilevjzi.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/ghqguscaq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.zdbjq.cn/Article/details/gpwsghpji.sHtML

[U75] PHP：依赖注入
来源：http://3g.fehbvm.com/Article/details/gbxmwgvds.sHtML

composer require psr/container
来源：http://www.share.zdbjq.cn/Article/details/grpscpqhl.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/gvxszxnhb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.hesvh.cn/Article/details/gtrrnrdgu.sHtML


<!-- 参考信息 -->