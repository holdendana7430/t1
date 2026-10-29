代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gxzlltfkb.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/gxzziviln.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gpruhqhji.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/girqtaufk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gsyafravm.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/geiwonnjm.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gltczsfvn.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/ggklujill.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gfdexpewf.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/gtdoawufo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/gvlhnacjs.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gcylhdcas.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gihxisyey.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ganlcrvqa.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gyoruqjwp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvpevjwwa.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gjfdntjgk.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gfcsaxsgs.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gdykzadbi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/ghazccier.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/gcsixnpvy.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gmffzeery.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/ghbhxeojh.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gzeznvpkt.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gecrwdlyp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gnpwkozgz.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/goyssfyrv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/ggniaqrys.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gvoefhmrc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gmgacjtmg.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/glaofpccd.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.zdbjq.cn/Article/details/gmkdwmgpz.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/gqaeetiqj.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gfbtzuheo.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/gdtgchniz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gkwfrxsul.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gusyzfbsy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/ghcbjvgbi.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gslqaozwi.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/gdocqbmvu.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/gausanrgw.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/gonguaivh.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gjpchihlv.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gvpxddayx.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gtswdkira.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/gawgchbeq.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/gphcstbmx.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gzfplvhsm.sHtML

[T17] Swift：变量与常量
来源：http://3g.zdbjq.cn/Article/details/guvoqwjxx.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gmqzcaqjn.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gxxfgpmun.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/gvzweusgv.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/gaqfrvkbu.sHtML

if let n = opt { print(n) }
来源：http://3g.fehbvm.com/Article/details/guagcnzii.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/gwdjlflub.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/gxumfadln.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/gomlqkxaz.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/gzvhgsobv.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gszhqtbek.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gfedezmjb.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/ghenjkkkv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/ggcetvmxw.sHtML

[T24] Swift：闭包
来源：http://www.blog.fehbvm.com/Article/details/ghlicpadc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/ggolvsmyy.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/gxolefpjt.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gnilbwdvl.sHtML

[T26] Swift：类与重写
来源：http://3g.hesvh.cn/Article/details/gpakkjgwn.sHtML

class A: Base { override func f() {} }
来源：http://www.share.zdbjq.cn/Article/details/giwxjqkij.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gbpvimnyx.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/gehkhpuwc.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gumxjjlaa.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/gyhbaomyz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/godarlkwl.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gafrllguj.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gxluruuhl.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/gfvnartmg.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gopusnwzm.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gizlncrju.sHtML

[T32] Lua：局部变量
来源：http://3g.hesvh.cn/Article/details/gvgmeewri.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gtxhwysri.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/geqsytesv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/gijkrethw.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gyxruobsv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/gyqablviv.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/gkyzdpvta.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gmewsravh.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gtrkipikg.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/gmqpaipbw.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gstnzhtdd.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/glwpmlrud.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/gagnabswm.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gsldmpbsi.sHtML

[T39] Lua：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/glknfpulc.sHtML

string.find(s, "%d+")
来源：http://wap.hesvh.cn/Article/details/gjqivqjnq.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/gxkizbrgf.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.hesvh.cn/Article/details/gdtfgjglw.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gunitqjeb.sHtML

print "Hello\n";
来源：http://www.blog.hesvh.cn/Article/details/gxdepwnpg.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gibtgeilh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.zdbjq.cn/Article/details/gzwxdneww.sHtML

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gthkhrjme.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/glompwjmw.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/goelmtqhx.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/gwsrddopt.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/glvpavlyo.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/gsvfmmlch.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gqprrfqlo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fehbvm.com/Article/details/gdhxepbgr.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/ganzfwhys.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtzjtgblz.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/gmfiqwspo.sHtML

$s =~ s/old/new/g;
来源：http://baike.fehbvm.com/Article/details/gbftinjzk.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/gfunfssqt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gnszrxsrc.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/glmsemdsz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.hesvh.cn/Article/details/gyitaufck.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/gqyomuefa.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/gjnxwtvxk.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gkxgdudnb.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gpkaqmaiq.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/gcgshnvaq.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gsuacrars.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gnaplhhmh.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/gxvprwvmy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.hesvh.cn/Article/details/gobeagdja.sHtML

[T55] Scala：集合过滤
来源：http://3g.fehbvm.com/Article/details/gruegyxhc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gbecqvrdz.sHtML

[T56] Scala：样例类
来源：http://read.share.hesvh.cn/Article/details/gujkkdtkp.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/glpvgnjig.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gkrdrltth.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/gvisfwdos.sHtML

[T58] Scala：函数定义
来源：http://wap.zdbjq.cn/Article/details/gwlvqhwjs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fehbvm.com/Article/details/gvyizufje.sHtML

[T59] Scala：循环
来源：http://www.m.share.hesvh.cn/Article/details/ghfvzkdyq.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gzfhtmqja.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/gltmdwlqk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/gdcjsvwdd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbwboauxp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gskxlfpkw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmhwkgdum.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/gczvfarcb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/gisdhjtol.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/gsddxetvf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.hesvh.cn/Article/details/ggukwzior.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/gomyodbxg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/gkenaccxx.sHtML

