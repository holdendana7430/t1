代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gfwtjerlp.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/gzdfccevb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gksqabdxr.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/gqixuvcln.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/goyhskewk.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gvpdsvbqx.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gnuvjgslx.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/goticbofy.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gwgqoqqml.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gwtumovty.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/gqyrcgjpg.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gqdcmmhlv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/gdcfbfsez.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbkddgajy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gxkcdkbgq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gezjrucpp.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/gpvdfwjqt.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gasxsnfpm.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/gvfqcemdc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gntpqhwki.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gplsmlnqe.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/gbfbkqfjp.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/geeybeyyt.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/gxwyxuzdl.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gpqgqruus.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/gjrcnzegq.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/gwvoegifi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gokvaadis.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/grxfzjtui.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gootsltog.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/gxybofmbl.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gaedzwdai.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/glgrxwzoz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gqpkfmygw.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/gjcdjjqsn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gberbyamn.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/ggxamqind.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gqvglcitm.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gwxunamab.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/ghoorpbng.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/gloqoqaan.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/gjbpebyuh.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/gixdytsja.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gniybcboi.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/gdqkwsrku.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gaufkkccm.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/gdlxkmfog.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gatwbonoa.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/gfsbgwzoq.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/goeywyuyr.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/ghhiulrym.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/ghyftsewj.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/gjxumduhn.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gxzqinvlz.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gnqqyavkn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.hesvh.cn/Article/details/glukydbsz.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gtgtxpzfz.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gnyygvlje.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/gcdhzjrgz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.zdbjq.cn/Article/details/geiabbaqz.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gljwgnlqd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/gswgvwwra.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/ghgccblbz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gpuwlozjr.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gyqlzaram.sHtML

struct P { var x: Int }
来源：http://www.blog.fehbvm.com/Article/details/gqtbqrbem.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/gsuauabbn.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/giakclyeb.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/gmipvfser.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fehbvm.com/Article/details/gyuwckqgr.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gciwpilmr.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/gaixkogoe.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/giuflqpra.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/gqxzewser.sHtML

[T30] Swift：协议
来源：http://baike.zdbjq.cn/Article/details/gwtyakzpv.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/ghhadwsop.sHtML

[T31] Lua：Hello World
来源：http://3g.hesvh.cn/Article/details/gicomkkqf.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gtloigcpk.sHtML

[T32] Lua：局部变量
来源：http://www.blog.hesvh.cn/Article/details/gqpfuaqdj.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gbwlywgms.sHtML

[T33] Lua：表（数组）
来源：http://blog.hesvh.cn/Article/details/gweapfjtk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.zdbjq.cn/Article/details/goubzghbx.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/gfbxianlz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/gkvspqlph.sHtML

[T35] Lua：字典表
来源：http://wap.hesvh.cn/Article/details/gqeutxzhv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.hesvh.cn/Article/details/gopqivygx.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/gxqoflkbj.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/gipbxdgfl.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gbxknshxe.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/gyucqqkxc.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gczdrfook.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/glebrhlwf.sHtML

[T39] Lua：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gaeywxbvh.sHtML

string.find(s, "%d+")
来源：http://www.m.share.hesvh.cn/Article/details/grcjlalxs.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/ghaczqpmn.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/gbmqwzowl.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gfngqcenl.sHtML

print "Hello\n";
来源：http://read.share.hesvh.cn/Article/details/gotefpzch.sHtML

[T42] Perl：变量类型
来源：http://m.share.fehbvm.com/Article/details/gftehreii.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.hesvh.cn/Article/details/gcsxsthlk.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/gcsjhkksc.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gsmkapkcf.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/gqokrprum.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.hesvh.cn/Article/details/gnneyhhca.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/gjwwzocko.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fehbvm.com/Article/details/gmojmmxiu.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/ghvmserao.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fehbvm.com/Article/details/gfftbmckf.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/gsqrnncys.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/gikefhhod.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gmboboxfe.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/ginqrguaj.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/gauzoofoe.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/goshqjueg.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gmpwidpxh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fehbvm.com/Article/details/gpcrefici.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/gizerpioa.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/gezksxkyl.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gpfxkzhyk.sHtML

[T52] Scala：变量
来源：http://3g.fehbvm.com/Article/details/gtthyqgdg.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/gpzwbyhsb.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gjynrvhnb.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/geumapepg.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gjdqdrqlw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/ghyaxxkee.sHtML

[T55] Scala：集合过滤
来源：http://baike.fehbvm.com/Article/details/goxbigbto.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gsanmbtid.sHtML

[T56] Scala：样例类
来源：http://www.m.share.hesvh.cn/Article/details/gbuhswdzn.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/gngvxlicv.sHtML

[T57] Scala：模式匹配
来源：http://baike.hesvh.cn/Article/details/gtjfpryfu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/gbbkatwok.sHtML

