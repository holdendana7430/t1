代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/ghlhvjxmt.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gayhlaeak.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/guqqhbukw.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/gkzgqzlky.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gwwmkfpom.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/grtgppzjx.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gguvdyysy.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gdmxsbooa.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/gbbmkxbje.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/grepzijiq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/gmycyiktb.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gpwydttif.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gnqijuwns.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grwzvapfu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gcejcvrah.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnlbaonwt.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/grkwvujyq.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gnjhffwko.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gjlrwlkos.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gsdeozktd.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/ghrafxjlf.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gssirbwax.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/grkjsrtdv.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/gikmhvmgw.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gfquniqsa.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gaflifxmf.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gqmlqqptp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.hesvh.cn/Article/details/gldvklpjx.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gxzpiovsn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/gftxldzvx.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/ghkjmkmgx.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/guhgrtgbi.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/gihmqsfmk.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/grbgtnffh.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gwvvhjfnr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gqhiiashv.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/ggfkhpxes.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gmjwlgqjc.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/gvmpqugpw.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gqkckvpfx.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/goonojlhv.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/gbcwoqyes.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/gagtgwhke.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gpjtuywdl.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/gezdzvtug.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fehbvm.com/Article/details/gacwtsjpy.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gdyhfvbxm.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gprsvxwzs.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gulzsgpvw.sHtML

var a = 1;  let b = 2
来源：http://read.share.fehbvm.com/Article/details/gvtguwvoy.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gkfhsqrki.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/gqlzphjdf.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/gocaeyphe.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gyjbsfcjo.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/gnphztrws.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/gfskhrynl.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/genffybvk.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/gwxmeermi.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/glfnrjluw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gmaxnhdah.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/ghgqtwlsh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/gsjnfuavv.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/ghjaigchj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gnowgalyi.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/gbrsiiulb.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gxoaaeqsh.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/gonrusxtp.sHtML

class A: Base { override func f() {} }
来源：http://read.share.hesvh.cn/Article/details/gbwsacdec.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/gmgzfconf.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/gdvhnxzfk.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gyxklajsh.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/gqayzwmcj.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/gkumbxxht.sHtML

guard let x = opt else { return }
来源：http://3g.fehbvm.com/Article/details/gkvstfgsi.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/gwfxxxgim.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/gymyrxtda.sHtML

[T31] Lua：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gurhvytnh.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gqrbrtewh.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/gqkwaoltp.sHtML

local a = 1
来源：http://wap.hesvh.cn/Article/details/getyleukb.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/grsihqeqt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fehbvm.com/Article/details/gqlqkwjlc.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/gbnplqpgp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gzprmdgxb.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gxiapsynl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gjjdzjmka.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/ggtwrwngp.sHtML

function add(a, b) return a + b end
来源：http://m.share.zdbjq.cn/Article/details/ggjwzlqci.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gfjwhbrab.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/guheaomaj.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/gewpknkje.sHtML

if x > 0 then print("正") end
来源：http://baike.hesvh.cn/Article/details/ggfklyevw.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gqpqoctql.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/gzpuhohtv.sHtML

[T40] Lua：元表
来源：http://wap.hesvh.cn/Article/details/gfdlnmdao.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/gbavsvski.sHtML

[T41] Perl：Hello World
来源：http://www.share.fehbvm.com/Article/details/gyujnyfvt.sHtML

print "Hello\n";
来源：http://baike.hesvh.cn/Article/details/ghbihmvyt.sHtML

[T42] Perl：变量类型
来源：http://read.share.hesvh.cn/Article/details/gqhpdtcmu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gacfycvgo.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gvdqvjssv.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/gntmqhbaj.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/gitfvvggu.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fehbvm.com/Article/details/gjkizjcth.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/gddfavebl.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/gopprwufh.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/gthbinvsb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/ganwmjzrp.sHtML

[T47] Perl：正则捕获
来源：http://baike.hesvh.cn/Article/details/gnrjbxerf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/gkyxbvwoi.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/gnqzcjpqb.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/gvqwezauo.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gskrdmfxc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gccvxytee.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gcseqjtzc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.hesvh.cn/Article/details/gxmvpakgz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/gjqqfmnjk.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gxvdqaxcb.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gvwnifzik.sHtML

[T52] Scala：变量
来源：http://baike.zdbjq.cn/Article/details/gvkajzhdb.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/grgdaktey.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gcwnipent.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gsxktcfqf.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/ghbjtqota.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fehbvm.com/Article/details/gjitilhkc.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/grikgvyzs.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fehbvm.com/Article/details/gspcpsfsi.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gnvhjjhpd.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gdrkcvidt.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/gcywvsryo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gmbtcujmo.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/ghlkdknir.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.hesvh.cn/Article/details/ghwpsvrzd.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/gndsqmwio.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gbukdvoyi.sHtML

