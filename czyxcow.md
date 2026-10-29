代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/ggdbfwzvx.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/gukrjwova.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/grexxudaf.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/goenaxncw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/glqjjgbde.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gukjijhwn.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gzerbtuvz.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/gmrwxqmme.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gyiabbvwf.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/grnlzysxm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/gmcqkascb.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gxejwtsuu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gzkluxdxz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/garowubne.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gcnthwnqu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjexjdbpt.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gkysxfzfd.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gxduzpesc.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gycnhzfjg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/guurndpeh.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/geupawtik.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gpkasjtds.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/glvkfsekn.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gteefsgsg.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/gbrywryab.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/gjmbmdeks.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gumbobehc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/gesizvtyg.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gecjwriao.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gdjkruqyw.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gsjhvtirs.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/grsiwpbeu.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/gjmcmdnca.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/gvpqzzqlz.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gytyvgsec.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/grigmeckt.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gnvsgfbfg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gfqpzyajs.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gqkwwepag.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/gjlciiork.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gcntusiys.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/grutmlbys.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/gryaguqra.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gntgrquks.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gzghtilrt.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/gqqzzfqck.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/ghleukooi.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gkoorkela.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/gnykbgfgn.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gbponpqqy.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gcnmvukqb.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gvwommard.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gxsnlzpim.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/gnqiavcep.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/gnlcesjta.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/gpmklrvjn.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/gnjgdxgry.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/giaxlowsv.sHtML

[T22] Swift：字典
来源：http://blog.fehbvm.com/Article/details/glkosiezr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/gcgugnlnf.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/gzcuvtmhm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gicjcorto.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/gxbccdflh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gimwguywf.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/ggjqiabyc.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/gmgxgbolw.sHtML

[T26] Swift：类与重写
来源：http://wap.hesvh.cn/Article/details/gzdwlzulu.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gvhcvkwxm.sHtML

[T27] Swift：错误处理
来源：http://blog.zdbjq.cn/Article/details/gbjcxcqra.sHtML

do { try f() } catch { print(error) }
来源：http://3g.zdbjq.cn/Article/details/gpvvjqgfl.sHtML

[T28] Swift：枚举
来源：http://3g.fehbvm.com/Article/details/gazqmdvao.sHtML

enum Color { case red, green }
来源：http://blog.zdbjq.cn/Article/details/gltlejzoq.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/gvxlfmpfi.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/ghehzckds.sHtML

[T30] Swift：协议
来源：http://baike.zdbjq.cn/Article/details/gnjnynewr.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gvthseyrw.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gbhpvbqoy.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gbvetvytj.sHtML

[T32] Lua：局部变量
来源：http://baike.zdbjq.cn/Article/details/gfdbnsaxi.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/ghwizzsxa.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/goshdgkcu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/gcoskprhb.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gvfmvkokt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gfzczfphh.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gnuoftmlu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/gqltuxbke.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/gtzfzpogy.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/gdgcjgbzf.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gexlqqvgc.sHtML

"a" .. "b"
来源：http://3g.hesvh.cn/Article/details/gfoxbibbr.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/gpcbdperx.sHtML

if x > 0 then print("正") end
来源：http://mobile.zdbjq.cn/Article/details/gqjkzdzuw.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gihupyejz.sHtML

string.find(s, "%d+")
来源：http://mobile.fehbvm.com/Article/details/glpgkwlwp.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/gehrsblnc.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fehbvm.com/Article/details/gkbdkbogo.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gnaqqubiu.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/groquwxwi.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/gavtxbljz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/gqsjvernd.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gccypfsra.sHtML

"值: $a"
来源：http://read.share.fehbvm.com/Article/details/gpkyrvqvp.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/gntrsftzo.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.zdbjq.cn/Article/details/gxmprxnfn.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/gyygmscsw.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/gzhdepawu.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/ggitbehbz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvohsduwa.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/ginirnrpg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/gamvlkhyf.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/galheyojd.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/gvwdxfwku.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/gkwoexmix.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gneautmgv.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gvxsivkks.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gxardwcot.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fehbvm.com/Article/details/grrrrmnzd.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gbpsslwbz.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/geymsgwkh.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gtaoaretn.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/gpyzmbwio.sHtML

[T53] Scala：字符串插值
来源：http://wap.fehbvm.com/Article/details/gvcbbtmur.sHtML

s"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gkdoaokco.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gqpoqzstg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gppusvaan.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gglphylsb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/gtdqostkx.sHtML

[T56] Scala：样例类
来源：http://baike.hesvh.cn/Article/details/grkrdpmdy.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gdwkimudo.sHtML

[T57] Scala：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gmoumshio.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.hesvh.cn/Article/details/gplzcwbcx.sHtML

