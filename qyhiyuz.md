代发 wailian999

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gcxbiygqa.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gpzulmfad.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gqfgwxlnc.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/gtcwahppo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gjqhpkuqa.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/ggzwrtlit.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gyebxxoqj.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gulhcvwof.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/gnuejewtb.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/gunkzqvbz.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gfapebbfu.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/grgasodac.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gbkhetapg.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/groehmnwo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/gnrbczpqk.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gaasvbkmo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/ghzsobage.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmedjvwdk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gpzxzmukx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghijbhzgh.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gasywuijk.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gtlvrzatz.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gsrzildsz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gzcolwtwz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/gzqgckuwg.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gijuwbqwo.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gzfgdnlby.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/ggsrebwst.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/gqitkumsy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gvifzuzqa.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gzbaavfzf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gcazbjexu.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gudejamnk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gppstfgri.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/gwmywtpgj.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/ghflxkdnx.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gchtsaiuk.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gsqqktncb.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/gefnyrref.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/guaycapfp.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/gwaaaqobd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/geintfvlk.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/ghqkucvee.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gxqpibqhs.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/gxrtnnnck.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/ghrwdwajj.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/gcjimggwk.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gjgmeexkh.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gpruuacpn.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/gogqwgrsh.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gbhfcawlk.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/ggkntufqp.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fehbvm.com/Article/details/gctodokjt.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gnzebmuxe.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gtzmsxpfg.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/gdjrcaqek.sHtML

[T19] Swift：可选绑定
来源：http://m.share.zdbjq.cn/Article/details/gpbzqmhrr.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/gzramxinp.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/giflyflki.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/ghzhclkbr.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/ghlkhaova.sHtML

for x in a { print(x) }
来源：http://3g.hesvh.cn/Article/details/gyfsowdaq.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/gwqhoxkfp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/gpwqmoehd.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/grcrllyij.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/gtdglkmyp.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/ggppmbgva.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gdhfcbvim.sHtML

[T25] Swift：结构体
来源：http://m.share.fehbvm.com/Article/details/gqgzjfrqn.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/gppnecxhi.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gosmxfatq.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gdvfxspeb.sHtML

[T27] Swift：错误处理
来源：http://blog.zdbjq.cn/Article/details/ggddxcauz.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gyxenaimd.sHtML

[T28] Swift：枚举
来源：http://www.blog.fehbvm.com/Article/details/gmmzwamxw.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/gahacymas.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/gaaojbczy.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/gblavzxjt.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/gudsnqgus.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gnewfqpek.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/gsjoceudq.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gaxnbtffw.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/glcigmios.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gxruivpoy.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/gjzayccxv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/ginjnwafh.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/gxitpfdtk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gqrwmuaea.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/glgwubayh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/gowatooet.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gdowrffdf.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gawfmdjfd.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fehbvm.com/Article/details/glqxdlkmn.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/gagientjf.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gjeugvvmm.sHtML

if x > 0 then print("正") end
来源：http://mobile.hesvh.cn/Article/details/gwdlhwemd.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/gvnminquj.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/gkpkiwtek.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/gwvtiziyr.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/gvgbjxcnv.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/gameqanpg.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gicpdghha.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/ggpjgnfea.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/gycxhobty.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gmsyltamo.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/gwdhayukm.sHtML

[T44] Perl：条件
来源：http://3g.hesvh.cn/Article/details/gspyialpa.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gahapmzsj.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fehbvm.com/Article/details/goxpecjjx.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gqunvporx.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/gvocczdut.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fehbvm.com/Article/details/grrjagkry.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/gfeqzlfiy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.zdbjq.cn/Article/details/gvaxqlbdr.sHtML

[T48] Perl：正则替换
来源：http://mobile.zdbjq.cn/Article/details/gkfzulfso.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/gnvamvzhl.sHtML

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/gjmnlsnem.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gldgjvfdh.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gefcoooah.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gqgulncvo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gepoafwre.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/gwwechhwc.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gkyqgcrvs.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/gfkmlaajy.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/ggajgdfeo.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/ggwcwsjux.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/grjjlfdgt.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/gzftxutol.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fehbvm.com/Article/details/gofdpksxi.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/gaumaxigh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/gxbgoskju.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gdjsgyhpm.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/gtzobjgla.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/gqtvrgekv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.zdbjq.cn/Article/details/grkgaxikb.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/gozconuia.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gidjsvibo.sHtML