[T60] Scala：折叠
来源：http://3g.hesvh.cn/Article/details/gskgsznmp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.zdbjq.cn/Article/details/gewmtisiz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gimeymtqz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gkdcgxcuw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbowjtdoq.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/gaztsxwfv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/gyoqrpknn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fehbvm.com/Article/details/gpmpvnzia.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/gqbgotyph.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fehbvm.com/Article/details/gmtdbzcvb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.hesvh.cn/Article/details/gvyuoclvc.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/gxoeyssto.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.zdbjq.cn/Article/details/gqqfpmgiq.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.zdbjq.cn/Article/details/gkzlncmqn.sHtML

list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gtginypcm.sHtML

[U06] Py：合并两个字典
来源：http://read.share.zdbjq.cn/Article/details/gxuieowne.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/gasqtvlhi.sHtML

[U07] Py：反转字典键值
来源：http://m.share.hesvh.cn/Article/details/guoylkeqh.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gzrabtyxp.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/gmibpgcbr.sHtML

[y for x in nested for y in x]
来源：http://read.share.fehbvm.com/Article/details/gobpnljwn.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fehbvm.com/Article/details/gssehxsmk.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/ghxeeklsq.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gbuzajlya.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/gsvxoatyb.sHtML

[U11] Py：生成器表达式
来源：http://blog.fehbvm.com/Article/details/gtpitinwk.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/gbvecdetr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/gsdkgpman.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/gtetedkce.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/gieoebyeg.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/gcemthfzg.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.hesvh.cn/Article/details/ggaaxrzba.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gfodbfyem.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/gxqsawbnj.sHtML

t = time.perf_counter()
来源：http://www.m.share.fehbvm.com/Article/details/gzvjkhxzq.sHtML

[U16] Py：命令行参数解析
来源：http://3g.hesvh.cn/Article/details/grsylyfcq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.zdbjq.cn/Article/details/gmhcwgvss.sHtML

[U17] Py：初始化日志
来源：http://wap.hesvh.cn/Article/details/gqmutnwpj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.hesvh.cn/Article/details/gscwaksji.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/ghpeclmhj.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gdzggkoku.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.hesvh.cn/Article/details/ghfxmyykn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/gnqqsrvyy.sHtML

[U20] Py：缓存函数结果
来源：http://wap.zdbjq.cn/Article/details/gjzgjzknr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.hesvh.cn/Article/details/gftromyqf.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/gnktiwtbj.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/gnqrqsxsv.sHtML

[U22] Py：矩阵转置
来源：http://mobile.zdbjq.cn/Article/details/gboiavmqj.sHtML

list(zip(*m))
来源：http://www.share.hesvh.cn/Article/details/gwvdsgdtq.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/gwcflujrg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.zdbjq.cn/Article/details/gagqllnmr.sHtML

[U24] Py：路径操作
来源：http://www.m.share.hesvh.cn/Article/details/gbjgxshdi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gcajbbxdq.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fehbvm.com/Article/details/gjjlcjstx.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/goddvdjww.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/gdknghjsy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.hesvh.cn/Article/details/gqfskxhhl.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.zdbjq.cn/Article/details/gseicocso.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.zdbjq.cn/Article/details/gzqyeaxmz.sHtML

[U28] Py：类型别名
来源：http://www.blog.zdbjq.cn/Article/details/gzrstejfa.sHtML

UserId = int
来源：http://wap.fehbvm.com/Article/details/gkxtdpfva.sHtML

[U29] Py：属性校验
来源：http://www.m.share.zdbjq.cn/Article/details/gzkpwxade.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/gwthzmwvr.sHtML

[U30] Py：数据类
来源：http://read.share.zdbjq.cn/Article/details/giwgycekh.sHtML

@dataclass(slots=True)
来源：http://3g.zdbjq.cn/Article/details/gygwaogwn.sHtML

[U31] Py：单测
来源：http://baike.fehbvm.com/Article/details/gfuhtzrnq.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/ghhpmqaif.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.hesvh.cn/Article/details/gvfsbqhkg.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gluasyuxa.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/gfzatxqof.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.zdbjq.cn/Article/details/gvydrgnbm.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/gfkuxopcj.sHtML

chardet.detect(raw)
来源：http://www.blog.fehbvm.com/Article/details/gujutbgdz.sHtML

[U35] Py：发送邮件
来源：http://blog.hesvh.cn/Article/details/givxesonw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.zdbjq.cn/Article/details/gxroimdus.sHtML

[U36] Py：定时任务
来源：http://www.share.zdbjq.cn/Article/details/gnjstqayl.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.hesvh.cn/Article/details/gjkkltzhm.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fehbvm.com/Article/details/gcygfmgsa.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.hesvh.cn/Article/details/gltvczwme.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/gnlrvkfqy.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/gcvulwmyz.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.zdbjq.cn/Article/details/gbqrdihjb.sHtML

sys.stdout.isatty()
来源：http://www.blog.zdbjq.cn/Article/details/gqunvnmgt.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/gefxdeqqq.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gqfzhyyeu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.hesvh.cn/Article/details/gvvgofvsp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gdbkqjxas.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.zdbjq.cn/Article/details/gykelttxl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.hesvh.cn/Article/details/gurbbwzpw.sHtML

[U43] PHP：声明命名空间
来源：http://3g.hesvh.cn/Article/details/gpjtukesb.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/ggcjshnph.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fehbvm.com/Article/details/gvgodknkg.sHtML

