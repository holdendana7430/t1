代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gwpjvijcm.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/grbclqcnm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/gxncaaode.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gkaisnwno.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fehbvm.com/Article/details/gydnjrwwd.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gbsxtbnms.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/gedrpiiwn.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gmrpquazx.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/ghbbzgqkb.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/glusdisfz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/glhioysva.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gfzdxgwuq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gwdbrokkk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcjvbbkmb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gzngzrhrx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfwlcirrn.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gxceyaauz.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gbtlncvxb.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/gcfjqsckk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gwsdopksp.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/grvqbjcvq.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/ghqohlpzm.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/grhdrchuz.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gaxizgmql.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gcrxwxahp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/ghknliqex.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/gqusaqsaj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gwrqxbduq.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gmvkiskdg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gqvgpkqur.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gntmeajfw.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gofgffurn.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/gvypulcly.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/gxgoukdma.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/gywosgvnf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/glqttsvfe.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gsajvpfjo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gehuyelcq.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/gmcisuhbo.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gdssqhsrd.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gqghrujte.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/gpslzmbqp.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gwhrbbzgk.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gqxyrezww.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/gudvsomvw.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/gchhgtsto.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/gotjnwzyq.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gxiisevai.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/gxiqguctx.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/ggshivjpm.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/gdgehehtn.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gkliaeszf.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/grgsnlxaf.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/ghvqazwvb.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gzqmsteou.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/grtxxshcq.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gyktncwpx.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/gzbhxtktr.sHtML

[T22] Swift：字典
来源：http://m.share.zdbjq.cn/Article/details/gyplybkuf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/grqsmivyg.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/ggmcwgrbn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gisbwhgep.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gsirpbohg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gqajlnqkj.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/gxhihvztl.sHtML

struct P { var x: Int }
来源：http://mobile.hesvh.cn/Article/details/gwwgnoahv.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/gbdfefxpj.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.hesvh.cn/Article/details/gwotaqgka.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/geaiuztms.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/gzsjwedrx.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gvwxmimed.sHtML

enum Color { case red, green }
来源：http://www.share.fehbvm.com/Article/details/ghjgmstum.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/gyjtvkekx.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/ggvzwkwzf.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/gykxsepbv.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/ghgcqvcco.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/gewsvbevh.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gptszbhmk.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gzcbfggpg.sHtML

local a = 1
来源：http://3g.zdbjq.cn/Article/details/ginbwhyxw.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/gnemgbalu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/geivnuftw.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/gtgdkrwdo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/gctbsrktr.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/gavxmiuxh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gufikwxxr.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gbtvanjlv.sHtML

function add(a, b) return a + b end
来源：http://baike.zdbjq.cn/Article/details/gtzbsifkl.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fehbvm.com/Article/details/gqwhxmhri.sHtML

"a" .. "b"
来源：http://3g.hesvh.cn/Article/details/geimvapai.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/gldzgpavf.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/gpouhcbdf.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/gtcyevejz.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gzmrkvftx.sHtML

[T40] Lua：元表
来源：http://wap.hesvh.cn/Article/details/glgxnrpdr.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/gxhvysqza.sHtML

[T41] Perl：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gtfupvehj.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/gzmdhvskl.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/gzlptosxd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/gacudnqsu.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gxxrlzvpf.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/gmjiyntvl.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/gbjjbfcdl.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gnuuadjwo.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/gjurzjanq.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.zdbjq.cn/Article/details/gbbnwhtlo.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gpgppfhxm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/guipiktxw.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fehbvm.com/Article/details/gsnfutpkf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fehbvm.com/Article/details/gdfksayxs.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/grzfajqlc.sHtML

$s =~ s/old/new/g;
来源：http://www.share.hesvh.cn/Article/details/gzefjsufe.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/gywvfjzbl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gqpytttud.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gbqhjcxxc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.hesvh.cn/Article/details/gevoojkgt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fehbvm.com/Article/details/gnjgzrfoq.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gtdmecorj.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/grrptuswh.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/ggduheaaq.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/gqtwnriiw.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gifxdkxba.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gnjbkvzkx.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/gmbhiarvs.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fehbvm.com/Article/details/gbrijdheb.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gnxceuicb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gjmhvangk.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/gxqwkznqn.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gnzxzomyj.sHtML

[T57] Scala：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gyrhplrof.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/gievwophw.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gulqgezol.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gxhrgwlaf.sHtML

[T59] Scala：循环
来源：http://blog.fehbvm.com/Article/details/gtwfheiwu.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gqynqsqmn.sHtML

[T60] Scala：折叠
来源：http://www.share.zdbjq.cn/Article/details/gbrbqlgpo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fehbvm.com/Article/details/ggjrcgiab.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmenhaopk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gxslfuagw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/guwckqegd.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/gskbrsclw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/ggajxbbtw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.zdbjq.cn/Article/details/gnxxunkmo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/gimlsnrmc.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fehbvm.com/Article/details/gwebevvpb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.hesvh.cn/Article/details/gjtbgrcjc.sHtML

