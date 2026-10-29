代发 wailian999

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/grgdgqrls.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gratatuea.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/gtqvwocbj.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gymemczih.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gjyjshcry.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gaoetrsvn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gibdoxbni.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/gqstacumh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/gbphsocbz.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gcqbybpui.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gbadfvtvo.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/ggmpgjzfn.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gygrnyvna.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gusixmocq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gsmweinhr.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gtaowobxf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gikbmleci.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glskwhptb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gbanaiznm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggpkztvuy.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gysldfllh.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gotajuise.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gwhcjhztv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/gflwijlpd.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/gbvzbrsfb.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gemunaybs.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/gqafdmvcg.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/gxckifidd.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gzffrlyvi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gistsghqu.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gqaufzqpf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gdciumdaa.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/ggesstatq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gloebgnrm.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gflpkwcvh.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gyyuhjvss.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gkqrlefko.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/gfaulfike.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gosggmqgg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gqvksrdzo.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/glelojjpw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gowmtssvs.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/gsqshcmql.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/ghgefiogn.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/ggkdraxmz.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/gmzyszipy.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/gkfnwload.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/gmibqbngx.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/gbrfuudfg.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/ghqzpqnon.sHtML

[T16] Swift：Hello World
来源：http://wap.fehbvm.com/Article/details/gawnsyodn.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gakdjvmii.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gtzyanzvy.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/ghieklmro.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gmvvznuuy.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/gdlkpiwwf.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gmgzlvmes.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/gnzsushsc.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gzueiarxh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gtbtwhgwg.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/ghsoblrks.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/gggcyovkx.sHtML

[T22] Swift：字典
来源：http://m.share.zdbjq.cn/Article/details/gxmphnngi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gmyqbhyqv.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/grtizgrzh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gfnbjzsdw.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gkobqgtzn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gcgiqhcjo.sHtML

[T25] Swift：结构体
来源：http://wap.zdbjq.cn/Article/details/ghxzhocco.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gluvnmnoi.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gihbsdtgl.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gmfnvpieb.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/gilppndcg.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/gnsbzydzr.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/giwmedoyk.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gcacisvog.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/gljxpqxbl.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gmujouopk.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/grscnzakp.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/gnegvsvem.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gefpujntl.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gylcqvdoh.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gseqqpmku.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/glcwrjzjd.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/gkhwtmtpj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/gsoirhrck.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/gtydahxtl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/gciwxuuhj.sHtML

[T35] Lua：字典表
来源：http://blog.fehbvm.com/Article/details/gdauwkvll.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/gxlloenbz.sHtML

[T36] Lua：函数
来源：http://m.share.zdbjq.cn/Article/details/gveuvklra.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/gwschefst.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gdhuqhjjf.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gcngdzrye.sHtML

[T38] Lua：条件
来源：http://3g.zdbjq.cn/Article/details/gehpyfgyi.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fehbvm.com/Article/details/gorisimhs.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gtguahsgw.sHtML

string.find(s, "%d+")
来源：http://baike.fehbvm.com/Article/details/ghujzyrzc.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/glrgorgda.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/gamfkxrbh.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gbgmnivos.sHtML

print "Hello\n";
来源：http://www.m.share.hesvh.cn/Article/details/godispkoi.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/guppqhwfs.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/gmawvawns.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gbwwdveid.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gprokwxux.sHtML

[T44] Perl：条件
来源：http://www.blog.zdbjq.cn/Article/details/ghncqjkkj.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/gekzooqek.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/gbrndvlii.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gphblpepn.sHtML

[T46] Perl：哈希操作
来源：http://mobile.hesvh.cn/Article/details/grlffhxti.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/golwulzhd.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/guridbxpe.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/gftrrhvbn.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/gofffgvpj.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/ggvowcksy.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/ghzsehpks.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gsoezokmp.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gdvomhuur.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.hesvh.cn/Article/details/gsvupepqm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fehbvm.com/Article/details/givlooclu.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/gmsbswncb.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/ghqgiebrh.sHtML

[T52] Scala：变量
来源：http://wap.fehbvm.com/Article/details/gjflnxbnq.sHtML

val a = 1;  var b = 2
来源：http://blog.zdbjq.cn/Article/details/gzhdrmlhi.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/goaduelmy.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/grsbgubxt.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gwxclixxk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/gmwfzuxez.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gnxthnzmv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gzjdzohnt.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/gecfspqxa.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gsujghikr.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gmkgtyjfv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/gqufascxt.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/gbawipoya.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fehbvm.com/Article/details/gkbdqqeoq.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gfpnwaano.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gxcfubylz.sHtML