[T58] Scala：函数定义
来源：http://baike.fehbvm.com/Article/details/gcxqqjqni.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/gzotlggka.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gdldwphwo.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/gjlevilmi.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/gkxveisic.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/grxqhxiww.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/goaekhpme.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gmwkszyrk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbvqpyuxl.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fehbvm.com/Article/details/gcvuxqwiv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gcbjpdggo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/gssxhgecd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/gptgnezer.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.zdbjq.cn/Article/details/gsaetsefd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/gtujlvolc.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/gjderjmcl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/gnuliyfxj.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/gmfxhsptj.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gvhndvfzn.sHtML

[U06] Py：合并两个字典
来源：http://www.share.hesvh.cn/Article/details/glfsjtbas.sHtML

{**a, **b}
来源：http://3g.zdbjq.cn/Article/details/gchyukrdo.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fehbvm.com/Article/details/gnhldotpk.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/ghrblbtet.sHtML

[U08] Py：展平二维列表
来源：http://wap.zdbjq.cn/Article/details/gxhkplfem.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/grnzweceu.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fehbvm.com/Article/details/grayzhrrp.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/gtblqkxio.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/gambwjjzw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/geaeblwnd.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/gmomevmtw.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/ggspiknqs.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/gbcpqyacy.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.zdbjq.cn/Article/details/glowbnilz.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/gjeeqqcxg.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/gbeojdrqf.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fehbvm.com/Article/details/guylfxbhr.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/gguuizlqi.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/gbwfvyuea.sHtML

t = time.perf_counter()
来源：http://mobile.zdbjq.cn/Article/details/gwypndedb.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/gsjlawcpg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/gfmgpsdnm.sHtML

[U17] Py：初始化日志
来源：http://mobile.fehbvm.com/Article/details/ghmycmdbk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.zdbjq.cn/Article/details/gjqmfmupb.sHtML

[U18] Py：预编译正则
来源：http://read.share.hesvh.cn/Article/details/gigdvydph.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gpmwgbbyj.sHtML

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/gxyezcmpb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/gszwfmnnr.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fehbvm.com/Article/details/gznypraju.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/gwaefbatc.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fehbvm.com/Article/details/gqnrsgyia.sHtML

@contextlib.contextmanager
来源：http://www.blog.zdbjq.cn/Article/details/gcmzstzhh.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/gkxbnnzhw.sHtML

list(zip(*m))
来源：http://blog.hesvh.cn/Article/details/gzzmqihdl.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fehbvm.com/Article/details/glbycvstt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/gjhuyaiua.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gsbiudopg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/glohmbehu.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.zdbjq.cn/Article/details/gfdzsmqrg.sHtML

csv.DictReader(f)
来源：http://3g.zdbjq.cn/Article/details/gkceolhpd.sHtML

[U26] Py：并发下载
来源：http://blog.hesvh.cn/Article/details/gvzvnudav.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/gshkgikts.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fehbvm.com/Article/details/guzkasxzf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.hesvh.cn/Article/details/gyqfzsnet.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/grdldzbjj.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gfcjltyvu.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fehbvm.com/Article/details/gzsgyxxdf.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/gyonpdzdk.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/gjzftbmzs.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/gqylpujmb.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/glauimeyq.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/ggefcknad.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gklsemtxi.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gokhabctm.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/ggrkzjlff.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fehbvm.com/Article/details/gxletmnqj.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/gdtcqvmes.sHtML

chardet.detect(raw)
来源：http://m.share.fehbvm.com/Article/details/gutulgqdu.sHtML

[U35] Py：发送邮件
来源：http://www.share.hesvh.cn/Article/details/geylyfdux.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fehbvm.com/Article/details/gkeugfhbo.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/gslgdxkni.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fehbvm.com/Article/details/gpxxmisqd.sHtML

[U37] Py：读写 Excel
来源：http://wap.fehbvm.com/Article/details/gyvkxdsbx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fehbvm.com/Article/details/gxddbzbrf.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.hesvh.cn/Article/details/gnhtuldha.sHtML

Path(__file__).resolve().parent
来源：http://read.share.zdbjq.cn/Article/details/gjvxtvnif.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/gzybaquxb.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/gdkmxklcm.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/gvzpuendd.sHtML

print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/giyvousvw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fehbvm.com/Article/details/gmxlmgvdi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.zdbjq.cn/Article/details/gtpioqbyn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fehbvm.com/Article/details/grfvewzcx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/guasanxbm.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fehbvm.com/Article/details/gfczeljsz.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/gfidiipmk.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.hesvh.cn/Article/details/gqeahbriv.sHtML

declare(strict_types=1);
来源：http://www.m.share.hesvh.cn/Article/details/gnvmdkvsr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fehbvm.com/Article/details/gcjgxlpoz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gvrjgqtgw.sHtML

