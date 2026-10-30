代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gkoizxsyl.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/grrviqlck.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/glieteqgk.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/gfpbskdek.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gybitwvuc.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/geapfufhd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.zdbjq.cn/Article/details/grutoliok.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gtuuhdvwj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/gapkyflve.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghqklmjhp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gvfwemtsj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/geqkifztl.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/grlsvghkn.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gbbjxxwzk.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/gjxfxyaxx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/ggwvaehsf.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/gmsgfissf.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/ggdspfpih.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/gikblmxlf.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gqntwgsfm.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gqimfmuuc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/gewmksewa.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/giffpiymd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gexjbsurj.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/gsloapeik.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gaqcgmogy.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gboehfuut.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gythjwphr.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/glyxlolqo.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gvsvvrcou.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gdfmzvnmp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gxaogmukx.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gjwhiaauv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/gpveqllik.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gxllzdqad.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gqykswtxc.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/gdgqxvvac.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gndtxftsw.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/geytvsixv.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/gedfexzzb.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/ggzwukzrj.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/goivwjucz.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gkonkenzp.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gfonzctog.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fehbvm.com/Article/details/glljhrobx.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/ghvlclmry.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/goyafhnxr.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/gtkzkbzia.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gmjphqodr.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gvgmjylas.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gbpsfxnje.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/gmcldhdbj.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/ggttsknft.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/gytehuubh.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gwlwhbpow.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gdpufzwze.sHtML

[T23] Swift：函数
来源：http://3g.hesvh.cn/Article/details/gajupmnql.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/gvtpiyzfh.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/glojqiyvc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gpkonojlu.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/gpvipqwbh.sHtML

struct P { var x: Int }
来源：http://www.m.share.fehbvm.com/Article/details/guoyopyym.sHtML

[T26] Swift：类与重写
来源：http://baike.hesvh.cn/Article/details/gwocbdlmi.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/gmogxxrzh.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/gekqnkfov.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/gjsgbhrcj.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/ghiuxscht.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/gkcizbaoz.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/gouxwqgid.sHtML

guard let x = opt else { return }
来源：http://m.share.zdbjq.cn/Article/details/gcwfjquoq.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/grvgluttp.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/gstelihaj.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gpgwafjxr.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/glymmrhmx.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gljdrtygn.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gteieqtzo.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gmhqwrymi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/gsrzfkoyy.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/gjsgxxthe.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/gsmzttgln.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/gsylinzne.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/gubndpfmw.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/gvahgunsh.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/gbnvjsrpr.sHtML

[T37] Lua：字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gxpplvgnd.sHtML

"a" .. "b"
来源：http://www.m.share.zdbjq.cn/Article/details/goflbjhxu.sHtML

[T38] Lua：条件
来源：http://read.share.fehbvm.com/Article/details/guoslnvti.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/gxrqygena.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/gwbbeppvz.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/gimgnicwp.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/gkgxgjnta.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/ghyezttqw.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/gxesheeqm.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gczgqzmvx.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/gazceozze.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/gkmqqexiv.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gobqmcnzj.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/gyyrroziy.sHtML

[T44] Perl：条件
来源：http://www.share.fehbvm.com/Article/details/gppphjfdj.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.hesvh.cn/Article/details/ggpjhvivm.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/gtraeghrw.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gbffiqdtp.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gtndnweyu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.hesvh.cn/Article/details/gmhqnwlso.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/gffonyvos.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/gcqvnkmak.sHtML

[T48] Perl：正则替换
来源：http://wap.fehbvm.com/Article/details/gwtoxlkuh.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/gowcxxkrx.sHtML

[T49] Perl：函数
来源：http://3g.zdbjq.cn/Article/details/gfrylhmdw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gjergxjxu.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gaweoouwx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fehbvm.com/Article/details/gsemxdsqm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.hesvh.cn/Article/details/gjpqkvwyj.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/grtyayxqz.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/glnkwbwan.sHtML

[T52] Scala：变量
来源：http://m.share.zdbjq.cn/Article/details/galybkpyj.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/gwnkqblyj.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gidvztwkb.sHtML

s"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gzlwqtawu.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/gmiuwowmg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gkiegwhvx.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gfujrhpbb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/gqceeroko.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/giyrmvurd.sHtML