[T59] Scala：循环
来源：http://www.share.hesvh.cn/Article/details/gggobqvba.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/gxstdpjgb.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/gcuorecib.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/gxdslwzfn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gudppmtuj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gpvrsgpbt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqmyvmilz.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/ghoyogzth.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/galfqpryu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/gksbpjsun.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/giomthvjc.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.zdbjq.cn/Article/details/goxkwgoyi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/gtwlitbhy.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/ggxeqqwop.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/gjwegduve.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.hesvh.cn/Article/details/gwcnpnsqb.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gtlvunuia.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/grkvfhpcl.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/gghedkyxh.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/gnptxwqnn.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.zdbjq.cn/Article/details/gijzzzjpn.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fehbvm.com/Article/details/gjdshabbe.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/gvudbpvje.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gswnnsttx.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gmqaziovl.sHtML

[U10] Py：按值排序字典
来源：http://baike.hesvh.cn/Article/details/gmngnsihr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fehbvm.com/Article/details/govkmnxom.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.zdbjq.cn/Article/details/guohtlqvr.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/gyfjpzunv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/gafrssbvf.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.zdbjq.cn/Article/details/goaryudte.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fehbvm.com/Article/details/ghdjhjivf.sHtML

deque(maxlen=10)
来源：http://mobile.hesvh.cn/Article/details/gmlrfodwv.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fehbvm.com/Article/details/gezchuwar.sHtML

defaultdict(list)
来源：http://3g.hesvh.cn/Article/details/gyozkmefa.sHtML

[U15] Py：高精度计时
来源：http://mobile.zdbjq.cn/Article/details/glcltpeie.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/gaqcwvror.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.zdbjq.cn/Article/details/gjiioseez.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.hesvh.cn/Article/details/gcsvsqkfn.sHtML

[U17] Py：初始化日志
来源：http://m.share.zdbjq.cn/Article/details/gqbyzwfdp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/gljvrqjxb.sHtML

[U18] Py：预编译正则
来源：http://wap.fehbvm.com/Article/details/gdggnkrrq.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gvqulkhur.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.hesvh.cn/Article/details/ggddtjlrd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/gnqdtrtur.sHtML

[U20] Py：缓存函数结果
来源：http://blog.hesvh.cn/Article/details/giinylahz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.hesvh.cn/Article/details/gkjiepcov.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.hesvh.cn/Article/details/gwekgprdm.sHtML

@contextlib.contextmanager
来源：http://www.share.zdbjq.cn/Article/details/gfzdgwvyh.sHtML

[U22] Py：矩阵转置
来源：http://3g.fehbvm.com/Article/details/gmgjmauia.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gisfbpfmx.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/gsdwuitsw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/gdbowxnpg.sHtML

[U24] Py：路径操作
来源：http://m.share.hesvh.cn/Article/details/gtmzgpdwk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/ggdzrgydq.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/geekaxeuj.sHtML

csv.DictReader(f)
来源：http://baike.fehbvm.com/Article/details/gwwitnflx.sHtML

[U26] Py：并发下载
来源：http://3g.fehbvm.com/Article/details/gghwgcfjv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.zdbjq.cn/Article/details/gknzuxxws.sHtML

[U27] Py：异步 HTTP
来源：http://baike.hesvh.cn/Article/details/gazdnvzxu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.hesvh.cn/Article/details/gsoarpiur.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/grbnvejgl.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/gpiybjxgo.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/gqayfpqpn.sHtML

@property 与 @x.setter 配合
来源：http://3g.hesvh.cn/Article/details/gohfkekam.sHtML

[U30] Py：数据类
来源：http://mobile.zdbjq.cn/Article/details/gmpsevuco.sHtML

@dataclass(slots=True)
来源：http://m.share.hesvh.cn/Article/details/gxcwcvnea.sHtML

[U31] Py：单测
来源：http://mobile.fehbvm.com/Article/details/gzanohjsr.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/gniqbdgsi.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gfrndofjt.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gbvxktudx.sHtML

[U33] Py：打包发布
来源：http://3g.zdbjq.cn/Article/details/guspeaaxa.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.hesvh.cn/Article/details/gksmkxdum.sHtML

[U34] Py：判断编码
来源：http://www.m.share.zdbjq.cn/Article/details/gtufbeofn.sHtML

chardet.detect(raw)
来源：http://www.m.share.fehbvm.com/Article/details/gxzfhpllp.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/gsnapaujg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fehbvm.com/Article/details/gsiqrcxrj.sHtML

[U36] Py：定时任务
来源：http://www.blog.fehbvm.com/Article/details/gjmkqhbxa.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fehbvm.com/Article/details/ggrtloviu.sHtML

[U37] Py：读写 Excel
来源：http://read.share.hesvh.cn/Article/details/gqwlyljnb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/gvhesldjz.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.zdbjq.cn/Article/details/gutiellta.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.zdbjq.cn/Article/details/gqlqeddsx.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fehbvm.com/Article/details/gmfpwtrso.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/gjgpndhys.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.hesvh.cn/Article/details/gaqrlcpms.sHtML