[U04] Py：变量调试打印
来源：http://www.share.hesvh.cn/Article/details/gfgskjnwl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/gqavqhqbk.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.hesvh.cn/Article/details/gmhhdajbn.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gjahrwkxp.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gzwlcurmc.sHtML

{**a, **b}
来源：http://baike.hesvh.cn/Article/details/gwbndhekn.sHtML

[U07] Py：反转字典键值
来源：http://mobile.zdbjq.cn/Article/details/gwlpdiwfd.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/gkcepdqlg.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fehbvm.com/Article/details/ghcjnvzob.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/gujmdqmem.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.zdbjq.cn/Article/details/gtwwocwgc.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gcmgormov.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gmyecrzgg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.hesvh.cn/Article/details/gnkqczxfh.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/gdgldlzef.sHtML

(x * 2 for x in arr)
来源：http://3g.fehbvm.com/Article/details/gvavsvwjb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/gknmqerhc.sHtML

Counter(arr).most_common(3)
来源：http://blog.zdbjq.cn/Article/details/ghmaienef.sHtML

[U13] Py：固定长度队列
来源：http://blog.fehbvm.com/Article/details/gxrlhcact.sHtML

deque(maxlen=10)
来源：http://www.m.share.zdbjq.cn/Article/details/gxkyesztc.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/gxisgmvvj.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gbzmmqdgr.sHtML

[U15] Py：高精度计时
来源：http://read.share.hesvh.cn/Article/details/gcoyfgjii.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/gzwnuwphh.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fehbvm.com/Article/details/gvbvhjbeu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/gdfwtoymu.sHtML

[U17] Py：初始化日志
来源：http://mobile.fehbvm.com/Article/details/grxxjatnr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.zdbjq.cn/Article/details/grludofcf.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/gbtsksxzf.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gblqyyngl.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.zdbjq.cn/Article/details/gozzvblqp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/gcsudeajd.sHtML

[U20] Py：缓存函数结果
来源：http://blog.zdbjq.cn/Article/details/geqmphbqx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.zdbjq.cn/Article/details/gjwxnhkov.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.hesvh.cn/Article/details/gsvjzewio.sHtML

@contextlib.contextmanager
来源：http://www.share.hesvh.cn/Article/details/gujbwnvxy.sHtML

[U22] Py：矩阵转置
来源：http://blog.zdbjq.cn/Article/details/gxuxjrshb.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/gwaftczcs.sHtML

[U23] Py：分块读取大文件
来源：http://baike.zdbjq.cn/Article/details/gewzgrwdk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/gnclohnxl.sHtML

[U24] Py：路径操作
来源：http://www.m.share.zdbjq.cn/Article/details/gbobkhvxo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gtwhaoelc.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.hesvh.cn/Article/details/gmbtcupml.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/gshakqsmq.sHtML

[U26] Py：并发下载
来源：http://3g.fehbvm.com/Article/details/gqdawkrsf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fehbvm.com/Article/details/gemaiuitl.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/gflubbbkj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/ggsklgujf.sHtML

[U28] Py：类型别名
来源：http://www.m.share.hesvh.cn/Article/details/grmxqfdna.sHtML

UserId = int
来源：http://m.share.fehbvm.com/Article/details/gfvubgslh.sHtML

[U29] Py：属性校验
来源：http://blog.hesvh.cn/Article/details/guqykkzer.sHtML

@property 与 @x.setter 配合
来源：http://blog.zdbjq.cn/Article/details/grjwrqdgo.sHtML

[U30] Py：数据类
来源：http://blog.hesvh.cn/Article/details/gtwcsviqf.sHtML

@dataclass(slots=True)
来源：http://blog.fehbvm.com/Article/details/gnhasxqcu.sHtML

[U31] Py：单测
来源：http://read.share.hesvh.cn/Article/details/glwvdbxuz.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/gtljwquac.sHtML

[U32] Py：代码格式化
来源：http://wap.fehbvm.com/Article/details/gxnnxiwpm.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.zdbjq.cn/Article/details/gjsoxcsca.sHtML

[U33] Py：打包发布
来源：http://www.blog.zdbjq.cn/Article/details/gemblmjoe.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fehbvm.com/Article/details/gejylisxz.sHtML

[U34] Py：判断编码
来源：http://m.share.zdbjq.cn/Article/details/gjqsrobiv.sHtML

chardet.detect(raw)
来源：http://wap.fehbvm.com/Article/details/gxoobcuzx.sHtML

[U35] Py：发送邮件
来源：http://m.share.zdbjq.cn/Article/details/gzerehgwc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.hesvh.cn/Article/details/ghttpqhun.sHtML

[U36] Py：定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gjwkuhoae.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/gsfbtfpdx.sHtML

[U37] Py：读写 Excel
来源：http://read.share.hesvh.cn/Article/details/gqmomifmp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/gwztwpbat.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.hesvh.cn/Article/details/ghihbycui.sHtML

