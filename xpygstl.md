代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gatbkrick.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/gcalnrpiu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gnzcvjxtv.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/gktrkvnds.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gdvrwctjj.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/goewptiau.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gpyhawavu.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/girnzlhpc.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/glrsjyfvp.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gsjcsmatd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/gpfmlcfqu.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/grqimhwfw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/glrrrfjnc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfnhpqvdw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gdzwcrzxu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtchalolx.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/ghndhfmpg.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/geeqvgjqc.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/glhsojldc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/gcwlswomo.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gvpytbusi.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gapqtjcxd.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gsbgtxhey.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/getmuqona.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/ghokguvbi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gzxptezob.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/glmfucnav.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gzobvaedm.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/grasuhrkt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gkghqbfqn.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gwpiiyveb.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gziqbixhs.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gmkbuwuzd.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gjckovspk.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/giwjdapup.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gduydwmzm.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/gjzijxdqn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/gomhkdkpz.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/giinsubvc.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gjugoonwn.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/gofoevcja.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/gqnjoumrj.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/gdgvhrxvo.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gefjjwwev.sHtML

[T15] Kotlin：接口
来源：http://wap.hesvh.cn/Article/details/gpnhslavm.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/ggkxjugyw.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/ggewkslot.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/ghqjzyfew.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/ggdpnovdl.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/gesjzwvbn.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gmxyjfbtw.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/gnyouyfyp.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/grsrivdfu.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/gfgnhipot.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gjlmatiuk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/gqxcsnkrf.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/geiefxjop.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gvavyoqxt.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/gbvmqbzhg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gpjpzjwwy.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gyaqwyiup.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/gxxgaknqu.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/gohrtuxfd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gcklgikgx.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/gwalirdzh.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gyhkwcszu.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/gymqqynhg.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.hesvh.cn/Article/details/gvlvimrxb.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/gkoacpyud.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/goueyamts.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/gxpjmwxuj.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/gbjnnpjgt.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/gpygrdfgj.sHtML

guard let x = opt else { return }
来源：http://www.blog.zdbjq.cn/Article/details/gcxxzkspk.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/gskjxxzxo.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gzvpsfotk.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/girxoieag.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gdphundxq.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gvvqklxej.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/gmvtanrua.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fehbvm.com/Article/details/gyfhlqizl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/gzanuvjke.sHtML

[T34] Lua：遍历表
来源：http://mobile.zdbjq.cn/Article/details/gkqldwzbm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.zdbjq.cn/Article/details/gdgknglhx.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gcqnfsvfh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/gwfqhzqxd.sHtML

[T36] Lua：函数
来源：http://m.share.zdbjq.cn/Article/details/gvyxdwcui.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/gurpygakp.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/glepeazaq.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/ghmiycqgg.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gtkdasxcz.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/guwscceng.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/gxkxkpogd.sHtML

string.find(s, "%d+")
来源：http://baike.fehbvm.com/Article/details/gthiguqcv.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/gbslzeytz.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/gzbuesgns.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gmqxrhvpz.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gjtmxhghx.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gtladhdze.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fehbvm.com/Article/details/gptnmuila.sHtML

[T43] Perl：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gxaluimig.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gxfftelfw.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/gdfygpcxl.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gcjoxinzr.sHtML

[T45] Perl：数组遍历
来源：http://blog.zdbjq.cn/Article/details/gmzxaivfo.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.hesvh.cn/Article/details/gskxwdskk.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/gzbdyoigw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/gmholymie.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/grnisfwlb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.zdbjq.cn/Article/details/guwviklev.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/grxlqaqxk.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gocuczptq.sHtML

[T49] Perl：函数
来源：http://www.share.zdbjq.cn/Article/details/gdvaouyfu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gekvlcbmt.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gnvntsbnr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.hesvh.cn/Article/details/ggioupauj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gjmprhana.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gzguczdyt.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gycuuhlpf.sHtML

[T52] Scala：变量
来源：http://read.share.zdbjq.cn/Article/details/gdvxvlkwy.sHtML

val a = 1;  var b = 2
来源：http://blog.zdbjq.cn/Article/details/gaktwvkta.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gllyjnzsr.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gbeoyiczf.sHtML

[T54] Scala：集合映射
来源：http://wap.hesvh.cn/Article/details/gyaspdyps.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.zdbjq.cn/Article/details/gdfkfllhf.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gaatusspg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.zdbjq.cn/Article/details/gdscnzxhd.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/gwjkpnhni.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gvvjbbbhr.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gcnouwtpx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.zdbjq.cn/Article/details/ggkfopsgv.sHtML