[T58] Scala：函数定义
来源：http://baike.hesvh.cn/Article/details/gwacginjo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/gvlprnded.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/gvgwmhcaq.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gmuknrqsj.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/gajhmnpaq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.zdbjq.cn/Article/details/gmqvmgycj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggeoavkpv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/ghonrhykc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkzbtrgye.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fehbvm.com/Article/details/ggzqitogm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.hesvh.cn/Article/details/glamentuf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/geaqkqxqo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.hesvh.cn/Article/details/gysriblrx.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.hesvh.cn/Article/details/grfsidgct.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/glxjjzpbc.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/gzqconqra.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/guycualjs.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fehbvm.com/Article/details/grkqvdmfu.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gjpomvyjk.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gupvrzrmi.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/ggjzopcfr.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/gqnpevbnt.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/gtfseshqe.sHtML

[U08] Py：展平二维列表
来源：http://read.share.hesvh.cn/Article/details/gbtcmlwpn.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/gkmiekahd.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.zdbjq.cn/Article/details/gigftoyfz.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gbipqrymz.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.zdbjq.cn/Article/details/gpzdxvten.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fehbvm.com/Article/details/gqmstlpbf.sHtML

[U11] Py：生成器表达式
来源：http://3g.hesvh.cn/Article/details/gjrilgxbu.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.hesvh.cn/Article/details/ggyhwewqf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/ghrbwkagk.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/gicyecvua.sHtML

[U13] Py：固定长度队列
来源：http://baike.zdbjq.cn/Article/details/gqnojbhyx.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/guqjmjvbs.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.zdbjq.cn/Article/details/gtvfpcbfb.sHtML

defaultdict(list)
来源：http://www.blog.hesvh.cn/Article/details/gtpmkrjqi.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/gzaekdirr.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/gcheiyijb.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fehbvm.com/Article/details/gnkkshapj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fehbvm.com/Article/details/gvowjeigk.sHtML

[U17] Py：初始化日志
来源：http://blog.zdbjq.cn/Article/details/gnlezmnzm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.zdbjq.cn/Article/details/giekyxwbm.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.zdbjq.cn/Article/details/gbankrnbz.sHtML

pat = re.compile(r"\d+")
来源：http://baike.zdbjq.cn/Article/details/gppgctcoq.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/gqkeiqwte.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/gitvmohmw.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/ghkpbbork.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.zdbjq.cn/Article/details/glijnagia.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fehbvm.com/Article/details/gqwzunjis.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fehbvm.com/Article/details/gvoztfswh.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/guvnxkpbo.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/glhdmhonq.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/gkyquscfg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.hesvh.cn/Article/details/geypfaafd.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gfhnidngc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gmrbwfroo.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/gifwzxaem.sHtML

csv.DictReader(f)
来源：http://m.share.zdbjq.cn/Article/details/gmbxenqmu.sHtML

[U26] Py：并发下载
来源：http://3g.fehbvm.com/Article/details/ggjnyszlk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/gggwbkcpd.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/gxdmgydmp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.hesvh.cn/Article/details/gnjuytdck.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/gycuyvctl.sHtML

UserId = int
来源：http://wap.fehbvm.com/Article/details/glatbwvlb.sHtML

[U29] Py：属性校验
来源：http://www.blog.hesvh.cn/Article/details/garstigwh.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/glfkixdck.sHtML

[U30] Py：数据类
来源：http://wap.hesvh.cn/Article/details/gmlfncggi.sHtML

@dataclass(slots=True)
来源：http://wap.hesvh.cn/Article/details/gyzjlwkxj.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/gpxcrjqox.sHtML

python -m pytest -q
来源：http://read.share.zdbjq.cn/Article/details/gxhytrnjl.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/goeiumqxc.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.hesvh.cn/Article/details/gjotmatif.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/gxvcvxcsq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fehbvm.com/Article/details/gxieowxqy.sHtML

[U34] Py：判断编码
来源：http://www.m.share.hesvh.cn/Article/details/gkzgafgmu.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/ggsgjckmg.sHtML

[U35] Py：发送邮件
来源：http://www.share.hesvh.cn/Article/details/gstlokodc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/gxsajqnsy.sHtML

[U36] Py：定时任务
来源：http://www.share.fehbvm.com/Article/details/gampyuibr.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.hesvh.cn/Article/details/ghwtusmxn.sHtML

[U37] Py：读写 Excel
来源：http://read.share.zdbjq.cn/Article/details/gwwiuyrch.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fehbvm.com/Article/details/gvenwmrpc.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fehbvm.com/Article/details/gspkklwkr.sHtML

Path(__file__).resolve().parent
来源：http://baike.hesvh.cn/Article/details/giwtjvhls.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/garulzfri.sHtML