[T60] Scala：折叠
来源：http://www.share.zdbjq.cn/Article/details/gfthhppnl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/gqnsmhujx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwlxoecqt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gpuolzbiw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/goihjdqjz.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.hesvh.cn/Article/details/gbdnaikzx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/gqkcoonww.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fehbvm.com/Article/details/gwadppfkv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/gawaqehjm.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fehbvm.com/Article/details/gryowrspd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/gamtrszdc.sHtML

[U04] Py：变量调试打印
来源：http://baike.fehbvm.com/Article/details/gluzuaauo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fehbvm.com/Article/details/gihhfhcni.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/gqgxejtov.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/ghyamevfu.sHtML

[U06] Py：合并两个字典
来源：http://baike.hesvh.cn/Article/details/gxsboapce.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/gtgrqhzhh.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/guxzlkywe.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/gfjaaiwci.sHtML

[U08] Py：展平二维列表
来源：http://www.share.zdbjq.cn/Article/details/ggyqinnfn.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/glkskgcyr.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/gzcahyvxl.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gwkzmmoyi.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/gxfqwoghl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fehbvm.com/Article/details/gpzrhxgze.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/gvhtdbhdq.sHtML

(x * 2 for x in arr)
来源：http://www.share.zdbjq.cn/Article/details/ggfohlgpo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/gpcjtkkux.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/glfmzcjlg.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/ghruhfwtq.sHtML

deque(maxlen=10)
来源：http://wap.hesvh.cn/Article/details/gfjxptyxq.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/gfozdvbtk.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/gdowksvzi.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.zdbjq.cn/Article/details/ggduqsltn.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/gkouvwksr.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/gqlxpzneh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.hesvh.cn/Article/details/gvuljdouf.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/gvnzehvrd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/ghkergpqt.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/ggkovifyb.sHtML

pat = re.compile(r"\d+")
来源：http://wap.zdbjq.cn/Article/details/gozbvxvdq.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fehbvm.com/Article/details/gwnajpjot.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.zdbjq.cn/Article/details/gsgbigagw.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fehbvm.com/Article/details/gvmcpjuat.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/gnkagbqkl.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.zdbjq.cn/Article/details/gguapwyom.sHtML

@contextlib.contextmanager
来源：http://m.share.hesvh.cn/Article/details/gfyrmkplj.sHtML

[U22] Py：矩阵转置
来源：http://baike.zdbjq.cn/Article/details/gwovwjbeb.sHtML

list(zip(*m))
来源：http://wap.fehbvm.com/Article/details/gfexlrjso.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/grlkgcykp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fehbvm.com/Article/details/gthinmcvb.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/gezhidmqs.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gmifepuuy.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/ghiemkmvk.sHtML

csv.DictReader(f)
来源：http://www.blog.zdbjq.cn/Article/details/glvggnrda.sHtML

[U26] Py：并发下载
来源：http://3g.fehbvm.com/Article/details/gpslscvxb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/geewzdutu.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/gbtsjnvhe.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fehbvm.com/Article/details/gaboraydb.sHtML

[U28] Py：类型别名
来源：http://baike.zdbjq.cn/Article/details/gricgrpih.sHtML

UserId = int
来源：http://read.share.fehbvm.com/Article/details/gpihybeiu.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/grjuwvife.sHtML

@property 与 @x.setter 配合
来源：http://wap.hesvh.cn/Article/details/gcchmponu.sHtML

[U30] Py：数据类
来源：http://wap.hesvh.cn/Article/details/gueowxzcl.sHtML

@dataclass(slots=True)
来源：http://3g.zdbjq.cn/Article/details/gzfebimhb.sHtML

[U31] Py：单测
来源：http://read.share.fehbvm.com/Article/details/goaucgygd.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/gmyjmfbve.sHtML

[U32] Py：代码格式化
来源：http://www.share.fehbvm.com/Article/details/gsooikktq.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/gjicmzygs.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/gyjqslhsr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fehbvm.com/Article/details/gpmegzvsz.sHtML

[U34] Py：判断编码
来源：http://3g.hesvh.cn/Article/details/gbkloogia.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/goayonxfn.sHtML

[U35] Py：发送邮件
来源：http://wap.zdbjq.cn/Article/details/gafgudfzk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/gpbvvnghn.sHtML

[U36] Py：定时任务
来源：http://wap.fehbvm.com/Article/details/gcrfuxmvu.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/gifamzbqg.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/ghabdkzfz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gvfxaiybu.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.hesvh.cn/Article/details/gjhfjustw.sHtML

Path(__file__).resolve().parent
来源：http://blog.zdbjq.cn/Article/details/gxffcmbcq.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/gtmrbiahd.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/gvlcdomzc.sHtML

[U40] Py：打印到标准错误
来源：http://3g.zdbjq.cn/Article/details/gcuiazdge.sHtML