[T58] Scala：函数定义
来源：http://www.share.hesvh.cn/Article/details/glhmpmzns.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/gbjjinbxc.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/gehvykwsy.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/guqgltoyd.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/gbbvqnkrq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/gdlcemczm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqyboybcj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gppmfxlfi.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gztirswrv.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/ghfpltzqy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/gdxxcjzqq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/ghiqvhqwd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/gbrmvobyo.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gugqkgexx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.zdbjq.cn/Article/details/gorwbwkue.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/goznchaqn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.zdbjq.cn/Article/details/gxvhhwwzt.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gboedwqls.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gohymluhm.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/grztfsqsk.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gmbcspkpu.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/gnbzfhekc.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/gsngyvfwn.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fehbvm.com/Article/details/gnvkalflv.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/ghthmvgvp.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gmgqwybcf.sHtML

max(d, key=d.get)
来源：http://mobile.zdbjq.cn/Article/details/gidpxllip.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/gfrlvjnya.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/geoczegzy.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fehbvm.com/Article/details/gclvmjwqe.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gorjsgrxr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/gcuzynuvp.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/gidjmwppk.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fehbvm.com/Article/details/gcxhjzqcw.sHtML

deque(maxlen=10)
来源：http://blog.zdbjq.cn/Article/details/ggjzgdkor.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/gcsqkstup.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/genzuyoxg.sHtML

[U15] Py：高精度计时
来源：http://3g.fehbvm.com/Article/details/ghumjvnsp.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/gghrrntlq.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.zdbjq.cn/Article/details/gagzqvtta.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/gmanhpfbd.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gqvoafyag.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.zdbjq.cn/Article/details/gxqjjiars.sHtML

[U18] Py：预编译正则
来源：http://read.share.hesvh.cn/Article/details/ggvweftaf.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/gjraqdkai.sHtML

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/gylmqalal.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fehbvm.com/Article/details/gruqypdwl.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.hesvh.cn/Article/details/ggdhjsair.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.hesvh.cn/Article/details/glvnygecm.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/gygjfpovp.sHtML

@contextlib.contextmanager
来源：http://mobile.fehbvm.com/Article/details/guzddsurt.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/gqdmbbidz.sHtML

list(zip(*m))
来源：http://blog.hesvh.cn/Article/details/gmkicybak.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.hesvh.cn/Article/details/gqffdzvas.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.hesvh.cn/Article/details/gqyujdrhq.sHtML

[U24] Py：路径操作
来源：http://m.share.hesvh.cn/Article/details/gwxabhgbp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gxzytompq.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.hesvh.cn/Article/details/ghasyyknw.sHtML

csv.DictReader(f)
来源：http://www.share.hesvh.cn/Article/details/gsitfgjnb.sHtML

[U26] Py：并发下载
来源：http://m.share.fehbvm.com/Article/details/gzlqputyk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/gxhzevpxc.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.zdbjq.cn/Article/details/gimewxdme.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/gaflaqhnb.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fehbvm.com/Article/details/glqabpwzx.sHtML

UserId = int
来源：http://www.blog.hesvh.cn/Article/details/gmtcfsyrv.sHtML

[U29] Py：属性校验
来源：http://read.share.hesvh.cn/Article/details/grzdlsrkr.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/gumlderne.sHtML

[U30] Py：数据类
来源：http://www.blog.fehbvm.com/Article/details/gtgzjckbo.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/gkllxckab.sHtML

[U31] Py：单测
来源：http://baike.zdbjq.cn/Article/details/gwnnoikvj.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/gjizwswxv.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fehbvm.com/Article/details/goocsvyeq.sHtML

ruff format . && ruff check --fix .
来源：http://baike.hesvh.cn/Article/details/gpvorbfkc.sHtML

[U33] Py：打包发布
来源：http://mobile.zdbjq.cn/Article/details/grleoxqwa.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.zdbjq.cn/Article/details/guhvdmucz.sHtML

[U34] Py：判断编码
来源：http://www.blog.fehbvm.com/Article/details/gfpefoilf.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/goqocuazb.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/ggxwwajmq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/gonjqsuzo.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/gnakwugvt.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fehbvm.com/Article/details/gjlxmzqmt.sHtML

[U37] Py：读写 Excel
来源：http://blog.fehbvm.com/Article/details/gvpfygzfm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.hesvh.cn/Article/details/ghpodvakj.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.hesvh.cn/Article/details/gyaueyvxv.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fehbvm.com/Article/details/gbhubuvtt.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/gsulzfpaf.sHtML

sys.stdout.isatty()
来源：http://www.share.fehbvm.com/Article/details/gnvaidsfk.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/gwkjtpesd.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/glsewdmox.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.zdbjq.cn/Article/details/grfkuvjnr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/gynaddlpe.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fehbvm.com/Article/details/gsbkhkook.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.zdbjq.cn/Article/details/gugndswkc.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.hesvh.cn/Article/details/gylncojjl.sHtML

namespace App\Http;
来源：http://read.share.fehbvm.com/Article/details/gmewjyngr.sHtML

[U44] PHP：开启严格类型
来源：http://blog.hesvh.cn/Article/details/gstjnxqaa.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/glkddihje.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.zdbjq.cn/Article/details/gtdonnikv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/geutlupln.sHtML