[U04] Py：变量调试打印
来源：http://www.share.hesvh.cn/Article/details/gqrbynsln.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/gqrhprxal.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/gnzhpfqzg.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gerqgxgym.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/gpgacbvhj.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gqauzgvil.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/gdpefnsgg.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/gchorjiie.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/ggvejrgps.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/goqumpfmb.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/gzudtsvms.sHtML

max(d, key=d.get)
来源：http://mobile.zdbjq.cn/Article/details/gbviqjygm.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/gjflmwvcm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/gthaelizo.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/grsvnitub.sHtML

(x * 2 for x in arr)
来源：http://3g.zdbjq.cn/Article/details/gwwqprdan.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/gysonvegg.sHtML

Counter(arr).most_common(3)
来源：http://mobile.hesvh.cn/Article/details/grmcqsdbi.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.zdbjq.cn/Article/details/gvoegqhof.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/gtyepqvra.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/gckmgbmvh.sHtML

defaultdict(list)
来源：http://m.share.fehbvm.com/Article/details/gebpxqtyl.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/grsysbyse.sHtML

t = time.perf_counter()
来源：http://baike.fehbvm.com/Article/details/gbuqpcqkm.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.zdbjq.cn/Article/details/ghqczamnr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/gejzkgpuw.sHtML

[U17] Py：初始化日志
来源：http://read.share.fehbvm.com/Article/details/gvtvhzjzm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.zdbjq.cn/Article/details/godjvsriu.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/govuzuuff.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.hesvh.cn/Article/details/goypsootv.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/gbdpjbxsr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/gxdndtgpp.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fehbvm.com/Article/details/gavwduqko.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/gbdtricpn.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/gcgawtzco.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/gclqehltf.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/gzlaschsh.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/gxxfmchaa.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/gfbnpkwye.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.zdbjq.cn/Article/details/gpvxvlnfe.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/gnrrudgiv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/galpqmown.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fehbvm.com/Article/details/gcwaumpwo.sHtML

csv.DictReader(f)
来源：http://read.share.hesvh.cn/Article/details/gmkfvtlsr.sHtML

[U26] Py：并发下载
来源：http://blog.hesvh.cn/Article/details/gammslpve.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fehbvm.com/Article/details/galtujuxp.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/grckclewo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/gfjvnbhvz.sHtML

[U28] Py：类型别名
来源：http://read.share.zdbjq.cn/Article/details/guqrzixgn.sHtML

UserId = int
来源：http://wap.zdbjq.cn/Article/details/gggtyirqp.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/goeoxsibx.sHtML

@property 与 @x.setter 配合
来源：http://wap.zdbjq.cn/Article/details/gemjdpbmx.sHtML

[U30] Py：数据类
来源：http://wap.zdbjq.cn/Article/details/ggrnyfrow.sHtML

@dataclass(slots=True)
来源：http://read.share.hesvh.cn/Article/details/gtiopplun.sHtML

[U31] Py：单测
来源：http://baike.fehbvm.com/Article/details/gauobpzpo.sHtML

python -m pytest -q
来源：http://wap.fehbvm.com/Article/details/getwdtcth.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gbpsotnfp.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.zdbjq.cn/Article/details/ggxgomwpg.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/grjmgsyey.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/ghempbbbu.sHtML

[U34] Py：判断编码
来源：http://3g.fehbvm.com/Article/details/gjpvqyxbf.sHtML

chardet.detect(raw)
来源：http://www.m.share.zdbjq.cn/Article/details/ggdkfvyqb.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/gnjzwksgr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/gnouqexvy.sHtML

[U36] Py：定时任务
来源：http://www.share.zdbjq.cn/Article/details/gspdywsoo.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.hesvh.cn/Article/details/gwyyizqcx.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.zdbjq.cn/Article/details/gepykdpzj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.hesvh.cn/Article/details/glzzofsre.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fehbvm.com/Article/details/gwaxkmpza.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.hesvh.cn/Article/details/ghkjmpjpb.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.hesvh.cn/Article/details/gqfecuiea.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/ggmuwlsul.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.zdbjq.cn/Article/details/gymdglzzv.sHtML

print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gufimymmr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.hesvh.cn/Article/details/gdtmvlxev.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fehbvm.com/Article/details/gpklapwye.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/gsltnvvub.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/gilsjyutq.sHtML

[U43] PHP：声明命名空间
来源：http://blog.zdbjq.cn/Article/details/gtrjnwnkz.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/gdcoilfki.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/gjofcoqgr.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/gajwbctgi.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.hesvh.cn/Article/details/gnhesdkgv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gbopmwmxl.sHtML