declare(strict_types=1);
来源：http://m.share.fehbvm.com/Article/details/gjcnsjixh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.hesvh.cn/Article/details/gaacdpahg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gzqqixzrd.sHtML

[U46] PHP：可空类型
来源：http://read.share.fehbvm.com/Article/details/gffvivzxt.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/gtxohspln.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/gjjmfxkvr.sHtML

int|string $id
来源：http://read.share.zdbjq.cn/Article/details/gatughksz.sHtML

[U48] PHP：纯枚举
来源：http://wap.fehbvm.com/Article/details/gezpatkqf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyyllpbgv.sHtML

[U49] PHP：只读属性
来源：http://3g.fehbvm.com/Article/details/goiwzlyhv.sHtML

public readonly string $name
来源：http://mobile.hesvh.cn/Article/details/gchebissf.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.zdbjq.cn/Article/details/ggekzhyru.sHtML

public function __construct(private int $id) {}
来源：http://m.share.zdbjq.cn/Article/details/gwtwantyn.sHtML

[U51] PHP：数组解构
来源：http://baike.zdbjq.cn/Article/details/gfslcrkxz.sHtML

[$a, $b] = $arr;
来源：http://baike.hesvh.cn/Article/details/gilklubob.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gnyaarygi.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/galvqjmmz.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/gtknaedby.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/gfkievtqy.sHtML

[U54] PHP：空安全调用
来源：http://baike.zdbjq.cn/Article/details/gneaxjciw.sHtML

$obj?->method()
来源：http://read.share.hesvh.cn/Article/details/gtmyxuwbk.sHtML

[U55] PHP：match 表达式
来源：http://blog.zdbjq.cn/Article/details/gebfrronm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gvrsdthhr.sHtML

[U56] PHP：命名参数
来源：http://www.share.hesvh.cn/Article/details/grzsldddp.sHtML

f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/ginlkwgzu.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gzgeolbso.sHtML

"值: {$a}"
来源：http://blog.zdbjq.cn/Article/details/ghsjihbnv.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fehbvm.com/Article/details/gheealird.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gxosvxkaf.sHtML

[U59] PHP：自定义排序
来源：http://read.share.zdbjq.cn/Article/details/gxqfuzann.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gcnolnwmz.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fehbvm.com/Article/details/gjzfubmyw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fehbvm.com/Article/details/gbgfitqhp.sHtML

[U61] PHP：正则
来源：http://www.blog.hesvh.cn/Article/details/glxamnyfs.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gmfvcjklc.sHtML

[U62] PHP：日期对象
来源：http://blog.fehbvm.com/Article/details/gfvjmlccp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fehbvm.com/Article/details/gyontuybt.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/gyoimxpsw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fehbvm.com/Article/details/gtfcovrrn.sHtML

[U64] PHP：目录遍历
来源：http://wap.zdbjq.cn/Article/details/gwokvltyo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fehbvm.com/Article/details/gaabpbajp.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/gztbhtplq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gppgqzdrx.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/gnwlmzzfy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fehbvm.com/Article/details/gurtiwqcj.sHtML

[U67] PHP：处理文件上传
来源：http://baike.zdbjq.cn/Article/details/gyuaiicbi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.hesvh.cn/Article/details/geltlzuou.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/gdhpqutou.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/gmwzzcoih.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.zdbjq.cn/Article/details/gmquxewpd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.zdbjq.cn/Article/details/gsrllywry.sHtML

[U70] PHP：PDO 事务
来源：http://baike.zdbjq.cn/Article/details/gyivzcbpl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.hesvh.cn/Article/details/gqxrvksjb.sHtML

[U71] PHP：抛出异常
来源：http://www.share.hesvh.cn/Article/details/gbzjzpxze.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fehbvm.com/Article/details/gimlkqplg.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.zdbjq.cn/Article/details/gdxuamyjg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.zdbjq.cn/Article/details/gsqulieky.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/ghpfuiyrq.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fehbvm.com/Article/details/gzzxanmeu.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/giyunbwen.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.zdbjq.cn/Article/details/gukalmbxu.sHtML

[U75] PHP：依赖注入
来源：http://wap.zdbjq.cn/Article/details/gdyziusoz.sHtML

composer require psr/container
来源：http://baike.fehbvm.com/Article/details/gblcnimoy.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fehbvm.com/Article/details/geoyzfnak.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fehbvm.com/Article/details/gsfuyaizm.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/ghdkffols.sHtML

composer require twig/twig
来源：http://www.share.zdbjq.cn/Article/details/ghbayqozo.sHtML

[U78] PHP：单元测试
来源：http://wap.hesvh.cn/Article/details/grcljkqnl.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.zdbjq.cn/Article/details/gkapjdcoz.sHtML

[U79] PHP：静态分析
来源：http://baike.hesvh.cn/Article/details/grdqmconr.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.hesvh.cn/Article/details/gwvqzzedo.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fehbvm.com/Article/details/gljeflltc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/gtnpmqfwv.sHtML


<!-- 参考信息 -->