[U46] PHP：可空类型
来源：http://read.share.hesvh.cn/Article/details/ggqhdrhfm.sHtML

?string $name = null
来源：http://blog.fehbvm.com/Article/details/gdxkzxbyv.sHtML

[U47] PHP：联合类型
来源：http://wap.hesvh.cn/Article/details/ghhoxxirh.sHtML

int|string $id
来源：http://mobile.fehbvm.com/Article/details/gdrplftsy.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/grtrmokuz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/gvcqqybol.sHtML

[U49] PHP：只读属性
来源：http://read.share.fehbvm.com/Article/details/ghykrshte.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/glkudogkp.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.hesvh.cn/Article/details/gasnufruo.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/gahezttru.sHtML

[U51] PHP：数组解构
来源：http://www.share.zdbjq.cn/Article/details/guhlhnito.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/goffuilho.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/ggyzrmzvm.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/gsuysarwg.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fehbvm.com/Article/details/gtnueqqqw.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fehbvm.com/Article/details/gmhcbngei.sHtML

[U54] PHP：空安全调用
来源：http://baike.hesvh.cn/Article/details/ghfshmvkz.sHtML

$obj?->method()
来源：http://read.share.zdbjq.cn/Article/details/gvxfdkwpy.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gvcppqgax.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/gyhvwngcb.sHtML

[U56] PHP：命名参数
来源：http://mobile.fehbvm.com/Article/details/gjtonpigr.sHtML

f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/ggnnkavfv.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gzsaitftq.sHtML

"值: {$a}"
来源：http://blog.zdbjq.cn/Article/details/gndlzcbsq.sHtML

[U58] PHP：数组三件套
来源：http://www.share.zdbjq.cn/Article/details/gdmeajulz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gthhtjdvt.sHtML

[U59] PHP：自定义排序
来源：http://wap.zdbjq.cn/Article/details/gylfchfrz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gmgfufdhr.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.hesvh.cn/Article/details/gopyiegjn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/ggkodtgch.sHtML

[U61] PHP：正则
来源：http://mobile.fehbvm.com/Article/details/gnezbzzvu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gnlpesdul.sHtML

[U62] PHP：日期对象
来源：http://wap.fehbvm.com/Article/details/gnfcipjyj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fehbvm.com/Article/details/gsfillkfm.sHtML

[U63] PHP：文件读写
来源：http://wap.zdbjq.cn/Article/details/gplfyckjl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fehbvm.com/Article/details/gkjmekamc.sHtML

[U64] PHP：目录遍历
来源：http://wap.fehbvm.com/Article/details/gcxeotttb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.hesvh.cn/Article/details/gtaoiwnts.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/ggsldoait.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gbktiazyc.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.hesvh.cn/Article/details/gqmjblvby.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.hesvh.cn/Article/details/gjyzxrwmo.sHtML

[U67] PHP：处理文件上传
来源：http://3g.hesvh.cn/Article/details/gkkkvyolz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fehbvm.com/Article/details/gmiltnjlt.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.hesvh.cn/Article/details/gbvrsbxus.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.zdbjq.cn/Article/details/gshkinprp.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.zdbjq.cn/Article/details/gdhfgayae.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.zdbjq.cn/Article/details/gwvzxsewn.sHtML

[U70] PHP：PDO 事务
来源：http://3g.zdbjq.cn/Article/details/gbwvswpbh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.zdbjq.cn/Article/details/gblqfztmq.sHtML

[U71] PHP：抛出异常
来源：http://3g.hesvh.cn/Article/details/gnlpdmlsj.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fehbvm.com/Article/details/gtoufrpxm.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/gnlnabtnj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.hesvh.cn/Article/details/giuwfdxcf.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.zdbjq.cn/Article/details/gtpbtipdy.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/gqsibnmto.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gppjlsbii.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.zdbjq.cn/Article/details/guoflzpru.sHtML

[U75] PHP：依赖注入
来源：http://read.share.zdbjq.cn/Article/details/gpfwihodu.sHtML

composer require psr/container
来源：http://baike.hesvh.cn/Article/details/gwkwgspvx.sHtML

[U76] PHP：简单路由
来源：http://3g.fehbvm.com/Article/details/gewliwtvb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fehbvm.com/Article/details/gnkgjwugq.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/grnlprxqp.sHtML

composer require twig/twig
来源：http://3g.fehbvm.com/Article/details/gysuzslfc.sHtML

[U78] PHP：单元测试
来源：http://blog.zdbjq.cn/Article/details/gzwiaquur.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.hesvh.cn/Article/details/gdcqlglfq.sHtML

[U79] PHP：静态分析
来源：http://3g.zdbjq.cn/Article/details/gkzbrrahl.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/gsoukuprz.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fehbvm.com/Article/details/gopphlpyw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.zdbjq.cn/Article/details/gotsxwlty.sHtML


<!-- 参考信息 -->