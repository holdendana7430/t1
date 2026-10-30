代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/gvxbqktem.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gpazsevbr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gyyeterar.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/gsyhjiyku.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gzelpsjxv.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gjabwqqdg.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/ggsiyvgiq.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gqrlfbzhg.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gnbdfdoap.sHtML

[S59] C++：静态断言
来源：http://read.share.fehbvm.com/Article/details/gsbparzya.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gythvrvia.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gndtpyurc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/grxpbxdrf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggofdltki.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gweovyzhe.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gaszswfzl.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/gzwbdakng.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/giqlbouxq.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/gmhtwdzmf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/gmpprspnw.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/gvdlswynl.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gvcdnhbfs.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/gtifuweoi.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/grqxhzebd.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gjkgcghfw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gcihvebyy.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gcnhrhmda.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/gdrxrnrgp.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gitieyegx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gcbchpbzt.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gznvlykbj.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/gijrnzcgy.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/gqmvegecd.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/gexfuvkbe.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gdlqogwvq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/gvoqxcddp.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gfwtxgzch.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/ghzwcwolo.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gbasskrol.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/guajzyycl.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/gfipeyrap.sHtML

val m = mapOf("a" to 1)
来源：http://3g.zdbjq.cn/Article/details/gpmakvejs.sHtML

[T14] Kotlin：循环
来源：http://blog.zdbjq.cn/Article/details/gwfjkemfr.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gqhywobpr.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/ggcdjqujs.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/glgmihjjd.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/gwoboklgd.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gcmsaidyw.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/gbwzxuwqo.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/ggwaqzrsy.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gyltzlbdb.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/gzbxyzfol.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gzmtxdqam.sHtML

if let n = opt { print(n) }
来源：http://blog.fehbvm.com/Article/details/gjcdnrzwt.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gmuflglwx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/gtplgkzmh.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/gyrnxddwu.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/giqmqwufz.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/gaudqfcmp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fehbvm.com/Article/details/gusaqpajh.sHtML

[T23] Swift：函数
来源：http://3g.zdbjq.cn/Article/details/ghyjwwezc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/gofvrqaog.sHtML

[T24] Swift：闭包
来源：http://www.blog.fehbvm.com/Article/details/gglsthkrz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gzvjbcyuq.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/ggzchdhul.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gelhithuq.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/gyvehqdja.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gtmjbhpjw.sHtML

[T27] Swift：错误处理
来源：http://read.share.hesvh.cn/Article/details/gtxkscprl.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gulqitepp.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gbppxmnjj.sHtML

enum Color { case red, green }
来源：http://3g.hesvh.cn/Article/details/gaavwzerb.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/grdmhckpf.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gnvnfvzpj.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gipqlyjfg.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/gbjdxdaup.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/gsgdjiyac.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gydtdxvcs.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/goqigysqx.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gjhuozygi.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/gvdgbeibl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/guxbhjgxo.sHtML

[T34] Lua：遍历表
来源：http://www.share.hesvh.cn/Article/details/gqyfmnvnr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/grshcljyl.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gvkszjcxt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/gtdwrkciy.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gqszqnqqj.sHtML

function add(a, b) return a + b end
来源：http://baike.hesvh.cn/Article/details/gadyvgkkx.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/goxvhzxrm.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/gyreitkpr.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/gjicivtzk.sHtML

if x > 0 then print("正") end
来源：http://baike.hesvh.cn/Article/details/gudqbzckj.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/ggfraaabm.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/gtmmbkwui.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/gtvsxyvmy.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gcriwaghm.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/ghvlpdvpf.sHtML

print "Hello\n";
来源：http://baike.hesvh.cn/Article/details/gmrqxuudo.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gliqwqznc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.hesvh.cn/Article/details/geszdqdcq.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/gfcoqpkau.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/geuqpvhns.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/gjczhocpz.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gvnnwahqf.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/glosikopt.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gwnpkjxvk.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gbvpadxme.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gqneltwqh.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/gxjunsxoz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/gsatvckje.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gaumlrbno.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/gbeszhlsa.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/gvwsenyoo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/greqsutra.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gycjwojsy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fehbvm.com/Article/details/gkrheggnl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gedmhobnq.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/gagnxrrbp.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gknwdprpx.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gqvlrodxo.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/gwguphptn.sHtML

[T53] Scala：字符串插值
来源：http://3g.hesvh.cn/Article/details/gmnydhgvr.sHtML

s"值: $b"
来源：http://mobile.hesvh.cn/Article/details/ghluhehsb.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gicobpffz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/gctswsqxj.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/ggxwdzlat.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.hesvh.cn/Article/details/gfbxndmag.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/guhxxliwz.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fehbvm.com/Article/details/grdumbqdu.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gymlqhocv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.zdbjq.cn/Article/details/gdnyiaqtb.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/gypcjvpjb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/gzfhukuzc.sHtML