case class User(name: String, age: Int)
来源：http://baike.zdbjq.cn/Article/details/gsxltxwvg.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/giqxpmdlg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fehbvm.com/Article/details/ghnlebaca.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/gknvppnzz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.zdbjq.cn/Article/details/ggeknyrym.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gcbetirew.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/gvcwlcfit.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/gupgppunn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fehbvm.com/Article/details/gioixaqcz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwinhcdkx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/gefohwfxp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gyfnbjczc.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/gnrgiscmk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/gsddkjxki.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/gaxutedxt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gadtpfssg.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fehbvm.com/Article/details/gposgomzc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.zdbjq.cn/Article/details/gxfozeayt.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gtqricuqq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.zdbjq.cn/Article/details/gltjmcpwd.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gaqgtnhbq.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gltgyuzhq.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/ggzliqcdh.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/gvjqtbavo.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.hesvh.cn/Article/details/gudsiiidq.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/gpkdyaeki.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/gtivpnqtl.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/glbysiktu.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/gbmamepzs.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/gbsmssmzj.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/ggptgcxtf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/gbrcvroro.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/gayncnwqf.sHtML

(x * 2 for x in arr)
来源：http://3g.zdbjq.cn/Article/details/gimxylyds.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/gzmzxzhpg.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gszyckbcp.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/gndmlwffa.sHtML

deque(maxlen=10)
来源：http://read.share.zdbjq.cn/Article/details/gvsluhwdu.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.zdbjq.cn/Article/details/gwwlrgesz.sHtML

defaultdict(list)
来源：http://read.share.fehbvm.com/Article/details/gyqdwkuvv.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/gclnxbhiq.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/gchdqrwzc.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/glhwkdtng.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gyihhgusy.sHtML

[U17] Py：初始化日志
来源：http://www.blog.zdbjq.cn/Article/details/gnjptzzjq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/glgwwkpit.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/gfokdjrnu.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fehbvm.com/Article/details/gxocjqypz.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/gcdmuzqha.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.hesvh.cn/Article/details/gnmkzotwb.sHtML

[U20] Py：缓存函数结果
来源：http://3g.zdbjq.cn/Article/details/gdvgxovyo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fehbvm.com/Article/details/gmlapadwx.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.zdbjq.cn/Article/details/glnfhpstm.sHtML

@contextlib.contextmanager
来源：http://www.share.fehbvm.com/Article/details/gisdtqhfb.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/gjzwchgdp.sHtML

list(zip(*m))
来源：http://www.blog.fehbvm.com/Article/details/gyjkslgbq.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/goxqfwcyd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/gjefdgmcz.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/gmbnygcxl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gaffbsnlu.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/gavhawpmc.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/ggchfhmbn.sHtML

[U26] Py：并发下载
来源：http://m.share.fehbvm.com/Article/details/gcghchzqa.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fehbvm.com/Article/details/ghxdoozow.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/ggzfjyrpk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.hesvh.cn/Article/details/gchotcmox.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/gpnmptixg.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/gbjqtqbym.sHtML

[U29] Py：属性校验
来源：http://m.share.fehbvm.com/Article/details/gwwjkxnwy.sHtML

@property 与 @x.setter 配合
来源：http://www.share.zdbjq.cn/Article/details/gjvygokch.sHtML

[U30] Py：数据类
来源：http://www.share.zdbjq.cn/Article/details/gcrfijjqm.sHtML

@dataclass(slots=True)
来源：http://www.blog.zdbjq.cn/Article/details/gzcpynkqp.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/gezfxdsho.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/glajcjhkd.sHtML

[U32] Py：代码格式化
来源：http://blog.zdbjq.cn/Article/details/gvxcnxgav.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/gnfgntoot.sHtML

[U33] Py：打包发布
来源：http://www.share.fehbvm.com/Article/details/gvzzffrms.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/gnqzjneos.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/gdgxcwafe.sHtML

chardet.detect(raw)
来源：http://blog.hesvh.cn/Article/details/gmxeujxft.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/gsjxeydhf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fehbvm.com/Article/details/gtqyonuwc.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/gdrthmduz.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/gyoiuvtvd.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/gfvlolydz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fehbvm.com/Article/details/grlnhtffc.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fehbvm.com/Article/details/giatvcxoj.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/guqiumdor.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/gcjatavuh.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/glrfngdoq.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/gdnddkqdk.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/ghvzfiwsj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fehbvm.com/Article/details/glffpxzfo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.zdbjq.cn/Article/details/ggdqfkdls.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.hesvh.cn/Article/details/gbbncxtyd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.hesvh.cn/Article/details/gadwgerbn.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.hesvh.cn/Article/details/gwdmglkgc.sHtML

namespace App\Http;
来源：http://wap.zdbjq.cn/Article/details/gciazxcwo.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.hesvh.cn/Article/details/gkmllbxyr.sHtML

declare(strict_types=1);
来源：http://mobile.fehbvm.com/Article/details/geuxqrcjw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/gkdkymoce.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gwrnfsust.sHtML

[U46] PHP：可空类型
来源：http://www.share.hesvh.cn/Article/details/ghterigza.sHtML

?string $name = null
来源：http://blog.hesvh.cn/Article/details/gijqkzdzp.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/gbgldpsre.sHtML

