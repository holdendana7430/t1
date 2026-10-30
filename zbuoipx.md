代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqimjrhk.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbnyiunw.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyduzxbr.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gullrxztg.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/glcmhlguw.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gjlpxcboe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gemaushru.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gchzgrpxw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gffshgudx.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwlmhgqb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/godeovqfx.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gvxwbffhc.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/glxuxasqm.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/ggokegere.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glaisludr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gwklhysam.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/glkuwfits.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/glsopkirn.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsxpfoya.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/gnztjamql.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcknexec.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gwowmietd.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gqcnnmmdl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gijxcqcov.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geojfupkm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gaitlkeir.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gfkwggaai.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gtaecncix.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gifjzpbqd.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/guchdbyvq.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrlrqbde.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gskojaogg.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gtofyjxsy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmmvhxjc.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/gentwignu.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrdpwaij.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnwmaqzi.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gwojoktxh.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxwmsqkm.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyfxjhab.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxdggwne.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gkgxxmyky.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrnrjzii.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gqurszypo.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtcfiklv.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbjvckjd.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giaaxopmw.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjtahssj.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gmokqenmf.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjizuxnks.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhayptud.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsosgfvym.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gmilikdyo.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzindbld.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlwotuti.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/ghjigbwww.sHtML

[T23] Swift：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrtwhqqf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbthdabf.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/glszcfxzn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/godjwskkn.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqujczwgb.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdauginqa.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/gllivovce.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/gpskmkeci.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gogrbgsug.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/gjulksnjo.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpnwbgzt.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galqxdrac.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gclznyljj.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/goyjuejef.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxykpcus.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaolbqvln.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvhewtqy.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gxxbjfpjs.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gommqwwbf.sHtML

local a = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gnprerkek.sHtML

[T33] Lua：表（数组）
来源：http://baike.fanxiaobao.xyz/Article/details/gxzngvaol.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/gzwfmtcnc.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/gmghxfzmi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowpxfxvr.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqgqufqs.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gebwgozqu.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gtkbwfxdr.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfpaaljt.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdqcqbbn.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/ghtsvvjra.sHtML

[T38] Lua：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspspqcvf.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/gihamwjxm.sHtML

[T39] Lua：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gegarpsal.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gdoryolbl.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/gkwgkuoyq.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrsnlxat.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcdpztwt.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gvcquxkhy.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekpwtwsq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gybysgild.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxnsffdd.sHtML

"值: $a"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrzrnbes.sHtML

[T44] Perl：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcdrawmb.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnabkkmsq.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gndyfgkhy.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzxpalmn.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggoyfescz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fanxiaobao.xyz/Article/details/giwsmicdt.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzqjgcly.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzznslky.sHtML

[T48] Perl：正则替换
来源：http://baike.fanxiaobao.xyz/Article/details/ghjhovudl.sHtML

$s =~ s/old/new/g;
来源：http://3g.fanxiaobao.xyz/Article/details/gttzmdlvp.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkjhjqzy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfdwezdxc.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjytxiva.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvzlbwwe.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfvgfnxob.sHtML

[T51] Scala：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gpikstezl.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gswhqwxyg.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gjadlwqcz.sHtML

val a = 1;  var b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/glejwwdyi.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gywpyffxk.sHtML

s"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfrjkvgw.sHtML

[T54] Scala：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/ggpbswczm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/goqlaccrr.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gulvdvfeo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkalpraz.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecpsirdh.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrkfjjsv.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkupxmxa.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqijllei.sHtML

[T58] Scala：函数定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhlbopyi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjxjbssp.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/guatrpzwu.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvegewuj.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/grykkizin.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/gmwxbfbaj.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gxpzsehdl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gcnjvwwnt.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxizcvtss.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fanxiaobao.xyz/Article/details/gxztgltme.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/gahrifoei.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/gannapfdq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/genydpsxf.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gnibtrneq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/gkkgyfxmz.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxjyvlpk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fanxiaobao.xyz/Article/details/gcndmrgum.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fanxiaobao.xyz/Article/details/gujjiydaq.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gxidpwpbs.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxbxlqon.sHtML