sys.stdout.isatty()
来源：http://blog.fehbvm.com/Article/details/guniqspeo.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.zdbjq.cn/Article/details/gwydigfam.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gpxfunprk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.hesvh.cn/Article/details/gfkbivhjx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fehbvm.com/Article/details/gotpweear.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/ggwzghvuw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fehbvm.com/Article/details/gkjsvmfeq.sHtML

[U43] PHP：声明命名空间
来源：http://3g.zdbjq.cn/Article/details/gjwpenkxy.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/gldvhmmqp.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fehbvm.com/Article/details/gyhcmcnnw.sHtML

declare(strict_types=1);
来源：http://www.m.share.fehbvm.com/Article/details/gzlwrehxd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.zdbjq.cn/Article/details/geauouzpv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/giftvdlcb.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/glojtssui.sHtML

?string $name = null
来源：http://wap.fehbvm.com/Article/details/gdmfxinrf.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/ghesdbhbr.sHtML

int|string $id
来源：http://www.share.zdbjq.cn/Article/details/gyabhexwm.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fehbvm.com/Article/details/glcmtyzxs.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/gpzdojpvb.sHtML

[U49] PHP：只读属性
来源：http://3g.fehbvm.com/Article/details/goapnrenj.sHtML

public readonly string $name
来源：http://www.m.share.zdbjq.cn/Article/details/gabyabkjs.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.hesvh.cn/Article/details/gqychdaou.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fehbvm.com/Article/details/gpkgynubl.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/guwtypjxb.sHtML

[$a, $b] = $arr;
来源：http://mobile.hesvh.cn/Article/details/gcihnmwya.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gqewqwfrl.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gllfnlsfg.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/gdahoogxq.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fehbvm.com/Article/details/gptfcgecg.sHtML

[U54] PHP：空安全调用
来源：http://blog.hesvh.cn/Article/details/gdprxdpnv.sHtML

$obj?->method()
来源：http://3g.hesvh.cn/Article/details/gkbqcredp.sHtML

[U55] PHP：match 表达式
来源：http://3g.hesvh.cn/Article/details/gdkygaxtg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.hesvh.cn/Article/details/gymzohhlv.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/gldvweamy.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/ghcmblmiu.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gumjzdmfi.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/gqysjrwbz.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.hesvh.cn/Article/details/gnsqbbyab.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.zdbjq.cn/Article/details/gxzokjvvg.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/gfphxlobq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gulppcqcl.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fehbvm.com/Article/details/gzxvvxobl.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.hesvh.cn/Article/details/gmuzlqvpi.sHtML

[U61] PHP：正则
来源：http://baike.zdbjq.cn/Article/details/gxlcyszug.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/guhkhguye.sHtML

[U62] PHP：日期对象
来源：http://3g.hesvh.cn/Article/details/glirloyif.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/gdulgkwxg.sHtML

[U63] PHP：文件读写
来源：http://m.share.zdbjq.cn/Article/details/gptmwztcd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/gospkoixb.sHtML

[U64] PHP：目录遍历
来源：http://mobile.zdbjq.cn/Article/details/gootzyizl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/gqcookqpt.sHtML

[U65] PHP：会话
来源：http://baike.fehbvm.com/Article/details/gnrgoafcs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/glorwjpqs.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/gxubwdwou.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.zdbjq.cn/Article/details/gmlymjwzm.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.hesvh.cn/Article/details/gqqwdwpgw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.zdbjq.cn/Article/details/gagbgvrmv.sHtML

[U68] PHP：PDO 连接
来源：http://wap.hesvh.cn/Article/details/ggzjzefcs.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.zdbjq.cn/Article/details/gvxbqtuos.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/ggyhkkmti.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fehbvm.com/Article/details/ghycrmfud.sHtML

[U70] PHP：PDO 事务
来源：http://3g.hesvh.cn/Article/details/gglglgiyx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fehbvm.com/Article/details/gfibkgftp.sHtML

[U71] PHP：抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gmmqolmgn.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/gvoaotvxl.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fehbvm.com/Article/details/glliqfjdl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.zdbjq.cn/Article/details/gsehnnuev.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gsiadqgmp.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/ggazpbwvk.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fehbvm.com/Article/details/gpofluvpk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/gizummfye.sHtML

[U75] PHP：依赖注入
来源：http://wap.fehbvm.com/Article/details/gczmukwcj.sHtML

composer require psr/container
来源：http://baike.hesvh.cn/Article/details/gaioyufzb.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/gxzwkukrr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/ghsvdpish.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/grxducxnn.sHtML

composer require twig/twig
来源：http://www.share.fehbvm.com/Article/details/gjzoallvk.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/glnjkslet.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.hesvh.cn/Article/details/gmxkpcnfa.sHtML

[U79] PHP：静态分析
来源：http://read.share.fehbvm.com/Article/details/gxbvbqugq.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fehbvm.com/Article/details/gyhavpllf.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fehbvm.com/Article/details/ganaxzayt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.hesvh.cn/Article/details/gfiizchrv.sHtML


<!-- 参考信息 -->