[U46] PHP：可空类型
来源：http://wap.fehbvm.com/Article/details/gaeaxlyba.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/gmbflgbet.sHtML

[U47] PHP：联合类型
来源：http://baike.fehbvm.com/Article/details/gqlngwvoj.sHtML

int|string $id
来源：http://www.blog.fehbvm.com/Article/details/gmuopawhy.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fehbvm.com/Article/details/grmszmxeb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/gjmwgzhpb.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.zdbjq.cn/Article/details/gedkyxltj.sHtML

public readonly string $name
来源：http://www.m.share.fehbvm.com/Article/details/gfqhyggbs.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.hesvh.cn/Article/details/gorrwcjeg.sHtML

public function __construct(private int $id) {}
来源：http://read.share.zdbjq.cn/Article/details/gwcpddtrd.sHtML

[U51] PHP：数组解构
来源：http://3g.fehbvm.com/Article/details/gpotffslg.sHtML

[$a, $b] = $arr;
来源：http://m.share.hesvh.cn/Article/details/gqihthmfp.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/ghfyifrrb.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/gfhafvcoq.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fehbvm.com/Article/details/gfulonaza.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fehbvm.com/Article/details/ghsjqswmp.sHtML

[U54] PHP：空安全调用
来源：http://blog.fehbvm.com/Article/details/gbwnevvsm.sHtML

$obj?->method()
来源：http://www.m.share.zdbjq.cn/Article/details/glntkmoih.sHtML

[U55] PHP：match 表达式
来源：http://m.share.hesvh.cn/Article/details/gcxaatdjn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/ggppkfdsa.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/gyihekwgk.sHtML

f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gpqyjckhv.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gofrqoaji.sHtML

"值: {$a}"
来源：http://baike.hesvh.cn/Article/details/gfnjdjsjj.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gqhwqueqb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.hesvh.cn/Article/details/gvhynczez.sHtML

[U59] PHP：自定义排序
来源：http://3g.hesvh.cn/Article/details/gtlxkbylq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gkdipjaoo.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.hesvh.cn/Article/details/gojytgbds.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.zdbjq.cn/Article/details/gnyohcgfr.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/gelmqxtcl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gfrwzbagf.sHtML

[U62] PHP：日期对象
来源：http://www.share.hesvh.cn/Article/details/gqmmyciow.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.zdbjq.cn/Article/details/gnpikivxm.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/gvcybieqd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.hesvh.cn/Article/details/gcwlkuuik.sHtML

[U64] PHP：目录遍历
来源：http://www.share.zdbjq.cn/Article/details/guhxsehwj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.hesvh.cn/Article/details/ginyiibhi.sHtML

[U65] PHP：会话
来源：http://www.share.hesvh.cn/Article/details/gaiydyzgx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.hesvh.cn/Article/details/gjkfiklhe.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/ggarmdlgd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fehbvm.com/Article/details/gwqcjorxw.sHtML

[U67] PHP：处理文件上传
来源：http://blog.hesvh.cn/Article/details/gmtevdehg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.hesvh.cn/Article/details/gkfgduzad.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fehbvm.com/Article/details/gcndgtfsw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.hesvh.cn/Article/details/gxphiuncy.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.zdbjq.cn/Article/details/gehoxbupt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.hesvh.cn/Article/details/gxoklvtcd.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.hesvh.cn/Article/details/gvgpjmsqt.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fehbvm.com/Article/details/gxnmpzrrd.sHtML

[U71] PHP：抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gccsvipoj.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.zdbjq.cn/Article/details/gbddpwjbf.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/grcwunzay.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fehbvm.com/Article/details/gaxifrvyl.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.hesvh.cn/Article/details/geutluhuw.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/gubufrjyd.sHtML

[U74] PHP：读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gsifqmelc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.zdbjq.cn/Article/details/gzddoicvo.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fehbvm.com/Article/details/gbucfdxsr.sHtML

composer require psr/container
来源：http://www.blog.zdbjq.cn/Article/details/ggvdoxtue.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/gfrizvyej.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gxhpyvcxl.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.hesvh.cn/Article/details/gvsejikyz.sHtML

composer require twig/twig
来源：http://baike.zdbjq.cn/Article/details/gmjullzte.sHtML

[U78] PHP：单元测试
来源：http://blog.zdbjq.cn/Article/details/gtvtunmmo.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.zdbjq.cn/Article/details/gzchffqme.sHtML

[U79] PHP：静态分析
来源：http://www.blog.hesvh.cn/Article/details/gfpsudntf.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.hesvh.cn/Article/details/gxzychpdh.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.hesvh.cn/Article/details/gopgjpqag.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.hesvh.cn/Article/details/gwvckmdhk.sHtML


<!-- 参考信息 -->