{**a, **b}
来源：http://3g.fanxiaobao.xyz/Article/details/ghwzlvety.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fanxiaobao.xyz/Article/details/gvspwharm.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgmuopdl.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gdceerspb.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/gbhlnhuyc.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fanxiaobao.xyz/Article/details/geqggoikt.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdizadbi.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gpycgazbz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/gvzfsanay.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gliumouty.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfxmxyun.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/gtstanunh.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gnohvlvnf.sHtML

[U13] Py：固定长度队列
来源：http://wap.fanxiaobao.xyz/Article/details/gerkoqcug.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokhnihgo.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gfoyaiyse.sHtML

defaultdict(list)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbryqxrvq.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvagussup.sHtML

t = time.perf_counter()
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyuottph.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fanxiaobao.xyz/Article/details/gtieuunas.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fanxiaobao.xyz/Article/details/geahoilqm.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gyoyqpwok.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaiigfvwy.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/gvzqemttz.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhgondid.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcfludcj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjlqpxuy.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/gaicdadvs.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fanxiaobao.xyz/Article/details/gypdayruy.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fanxiaobao.xyz/Article/details/grdjjolug.sHtML

@contextlib.contextmanager
来源：http://baike.fanxiaobao.xyz/Article/details/ghfoighwt.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxlcqmjt.sHtML

list(zip(*m))
来源：http://baike.fanxiaobao.xyz/Article/details/gqluviptm.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnoghxwzd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fanxiaobao.xyz/Article/details/gpqpunuiv.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gonytiufw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gmsanypwb.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfniomii.sHtML

csv.DictReader(f)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhptjamb.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcolwypv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghuiirzcc.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepszpsab.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fanxiaobao.xyz/Article/details/gclierjdc.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gzmcvswqj.sHtML

UserId = int
来源：http://blog.fanxiaobao.xyz/Article/details/gyyinpgnt.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwuipmzv.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqaeloeu.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxrbbewo.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitknceus.sHtML

[U31] Py：单测
来源：http://read.share.fanxiaobao.xyz/Article/details/gdifpduhw.sHtML

python -m pytest -q
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscaluniz.sHtML

[U32] Py：代码格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gjxzhtipi.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkmpsfuj.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/gbulihkeo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fanxiaobao.xyz/Article/details/gofsynzoq.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemtxdzau.sHtML

chardet.detect(raw)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaknizaae.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosvyjdin.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fanxiaobao.xyz/Article/details/goazlaikc.sHtML

[U36] Py：定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gibnjulem.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fanxiaobao.xyz/Article/details/grguuzecc.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fanxiaobao.xyz/Article/details/guypzyoop.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvebqtxj.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrqbtxje.sHtML

Path(__file__).resolve().parent
来源：http://baike.fanxiaobao.xyz/Article/details/griubejfq.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fanxiaobao.xyz/Article/details/guhnqcyvo.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/gqorjeojf.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdxdtgfe.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibigorev.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fanxiaobao.xyz/Article/details/gfsuefbpz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fanxiaobao.xyz/Article/details/gjoaumley.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/guckhglwg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fanxiaobao.xyz/Article/details/gbkylrmly.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyevytbbq.sHtML

namespace App\Http;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcliiojt.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxcynaor.sHtML

declare(strict_types=1);
来源：http://3g.fanxiaobao.xyz/Article/details/gzhjcwete.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gasovzmvs.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsfycrse.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvpyajme.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/gyxflkmnp.sHtML

[U47] PHP：联合类型
来源：http://wap.fanxiaobao.xyz/Article/details/gxhszuprz.sHtML

int|string $id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcevxeqfe.sHtML