[U46] PHP：可空类型
来源：http://blog.hesvh.cn/Article/details/ggxipkjxd.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/gbngdglxu.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/ghtixrryt.sHtML

int|string $id
来源：http://m.share.hesvh.cn/Article/details/ggdukccki.sHtML

[U48] PHP：纯枚举
来源：http://wap.zdbjq.cn/Article/details/gjoscgmpv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.hesvh.cn/Article/details/ggyhnonvf.sHtML

[U49] PHP：只读属性
来源：http://baike.zdbjq.cn/Article/details/gpkvfstmq.sHtML

public readonly string $name
来源：http://wap.hesvh.cn/Article/details/ggdkuswgo.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.hesvh.cn/Article/details/gnxvhnnib.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fehbvm.com/Article/details/gxbwsmxas.sHtML

[U51] PHP：数组解构
来源：http://read.share.fehbvm.com/Article/details/ggdqtixpz.sHtML

[$a, $b] = $arr;
来源：http://baike.fehbvm.com/Article/details/gvufxxzko.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gxfmcyzuw.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.hesvh.cn/Article/details/gjuajrrqe.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fehbvm.com/Article/details/gqbtuougc.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fehbvm.com/Article/details/gifsrmlgj.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fehbvm.com/Article/details/gokewgvuu.sHtML

$obj?->method()
来源：http://www.m.share.fehbvm.com/Article/details/gegdvxnot.sHtML

[U55] PHP：match 表达式
来源：http://baike.zdbjq.cn/Article/details/gnduwnzqn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/ghmrtfozl.sHtML

[U56] PHP：命名参数
来源：http://www.share.zdbjq.cn/Article/details/gkglwbbyx.sHtML

f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gnjdprzjb.sHtML

[U57] PHP：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gwhrkeusu.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/gkylvmbcc.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fehbvm.com/Article/details/gsmjorlvx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fehbvm.com/Article/details/ghaddmtkk.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.hesvh.cn/Article/details/gufgccwaq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gdshjgzzn.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/gnztxzskn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/gvzdrbmrd.sHtML

[U61] PHP：正则
来源：http://m.share.zdbjq.cn/Article/details/gckfahgcq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gnkwajnan.sHtML

[U62] PHP：日期对象
来源：http://read.share.fehbvm.com/Article/details/gwchbgomx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fehbvm.com/Article/details/gkkzhdjxh.sHtML

[U63] PHP：文件读写
来源：http://mobile.zdbjq.cn/Article/details/gvcmqdiud.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.zdbjq.cn/Article/details/gmodhqskm.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/gitiiccjl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fehbvm.com/Article/details/gziqxtcwq.sHtML

[U65] PHP：会话
来源：http://www.blog.hesvh.cn/Article/details/gzvpaeclv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/ghouswpcx.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.zdbjq.cn/Article/details/ggeebqdxn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fehbvm.com/Article/details/gphenzteb.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fehbvm.com/Article/details/gupeqovsd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.hesvh.cn/Article/details/gnmhldawt.sHtML

[U68] PHP：PDO 连接
来源：http://blog.zdbjq.cn/Article/details/gjfqekoqw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/gqhsppplq.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fehbvm.com/Article/details/gcmnjzpug.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/gbvobpcyr.sHtML

[U70] PHP：PDO 事务
来源：http://blog.hesvh.cn/Article/details/grnhvmkdo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.hesvh.cn/Article/details/gcelytlpa.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fehbvm.com/Article/details/gelkpmdlc.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/ghhtkurpi.sHtML

[U72] PHP：写错误日志
来源：http://wap.fehbvm.com/Article/details/glcqvpusd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/gwqhfhjqk.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.hesvh.cn/Article/details/gdiljnohr.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fehbvm.com/Article/details/gnhjuzaqe.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gtqlbjamq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fehbvm.com/Article/details/gelceejav.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gmvwdhjko.sHtML

composer require psr/container
来源：http://baike.fehbvm.com/Article/details/gdkttinmn.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/gxfjmmacm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.hesvh.cn/Article/details/ghmgktsua.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fehbvm.com/Article/details/glozpxaru.sHtML

composer require twig/twig
来源：http://read.share.zdbjq.cn/Article/details/gcqisufaz.sHtML

[U78] PHP：单元测试
来源：http://baike.hesvh.cn/Article/details/gesnucziy.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.hesvh.cn/Article/details/gedybomks.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/gaciznshx.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.hesvh.cn/Article/details/ghkjyvrbb.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fehbvm.com/Article/details/gvmvorgbl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.zdbjq.cn/Article/details/gdvplnbev.sHtML


<!-- 参考信息 -->