[T59] Scala：循环
来源：http://baike.fehbvm.com/Article/details/gndrpntok.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gzkosonyc.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/gdgeugjty.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fehbvm.com/Article/details/ggrviywzi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcxtnlyre.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gqrbeebhl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gujnqvvqb.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fehbvm.com/Article/details/gyrpockqp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/ghukfxmhy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/gstxjmghr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/gsymkxmmz.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gbhddqrmw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/gtltepblp.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/gcxpyfqcx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/gjxwxqwoo.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fehbvm.com/Article/details/gizlsxbph.sHtML

list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gsfqdmbyq.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.hesvh.cn/Article/details/ghdydlejx.sHtML

{**a, **b}
来源：http://3g.fehbvm.com/Article/details/gjextwzxx.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/gzpchrtmf.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/guyuxwczg.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/ggiwftwqt.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gthddgtaf.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fehbvm.com/Article/details/gctiwaewe.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/gvosdakqe.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.zdbjq.cn/Article/details/gdjybjxhd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.hesvh.cn/Article/details/gzdcdsdnk.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.zdbjq.cn/Article/details/goaanmjci.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gaerflwnk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/gxpombhkt.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/grjkabztu.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.zdbjq.cn/Article/details/gvpkzjoug.sHtML

deque(maxlen=10)
来源：http://www.share.fehbvm.com/Article/details/glucndiav.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fehbvm.com/Article/details/gvtajrwcz.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/gvskrikuy.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/gbdengydf.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gqizzwvmf.sHtML

[U16] Py：命令行参数解析
来源：http://baike.zdbjq.cn/Article/details/gdlfjqfys.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.zdbjq.cn/Article/details/gotzaozkt.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/gyiwfkjul.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.hesvh.cn/Article/details/gudpfuiby.sHtML

[U18] Py：预编译正则
来源：http://read.share.zdbjq.cn/Article/details/gtojhjjob.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gatchozge.sHtML

[U19] Py：正则替换带回调
来源：http://wap.hesvh.cn/Article/details/gtsfouffd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gkpcvmwtw.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/gmzbfuodj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/gyktzfhyt.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.hesvh.cn/Article/details/girvfbjmb.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/gtibyhkzi.sHtML

[U22] Py：矩阵转置
来源：http://read.share.hesvh.cn/Article/details/gotpvoadg.sHtML

list(zip(*m))
来源：http://baike.fehbvm.com/Article/details/gkqlcabar.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.hesvh.cn/Article/details/gwtxhocpm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/gukheawrq.sHtML

[U24] Py：路径操作
来源：http://mobile.hesvh.cn/Article/details/gwjjothdn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gnaaixtwg.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.zdbjq.cn/Article/details/gskjdsdzu.sHtML

csv.DictReader(f)
来源：http://3g.hesvh.cn/Article/details/gwpwjpukr.sHtML

[U26] Py：并发下载
来源：http://3g.fehbvm.com/Article/details/gxobechco.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/gthnvymtg.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.hesvh.cn/Article/details/gyouuwwhw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.zdbjq.cn/Article/details/gmmqkfoke.sHtML

[U28] Py：类型别名
来源：http://www.m.share.zdbjq.cn/Article/details/gkknsaytp.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/gayvpokkg.sHtML

[U29] Py：属性校验
来源：http://3g.fehbvm.com/Article/details/gnhurlyge.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/giobfowbi.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/glnounurm.sHtML