[U48] PHP：纯枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gdfpuosoo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnoyagfhq.sHtML

[U49] PHP：只读属性
来源：http://wap.fanxiaobao.xyz/Article/details/gepvjeixx.sHtML

public readonly string $name
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcpvpedr.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbwxouky.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfxtkqbs.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajvjloho.sHtML

[$a, $b] = $arr;
来源：http://baike.fanxiaobao.xyz/Article/details/gkkeyfakh.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwbhvndp.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzxwwpwj.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fanxiaobao.xyz/Article/details/gcffbfatn.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fanxiaobao.xyz/Article/details/gsligjvqb.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfztopdt.sHtML

$obj?->method()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmhtliag.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/giohfsmpk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fanxiaobao.xyz/Article/details/gtddbgimy.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/geuahpexi.sHtML

f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzvvhhcm.sHtML

[U57] PHP：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gyjmkrxjw.sHtML

"值: {$a}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyoeqjtlf.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkzulhmt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmuvecuf.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gsaqliinf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhivsuyk.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fanxiaobao.xyz/Article/details/gkmmrmiqn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxozuyzp.sHtML

[U61] PHP：正则
来源：http://3g.fanxiaobao.xyz/Article/details/gghwucxna.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/girzflzqd.sHtML

[U62] PHP：日期对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gusmrpkob.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fanxiaobao.xyz/Article/details/gaijxvncj.sHtML

[U63] PHP：文件读写
来源：http://baike.fanxiaobao.xyz/Article/details/gcxlkwfyo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnpbdkin.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyajwyhd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fanxiaobao.xyz/Article/details/guzkfnkia.sHtML

[U65] PHP：会话
来源：http://blog.fanxiaobao.xyz/Article/details/goexeodys.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmowhvjln.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fanxiaobao.xyz/Article/details/gftwptqzn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/glcwjrorl.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fanxiaobao.xyz/Article/details/gumcnhtvn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbytvxkq.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fanxiaobao.xyz/Article/details/gsdynnosp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdzhqurq.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fanxiaobao.xyz/Article/details/gzvitwpnw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbonqdzrl.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gworzocej.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fanxiaobao.xyz/Article/details/gfsysqwzz.sHtML

[U71] PHP：抛出异常
来源：http://3g.fanxiaobao.xyz/Article/details/gqvrsiilc.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fanxiaobao.xyz/Article/details/gasmysbzz.sHtML

[U72] PHP：写错误日志
来源：http://blog.fanxiaobao.xyz/Article/details/gqqhyftbs.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqjdraon.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/grhexoypn.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fanxiaobao.xyz/Article/details/giikeytnw.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gqpbqkjev.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmlxasau.sHtML

[U75] PHP：依赖注入
来源：http://3g.fanxiaobao.xyz/Article/details/gamwvokiy.sHtML

composer require psr/container
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmfockmc.sHtML

[U76] PHP：简单路由
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfumsyrq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fanxiaobao.xyz/Article/details/gznrstcys.sHtML

[U77] PHP：模板渲染
来源：http://blog.fanxiaobao.xyz/Article/details/gyvtsgbvd.sHtML

composer require twig/twig
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxejujzwg.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmgwmqsg.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fanxiaobao.xyz/Article/details/gzaddqldq.sHtML

[U79] PHP：静态分析
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrhldprk.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbktkxbe.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fanxiaobao.xyz/Article/details/gfjcnsjak.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fanxiaobao.xyz/Article/details/gnokywftx.sHtML

[U81] JS：初始化项目
来源：http://wap.fanxiaobao.xyz/Article/details/gnekyfkcm.sHtML

npm init -y;  npm i express
来源：http://read.share.fanxiaobao.xyz/Article/details/gazacxooc.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fanxiaobao.xyz/Article/details/gmwytqvvx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fanxiaobao.xyz/Article/details/gxajgkozg.sHtML


<!-- 参考信息 -->