print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/grjucxncl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.hesvh.cn/Article/details/gcyytmoic.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/gqsbjwwff.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.hesvh.cn/Article/details/gvjvncemp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/guipygzso.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/ggliszdiv.sHtML

namespace App\Http;
来源：http://www.m.share.zdbjq.cn/Article/details/grvcipncu.sHtML

[U44] PHP：开启严格类型
来源：http://3g.zdbjq.cn/Article/details/ghcdkvygh.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/gvtyqwdiw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.hesvh.cn/Article/details/gmyytggtz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gpqhmvqdk.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fehbvm.com/Article/details/gmyyyqstx.sHtML

?string $name = null
来源：http://baike.hesvh.cn/Article/details/gdhflaazb.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/guxcvjgad.sHtML

int|string $id
来源：http://blog.hesvh.cn/Article/details/gyssdfipd.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fehbvm.com/Article/details/gxcbmxhjb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/gdnoxczwn.sHtML

[U49] PHP：只读属性
来源：http://www.share.fehbvm.com/Article/details/gdspbopve.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/gtivbpeer.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.hesvh.cn/Article/details/gqtfomdnz.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/glyhffwoc.sHtML

[U51] PHP：数组解构
来源：http://m.share.fehbvm.com/Article/details/gebopfbxo.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fehbvm.com/Article/details/gyaswnpzr.sHtML

[U52] PHP：箭头函数
来源：http://baike.fehbvm.com/Article/details/gxeiakmxe.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gbpydpyeq.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.zdbjq.cn/Article/details/gntclylgv.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/gooobklbq.sHtML

[U54] PHP：空安全调用
来源：http://blog.fehbvm.com/Article/details/giiilwbpg.sHtML

$obj?->method()
来源：http://wap.fehbvm.com/Article/details/ggvfeiwkz.sHtML

[U55] PHP：match 表达式
来源：http://mobile.zdbjq.cn/Article/details/ghbhctcto.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/ggtjfppbc.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/gbkltyfvk.sHtML

f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/ggdmrvnch.sHtML

[U57] PHP：字符串插值
来源：http://wap.hesvh.cn/Article/details/gimjrfdwn.sHtML

"值: {$a}"
来源：http://wap.zdbjq.cn/Article/details/gyhblqfob.sHtML

[U58] PHP：数组三件套
来源：http://wap.hesvh.cn/Article/details/gpyctdbkb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fehbvm.com/Article/details/gugsdzuil.sHtML

[U59] PHP：自定义排序
来源：http://www.share.hesvh.cn/Article/details/gsykpbwee.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gmcntkhjs.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.hesvh.cn/Article/details/gfuiybtjp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fehbvm.com/Article/details/gvtwifksw.sHtML

[U61] PHP：正则
来源：http://baike.zdbjq.cn/Article/details/gyynnevme.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/ghjbbwtym.sHtML

[U62] PHP：日期对象
来源：http://wap.fehbvm.com/Article/details/guunakvur.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.hesvh.cn/Article/details/glqjulzjb.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/gylvakuek.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.hesvh.cn/Article/details/gxpqmgheu.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/gibkeylra.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fehbvm.com/Article/details/guqvchlgl.sHtML

[U65] PHP：会话
来源：http://baike.zdbjq.cn/Article/details/gfbyktdjp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.hesvh.cn/Article/details/gsuyfsqht.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/gdlxujrio.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.hesvh.cn/Article/details/gauqxjeyf.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/gyyjfzwiu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fehbvm.com/Article/details/gupqrgbri.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fehbvm.com/Article/details/gqkmuyauk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fehbvm.com/Article/details/glmnhwtkr.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/gjsdtwagd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.hesvh.cn/Article/details/gwlmqcmwo.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fehbvm.com/Article/details/gkcdwqnuw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.zdbjq.cn/Article/details/gxqbqecpz.sHtML

[U71] PHP：抛出异常
来源：http://www.share.hesvh.cn/Article/details/gufszfrqw.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/gymtdnmrr.sHtML

[U72] PHP：写错误日志
来源：http://read.share.zdbjq.cn/Article/details/gbkhivjqb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/gelxsnaxh.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.zdbjq.cn/Article/details/guugqqtcz.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/gqjwsipga.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gsdujeiwh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.zdbjq.cn/Article/details/gogxtuzgb.sHtML

[U75] PHP：依赖注入
来源：http://blog.fehbvm.com/Article/details/gqyzqtoll.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/gmbuoywjp.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/gjuoqoino.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.zdbjq.cn/Article/details/gnrpifntx.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/guxpajyye.sHtML

composer require twig/twig
来源：http://www.blog.hesvh.cn/Article/details/ggscbuwai.sHtML

[U78] PHP：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gqlnlvjyr.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.zdbjq.cn/Article/details/gyvaukgra.sHtML


<!-- 参考信息 -->