@dataclass(slots=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gfykochdg.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/ggmdvptna.sHtML

python -m pytest -q
来源：http://www.share.hesvh.cn/Article/details/gvecylgwt.sHtML

[U32] Py：代码格式化
来源：http://www.share.fehbvm.com/Article/details/gsgohgsfn.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fehbvm.com/Article/details/gncoouhxy.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/gxmrzjkgh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/gghofhrvb.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/ghbvpcapp.sHtML

chardet.detect(raw)
来源：http://www.m.share.zdbjq.cn/Article/details/grygraxou.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/gnzrtcvyi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.hesvh.cn/Article/details/gfwvbajkv.sHtML

[U36] Py：定时任务
来源：http://baike.fehbvm.com/Article/details/gsmcagwvb.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.hesvh.cn/Article/details/gbzluxjja.sHtML

[U37] Py：读写 Excel
来源：http://blog.hesvh.cn/Article/details/gyynpjoby.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.hesvh.cn/Article/details/glmojcqpg.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/gnlrswkfg.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.hesvh.cn/Article/details/ggntxuhoa.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.hesvh.cn/Article/details/gbhfpozuk.sHtML

sys.stdout.isatty()
来源：http://www.blog.fehbvm.com/Article/details/gayfywfik.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/gjcumylhn.sHtML

print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gerhwrzdv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fehbvm.com/Article/details/gwuqttsct.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/gdcwhepct.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fehbvm.com/Article/details/gwpfnywef.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fehbvm.com/Article/details/gkpugrzac.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/golkpeyjs.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/gaadvjngm.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.zdbjq.cn/Article/details/gsyyfhswx.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/gytfairek.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/geqzjupme.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gmjahtlsq.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fehbvm.com/Article/details/gwbkgqtjx.sHtML

?string $name = null
来源：http://www.blog.hesvh.cn/Article/details/gzkvnepjo.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/gorsjzico.sHtML

int|string $id
来源：http://www.m.share.hesvh.cn/Article/details/gotmbjmuk.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/ghndbdwzh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.hesvh.cn/Article/details/grxnrcbue.sHtML

[U49] PHP：只读属性
来源：http://3g.fehbvm.com/Article/details/gobuxvfdd.sHtML

public readonly string $name
来源：http://blog.hesvh.cn/Article/details/gjimoukdu.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/gcyxzkgse.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/gbflpnzem.sHtML

[U51] PHP：数组解构
来源：http://m.share.fehbvm.com/Article/details/gbfjcbpvs.sHtML

[$a, $b] = $arr;
来源：http://read.share.hesvh.cn/Article/details/gnbtmzeij.sHtML

[U52] PHP：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gadufwrwq.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gbgnkioqr.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.zdbjq.cn/Article/details/givhvyqqi.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fehbvm.com/Article/details/gqwqldrtd.sHtML

[U54] PHP：空安全调用
来源：http://read.share.hesvh.cn/Article/details/golgabuyi.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/gkbwmtnps.sHtML

[U55] PHP：match 表达式
来源：http://blog.zdbjq.cn/Article/details/gcafhhhrn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/gpwscewiy.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/gbkokjkyf.sHtML

f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gtolsckih.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/gtglkgumh.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gylcgbgfs.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/guxpvjzwz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gljjpawyz.sHtML

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/gmdnvoetv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/grgudvtmc.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fehbvm.com/Article/details/gboeozjil.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fehbvm.com/Article/details/gvfrpznky.sHtML

[U61] PHP：正则
来源：http://www.m.share.zdbjq.cn/Article/details/gssgkuwvw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/glxydfbjb.sHtML

[U62] PHP：日期对象
来源：http://read.share.hesvh.cn/Article/details/ggrjcdlkt.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.zdbjq.cn/Article/details/gqdyjupzn.sHtML

[U63] PHP：文件读写
来源：http://m.share.zdbjq.cn/Article/details/gnamttpgn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gjimgokxi.sHtML

[U64] PHP：目录遍历
来源：http://m.share.hesvh.cn/Article/details/giljxzrmd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.zdbjq.cn/Article/details/gtldjnbeo.sHtML

[U65] PHP：会话
来源：http://m.share.zdbjq.cn/Article/details/gfazwpxam.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gtnmdbuwt.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.zdbjq.cn/Article/details/grpqpayqw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.zdbjq.cn/Article/details/gadornqmb.sHtML

[U67] PHP：处理文件上传
来源：http://blog.hesvh.cn/Article/details/gvcvxpsfy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.zdbjq.cn/Article/details/gfecrttvs.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.zdbjq.cn/Article/details/glzgrbtgt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.hesvh.cn/Article/details/gskjndxnq.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.zdbjq.cn/Article/details/gnbjwkraa.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.hesvh.cn/Article/details/gifumegfw.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fehbvm.com/Article/details/guuaqgnhi.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fehbvm.com/Article/details/gsmcdipro.sHtML

[U71] PHP：抛出异常
来源：http://read.share.zdbjq.cn/Article/details/glzsdzdxb.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gvogskbwp.sHtML

[U72] PHP：写错误日志
来源：http://3g.hesvh.cn/Article/details/gbecnqwbg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fehbvm.com/Article/details/guswpxyqb.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/gzsxetuac.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fehbvm.com/Article/details/goeqkolrw.sHtML

[U74] PHP：读取环境变量
来源：http://wap.hesvh.cn/Article/details/gdwufopel.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fehbvm.com/Article/details/gmzcdcybj.sHtML

[U75] PHP：依赖注入
来源：http://mobile.hesvh.cn/Article/details/grrjmagtr.sHtML

composer require psr/container
来源：http://blog.fehbvm.com/Article/details/gqcjevhek.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/gvuvfkqib.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fehbvm.com/Article/details/gcubgtwun.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fehbvm.com/Article/details/gofomgiqh.sHtML

composer require twig/twig
来源：http://mobile.zdbjq.cn/Article/details/gruksiuoi.sHtML

[U78] PHP：单元测试
来源：http://m.share.zdbjq.cn/Article/details/glriqdynz.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.hesvh.cn/Article/details/gwpgfycht.sHtML

[U79] PHP：静态分析
来源：http://wap.hesvh.cn/Article/details/gqbhuocwc.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fehbvm.com/Article/details/gukhxjoyr.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.zdbjq.cn/Article/details/ggqamduas.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.zdbjq.cn/Article/details/gqpgmshtx.sHtML


<!-- 参考信息 -->