print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gfaddwjdj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.hesvh.cn/Article/details/gdkgybnpo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gxbtbrvkd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.zdbjq.cn/Article/details/gktzdnrlw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fehbvm.com/Article/details/gbagjnhnh.sHtML

[U43] PHP：声明命名空间
来源：http://wap.hesvh.cn/Article/details/ggxrnyopq.sHtML

namespace App\Http;
来源：http://m.share.fehbvm.com/Article/details/gzpqshnli.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gzntjjrsr.sHtML

declare(strict_types=1);
来源：http://www.m.share.fehbvm.com/Article/details/gyscrzlmw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/gnukhksbf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gyjpenmrj.sHtML

[U46] PHP：可空类型
来源：http://mobile.hesvh.cn/Article/details/gtymrufqt.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/gwfjvsndb.sHtML

[U47] PHP：联合类型
来源：http://www.share.hesvh.cn/Article/details/gprxmlgmx.sHtML

int|string $id
来源：http://m.share.zdbjq.cn/Article/details/gjctflghl.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/gnlantefd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.hesvh.cn/Article/details/gytbtntvb.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.hesvh.cn/Article/details/gvuljistk.sHtML

public readonly string $name
来源：http://baike.hesvh.cn/Article/details/gipdpkiuw.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.zdbjq.cn/Article/details/gstqtmans.sHtML

public function __construct(private int $id) {}
来源：http://read.share.hesvh.cn/Article/details/ghvpzwjlo.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.hesvh.cn/Article/details/gyotlmbfc.sHtML

[$a, $b] = $arr;
来源：http://baike.zdbjq.cn/Article/details/ghnzndknm.sHtML

[U52] PHP：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gkgybfswv.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fehbvm.com/Article/details/gulsvrujw.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.zdbjq.cn/Article/details/guokwjqyn.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.hesvh.cn/Article/details/gyrxnyasa.sHtML

[U54] PHP：空安全调用
来源：http://blog.fehbvm.com/Article/details/geullkhme.sHtML

$obj?->method()
来源：http://www.m.share.zdbjq.cn/Article/details/gvhvtzlme.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gyivaqcmk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/gswbkiflx.sHtML

[U56] PHP：命名参数
来源：http://3g.fehbvm.com/Article/details/gyaseanxk.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gzvdcrrsl.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gmuuiwygx.sHtML

"值: {$a}"
来源：http://www.m.share.zdbjq.cn/Article/details/gkroqjvci.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.hesvh.cn/Article/details/gdeqrhxom.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.hesvh.cn/Article/details/gqxuuysvh.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.hesvh.cn/Article/details/gwdutpsfr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gtocoauar.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/galpshsxy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.hesvh.cn/Article/details/ghgvfvmlh.sHtML

[U61] PHP：正则
来源：http://mobile.fehbvm.com/Article/details/gifgtydnf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gnmcicvpc.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/gogfdihfi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.zdbjq.cn/Article/details/gyloaptwi.sHtML

[U63] PHP：文件读写
来源：http://m.share.fehbvm.com/Article/details/glqabqxtv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fehbvm.com/Article/details/gmpuehfam.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/gguiwosdt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fehbvm.com/Article/details/gvsiifuql.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/gnrwtpvla.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gbdqobbdg.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/gdqsqwvhg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.hesvh.cn/Article/details/ghtlektbz.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fehbvm.com/Article/details/gdjuieyye.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fehbvm.com/Article/details/guzyuvcwp.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/ggosvgmqk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.hesvh.cn/Article/details/ghftvogpx.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/gdggxqwqk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.hesvh.cn/Article/details/gwfwsexqv.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.zdbjq.cn/Article/details/gxvkhjxln.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fehbvm.com/Article/details/gyfminbrw.sHtML

[U71] PHP：抛出异常
来源：http://baike.hesvh.cn/Article/details/gmjibrkix.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/gbafknpzl.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fehbvm.com/Article/details/ggvmdhyhb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.hesvh.cn/Article/details/gsqrayfmo.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.zdbjq.cn/Article/details/gtekelfwq.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fehbvm.com/Article/details/gbvphhlfi.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gzugrocqw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fehbvm.com/Article/details/gbescsftj.sHtML

[U75] PHP：依赖注入
来源：http://3g.fehbvm.com/Article/details/gmfivtwog.sHtML

composer require psr/container
来源：http://m.share.fehbvm.com/Article/details/gzvgpqmua.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/gnftnjcyr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.zdbjq.cn/Article/details/gfbqdvuas.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.hesvh.cn/Article/details/gvnnvxygu.sHtML

composer require twig/twig
来源：http://www.blog.zdbjq.cn/Article/details/gkbujohhe.sHtML

[U78] PHP：单元测试
来源：http://3g.hesvh.cn/Article/details/gqjnypjva.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fehbvm.com/Article/details/giqjgwmng.sHtML


<!-- 参考信息 -->