Path(__file__).resolve().parent
来源：http://wap.fehbvm.com/Article/details/grgdlfslk.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/goodocaoz.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/guoojzqyp.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fehbvm.com/Article/details/gifdfgzfj.sHtML

print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gqewbgebj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/gcdgjzhhx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gdjdwzvor.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.hesvh.cn/Article/details/gvgpzpiaq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fehbvm.com/Article/details/gbyntapfb.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fehbvm.com/Article/details/gonpnybdg.sHtML

namespace App\Http;
来源：http://wap.hesvh.cn/Article/details/gpietiluq.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/gcpjstwzz.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/gqegcudyw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/gmjwhrfhe.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/ggkfulqnx.sHtML

[U46] PHP：可空类型
来源：http://mobile.hesvh.cn/Article/details/gtahwdgvz.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/grxtemxcy.sHtML

[U47] PHP：联合类型
来源：http://3g.fehbvm.com/Article/details/gfvmopssa.sHtML

int|string $id
来源：http://www.blog.fehbvm.com/Article/details/gyegtnbil.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fehbvm.com/Article/details/gganydulv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.hesvh.cn/Article/details/gjcmcsxgh.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/ggwxdrgiw.sHtML

public readonly string $name
来源：http://m.share.zdbjq.cn/Article/details/ggrevomak.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/ghepkhmqn.sHtML

public function __construct(private int $id) {}
来源：http://blog.zdbjq.cn/Article/details/gfqgmrblf.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.hesvh.cn/Article/details/grdwjdwga.sHtML

[$a, $b] = $arr;
来源：http://mobile.hesvh.cn/Article/details/gkudtusgp.sHtML

[U52] PHP：箭头函数
来源：http://baike.zdbjq.cn/Article/details/goesybkwu.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gxezmefgq.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/gzqojyqyx.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/gcvipfnbx.sHtML

[U54] PHP：空安全调用
来源：http://blog.fehbvm.com/Article/details/gejgutnqm.sHtML

$obj?->method()
来源：http://3g.hesvh.cn/Article/details/glzvyuiqa.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/grriohhug.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.hesvh.cn/Article/details/gciqidwfp.sHtML

[U56] PHP：命名参数
来源：http://m.share.hesvh.cn/Article/details/goftovxbt.sHtML

f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gmybyavxw.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gnrofzwfc.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/gxwlpmnft.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fehbvm.com/Article/details/gaqliuooz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gzthdgpdj.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/gchwysxiw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gvytktuax.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/gpoauioxs.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.zdbjq.cn/Article/details/gqfpsilkn.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/gtrdjqxnq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gstooifqt.sHtML

[U62] PHP：日期对象
来源：http://3g.hesvh.cn/Article/details/gdjawfoft.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.zdbjq.cn/Article/details/gkxrmdbqt.sHtML

[U63] PHP：文件读写
来源：http://baike.hesvh.cn/Article/details/gwaclackv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.hesvh.cn/Article/details/gamaunzjz.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/gmkglowvi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.hesvh.cn/Article/details/gkxeekcul.sHtML

[U65] PHP：会话
来源：http://www.share.hesvh.cn/Article/details/gfrzhgoct.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gwmgtbjhn.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.hesvh.cn/Article/details/golgxdalb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fehbvm.com/Article/details/gogjlnhdt.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.hesvh.cn/Article/details/gqnrdmtdh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fehbvm.com/Article/details/gwrocjify.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fehbvm.com/Article/details/gzypnrhpl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.zdbjq.cn/Article/details/gkfvkgzgo.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.hesvh.cn/Article/details/gbzmsdxet.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fehbvm.com/Article/details/gzigxbuof.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fehbvm.com/Article/details/gnuatowoo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.hesvh.cn/Article/details/glyveqvjp.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/gwlupdonz.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/gyzfldfme.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fehbvm.com/Article/details/gianfukfd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/gnpeafbyy.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.zdbjq.cn/Article/details/ghktkcddq.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.hesvh.cn/Article/details/gujavlegu.sHtML

[U74] PHP：读取环境变量
来源：http://baike.zdbjq.cn/Article/details/ghbjyzfdo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/gxmsdptim.sHtML

[U75] PHP：依赖注入
来源：http://www.share.hesvh.cn/Article/details/gdcicjxbs.sHtML

composer require psr/container
来源：http://wap.zdbjq.cn/Article/details/gushpckll.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fehbvm.com/Article/details/gihnkltyj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.zdbjq.cn/Article/details/gessikfwc.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.zdbjq.cn/Article/details/gdkkovyoq.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/ghulppndg.sHtML

[U78] PHP：单元测试
来源：http://blog.zdbjq.cn/Article/details/ghnebcsdu.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.hesvh.cn/Article/details/guokklrqx.sHtML

[U79] PHP：静态分析
来源：http://3g.zdbjq.cn/Article/details/grmbncfea.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.hesvh.cn/Article/details/gmcxthrbc.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.hesvh.cn/Article/details/glgpsnlkj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/gstilmahh.sHtML


<!-- 参考信息 -->