int|string $id
来源：http://www.share.zdbjq.cn/Article/details/gziuxjrri.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/ggyfestvi.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.hesvh.cn/Article/details/ganegrouo.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.hesvh.cn/Article/details/gmnuvrcxc.sHtML

public readonly string $name
来源：http://wap.hesvh.cn/Article/details/grwgmaogo.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.hesvh.cn/Article/details/gvkcdqxgo.sHtML

public function __construct(private int $id) {}
来源：http://blog.fehbvm.com/Article/details/grgixfxdn.sHtML

[U51] PHP：数组解构
来源：http://blog.hesvh.cn/Article/details/gvgnfyqyk.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fehbvm.com/Article/details/gqcfjshcq.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gkybafvbj.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fehbvm.com/Article/details/ggfqlpndw.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/grefvlrcl.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.zdbjq.cn/Article/details/gghdxjrxs.sHtML

[U54] PHP：空安全调用
来源：http://www.share.hesvh.cn/Article/details/gnyehhvvy.sHtML

$obj?->method()
来源：http://www.blog.zdbjq.cn/Article/details/gvtxrqxai.sHtML

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/grgflwtbi.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gvdhmxvxh.sHtML

[U56] PHP：命名参数
来源：http://wap.hesvh.cn/Article/details/gobqkzjvk.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gjuvnepnd.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gutojxvsf.sHtML

"值: {$a}"
来源：http://baike.zdbjq.cn/Article/details/gcjjybaom.sHtML

[U58] PHP：数组三件套
来源：http://baike.hesvh.cn/Article/details/ggtdatwlw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.hesvh.cn/Article/details/gbdgkzuuu.sHtML

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/gibzlxvwp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/grxmwfvqm.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/gqcyrowlf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/gknrpitmv.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/gkvoapnye.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/gwefwhwfz.sHtML

[U62] PHP：日期对象
来源：http://3g.zdbjq.cn/Article/details/gbxrisckh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fehbvm.com/Article/details/gikucigtb.sHtML

[U63] PHP：文件读写
来源：http://wap.zdbjq.cn/Article/details/gktqzresj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.zdbjq.cn/Article/details/ggnqhhtvv.sHtML

[U64] PHP：目录遍历
来源：http://blog.hesvh.cn/Article/details/gevedsnpm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fehbvm.com/Article/details/gtbcrnjxa.sHtML

[U65] PHP：会话
来源：http://blog.fehbvm.com/Article/details/grhkgkvat.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gcmqftmnv.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fehbvm.com/Article/details/gycehinun.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/gawajdlzi.sHtML

[U67] PHP：处理文件上传
来源：http://blog.hesvh.cn/Article/details/gglurxpmi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fehbvm.com/Article/details/gvzxeexvj.sHtML

[U68] PHP：PDO 连接
来源：http://3g.hesvh.cn/Article/details/gfdpjhwoe.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/gyaxxopqs.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.zdbjq.cn/Article/details/gxaufgvdy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.zdbjq.cn/Article/details/gsyenxohd.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.zdbjq.cn/Article/details/gvukuiebx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.zdbjq.cn/Article/details/gtequqnpf.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/gsqzaprmf.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/gqhkoeqro.sHtML

[U72] PHP：写错误日志
来源：http://www.share.zdbjq.cn/Article/details/gufmvckbw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fehbvm.com/Article/details/gsynxpoxm.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.zdbjq.cn/Article/details/gnsnpvzqc.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fehbvm.com/Article/details/gnmzpnxmr.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gxujuiqwu.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.hesvh.cn/Article/details/gaydwpznk.sHtML

[U75] PHP：依赖注入
来源：http://m.share.zdbjq.cn/Article/details/ghpyqsltu.sHtML

composer require psr/container
来源：http://baike.hesvh.cn/Article/details/gnsisqzlx.sHtML

[U76] PHP：简单路由
来源：http://baike.zdbjq.cn/Article/details/gyptlipfq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/gvkheutsk.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fehbvm.com/Article/details/gsszrzbwu.sHtML

composer require twig/twig
来源：http://www.blog.hesvh.cn/Article/details/gedydwasj.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/gglgkkjez.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fehbvm.com/Article/details/gdwohounx.sHtML

[U79] PHP：静态分析
来源：http://read.share.hesvh.cn/Article/details/gncvorjys.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fehbvm.com/Article/details/gucwdzepj.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/gcxdbvfjr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.hesvh.cn/Article/details/gnbbxftin.sHtML

[U81] JS：初始化项目
来源：http://baike.zdbjq.cn/Article/details/gvakxkind.sHtML

npm init -y;  npm i express
来源：http://www.share.hesvh.cn/Article/details/gwuwfrfwm.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.hesvh.cn/Article/details/gwljbtaxq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.hesvh.cn/Article/details/gpnvmyljs.sHtML


<!-- 参考信息 -->