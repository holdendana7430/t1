代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gsxiqmauo.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gkiruaokz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gvtrkfcue.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/gqzleffaj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/gitckuqcv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvrasxcrk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gcgmsvwmy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grrjbwfbw.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gfkcvavfy.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gkhopfyoe.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/ggwcaixtl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gsatuukru.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/gzdkcntpt.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/glpnxgrci.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/graggvbqw.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/garpsyynk.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/ghyvikyym.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/grlprtodc.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gteuephur.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/ghebnyxvk.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gtmyvdfnz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gmatsrqzm.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/grnyxrmgb.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gqopfizfz.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gavvxxqhk.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gtcmnpbpd.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/ghxulgopb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/glxjxmpaf.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/gfjjxewli.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/gmvbefonc.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gkgtxiafj.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gdorrliic.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gpscxxcfg.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/guecxnwfs.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gvcxqlnom.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gevjzmitx.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/gnexipdok.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/ghpyobccg.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gzsysrioo.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/glgcipkhb.sHtML

[T17] Swift：变量与常量
来源：http://3g.zdbjq.cn/Article/details/gnxwkktfi.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/ghccfpgov.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/gxbftbagh.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/gkdydaqhu.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/ginyogvyc.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/gvxlgxlhx.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gukdbdsjn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.hesvh.cn/Article/details/gnpsklhmv.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/gkmjnkxej.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/giwihzsjp.sHtML

[T22] Swift：字典
来源：http://m.share.zdbjq.cn/Article/details/gaamlkyhe.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/gfgyyzpmh.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gkgbqlsts.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/gjeuzknye.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/gbqrysine.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gilejnpmj.sHtML

[T25] Swift：结构体
来源：http://m.share.zdbjq.cn/Article/details/gntachotv.sHtML

struct P { var x: Int }
来源：http://blog.zdbjq.cn/Article/details/gushapsuk.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/gpmloutno.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gcgzjtcbe.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/gfgudxvww.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fehbvm.com/Article/details/gmcynhkhh.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/gufovkjnu.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/gkznpmzps.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gviklbkqx.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/giigiiffz.sHtML

[T30] Swift：协议
来源：http://www.share.zdbjq.cn/Article/details/goemiapvm.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.hesvh.cn/Article/details/gbktvhudf.sHtML

[T31] Lua：Hello World
来源：http://blog.zdbjq.cn/Article/details/gvykfabvu.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gevyhytvp.sHtML

[T32] Lua：局部变量
来源：http://3g.hesvh.cn/Article/details/gizmrfapi.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/gpwistbrs.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/glzklqxsm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/gkjvuujfx.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/gqrmooziq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gqylaabet.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/gjbnjanhs.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/gtkgtysxg.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/gokdczjhp.sHtML

function add(a, b) return a + b end
来源：http://www.blog.zdbjq.cn/Article/details/gkidwgdtd.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gvqmzzwxx.sHtML

"a" .. "b"
来源：http://3g.hesvh.cn/Article/details/gcgssnqqq.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/gtpdpxjbs.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/ghqkmhyfr.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gmjmhquzo.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gjxffjvfn.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/gmpydbpsd.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/gzmvowlav.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gxxnegupo.sHtML

print "Hello\n";
来源：http://www.blog.hesvh.cn/Article/details/grmapggvv.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/gyutbncbx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/guvfisfmh.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/grgsrernz.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gdiyxowyf.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/gesseameq.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gmadjffej.sHtML

[T45] Perl：数组遍历
来源：http://baike.fehbvm.com/Article/details/gkqbvukue.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/giixhxols.sHtML

[T46] Perl：哈希操作
来源：http://wap.hesvh.cn/Article/details/gpsxdfofv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fehbvm.com/Article/details/gtftqgjqt.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/gqrsmrvth.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/gupkftrtg.sHtML

[T48] Perl：正则替换
来源：http://3g.fehbvm.com/Article/details/galegtooq.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.zdbjq.cn/Article/details/ggwlwtnft.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/gamvgnuux.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gtfnzeqyr.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gpmsueogq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/ghdutxibe.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/gzdfcvbcc.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/gntxmcajy.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gengyqiyq.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/gpafhcuku.sHtML

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/gkvtvkmfh.sHtML

[T53] Scala：字符串插值
来源：http://blog.fehbvm.com/Article/details/gjqwggvko.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gwygiqmmx.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/gbegsrvla.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gmelpsrpw.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gjkptuyvi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.hesvh.cn/Article/details/glbjdlkxk.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/ggetfmqya.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fehbvm.com/Article/details/gthbvscdr.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/gznvmiidc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/gpvthtgcr.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/gypnpugic.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.zdbjq.cn/Article/details/gmswwfmck.sHtML

[T59] Scala：循环
来源：http://read.share.fehbvm.com/Article/details/gstrtzaaf.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gwetwflvs.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/giomegrtu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gbbestmul.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/geuifqbxe.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/gxsvnqbrh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkieybfne.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gwwmqctfe.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gwtkvfaxs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/gtpkrzdro.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/ghppovxkc.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gfpbqqzif.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.zdbjq.cn/Article/details/gyesyafxd.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/gzkuxyvbt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/gbyslwrur.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/gecvpwrzh.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/glnucaayg.sHtML

[U06] Py：合并两个字典
来源：http://m.share.hesvh.cn/Article/details/ghqusprlq.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/gbmnfsbdh.sHtML

[U07] Py：反转字典键值
来源：http://baike.fehbvm.com/Article/details/gcgcszohk.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/grcjxufam.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/guptzeyfk.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/gvtppavdt.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.zdbjq.cn/Article/details/gusofjgxa.sHtML

max(d, key=d.get)
来源：http://blog.zdbjq.cn/Article/details/gbiumtelp.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/gmxddgjpt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/gkhqgyjeh.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/garneadoy.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gwtfypamb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/gxqosiyhm.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/gelvdvdod.sHtML

[U13] Py：固定长度队列
来源：http://blog.fehbvm.com/Article/details/gmevwkozt.sHtML

deque(maxlen=10)
来源：http://blog.fehbvm.com/Article/details/gflfjiagm.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gfcjkivls.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/gnscbruia.sHtML

[U15] Py：高精度计时
来源：http://mobile.zdbjq.cn/Article/details/gdyylayfp.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gjrxjdmjw.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/gxekxqyfn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/gcrpvuipl.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/ggbqqfsjd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/gunmkadkq.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/gqxknruoa.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/gvpwuxfjv.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/gsqtachjt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.zdbjq.cn/Article/details/grwgcwiag.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/gxwggepok.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/ggeomptee.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fehbvm.com/Article/details/gxwnvwgva.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/gomzbrcts.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/gvqwccura.sHtML

list(zip(*m))
来源：http://www.share.hesvh.cn/Article/details/gbfjifgts.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/gypdaspma.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/gsttwxgpf.sHtML

[U24] Py：路径操作
来源：http://baike.fehbvm.com/Article/details/gkneckgba.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gtlmjvozd.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.hesvh.cn/Article/details/gorxffpmp.sHtML

csv.DictReader(f)
来源：http://www.blog.zdbjq.cn/Article/details/gqwcnxeob.sHtML

[U26] Py：并发下载
来源：http://wap.hesvh.cn/Article/details/gmxzqaeoe.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.hesvh.cn/Article/details/gumrnywcb.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gdruxwpqs.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.hesvh.cn/Article/details/guibhcvxr.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gmeziqxzo.sHtML

UserId = int
来源：http://3g.zdbjq.cn/Article/details/gbkjgyqcr.sHtML

[U29] Py：属性校验
来源：http://m.share.zdbjq.cn/Article/details/gongcrrvz.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/grayufqik.sHtML

[U30] Py：数据类
来源：http://www.blog.hesvh.cn/Article/details/gstksfzpa.sHtML

@dataclass(slots=True)
来源：http://wap.zdbjq.cn/Article/details/gzkyivcqk.sHtML

[U31] Py：单测
来源：http://wap.fehbvm.com/Article/details/gfpbraenz.sHtML

python -m pytest -q
来源：http://www.share.hesvh.cn/Article/details/gvsmzykit.sHtML

[U32] Py：代码格式化
来源：http://blog.zdbjq.cn/Article/details/gbkypaulf.sHtML

ruff format . && ruff check --fix .
来源：http://baike.hesvh.cn/Article/details/gkyokrqxe.sHtML

[U33] Py：打包发布
来源：http://3g.fehbvm.com/Article/details/gqbnoyfki.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/gwgkyhvxw.sHtML

[U34] Py：判断编码
来源：http://wap.zdbjq.cn/Article/details/ghavfrxrs.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/gvyaczjbv.sHtML

[U35] Py：发送邮件
来源：http://wap.hesvh.cn/Article/details/gsgckepmy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fehbvm.com/Article/details/gcllxptgl.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/gwkbqkyjz.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.zdbjq.cn/Article/details/geqgxemdc.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/gztylvuvb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/govnkwelr.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/gtsppnhbm.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gvrtyyemc.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.hesvh.cn/Article/details/gzhhlfffm.sHtML

sys.stdout.isatty()
来源：http://read.share.hesvh.cn/Article/details/gnmrugqes.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fehbvm.com/Article/details/gpjukgcye.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/guvjlabnv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fehbvm.com/Article/details/gjlnihigb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.zdbjq.cn/Article/details/gguvpannw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/gipkhnapy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/gqhfytxde.sHtML

[U43] PHP：声明命名空间
来源：http://wap.zdbjq.cn/Article/details/gncdzffxb.sHtML

namespace App\Http;
来源：http://baike.hesvh.cn/Article/details/gnozobtvo.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/gngkwgqjq.sHtML

declare(strict_types=1);
来源：http://blog.hesvh.cn/Article/details/gwlknpmqy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fehbvm.com/Article/details/gtuzcuirs.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gtkjptkds.sHtML

[U46] PHP：可空类型
来源：http://mobile.fehbvm.com/Article/details/gqevwbiik.sHtML

?string $name = null
来源：http://baike.fehbvm.com/Article/details/gadbodszf.sHtML

[U47] PHP：联合类型
来源：http://m.share.zdbjq.cn/Article/details/gwxfedpne.sHtML

int|string $id
来源：http://www.blog.hesvh.cn/Article/details/gpznrcqrb.sHtML

[U48] PHP：纯枚举
来源：http://blog.fehbvm.com/Article/details/gwrmbxhcj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.hesvh.cn/Article/details/gqxdhwfig.sHtML

[U49] PHP：只读属性
来源：http://blog.zdbjq.cn/Article/details/gnokvsdee.sHtML

public readonly string $name
来源：http://read.share.fehbvm.com/Article/details/ggqawyjru.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.zdbjq.cn/Article/details/glqkpayme.sHtML

public function __construct(private int $id) {}
来源：http://wap.hesvh.cn/Article/details/gzxtieqsz.sHtML

[U51] PHP：数组解构
来源：http://3g.fehbvm.com/Article/details/grwvifxng.sHtML

[$a, $b] = $arr;
来源：http://3g.hesvh.cn/Article/details/gytkzbegi.sHtML

[U52] PHP：箭头函数
来源：http://baike.hesvh.cn/Article/details/gmfhkagtu.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gunqgdxfv.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/gcckptcvd.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/goegwwdpu.sHtML

[U54] PHP：空安全调用
来源：http://wap.zdbjq.cn/Article/details/gickcibhc.sHtML

$obj?->method()
来源：http://www.share.hesvh.cn/Article/details/gryshnuny.sHtML

[U55] PHP：match 表达式
来源：http://baike.fehbvm.com/Article/details/gczjyebyz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gklmvsjoo.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/gzamcwwck.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gvpetzyjy.sHtML

[U57] PHP：字符串插值
来源：http://baike.fehbvm.com/Article/details/gwwsljawb.sHtML

"值: {$a}"
来源：http://3g.hesvh.cn/Article/details/gokfhsujw.sHtML

[U58] PHP：数组三件套
来源：http://www.share.hesvh.cn/Article/details/gzvfofkpq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.hesvh.cn/Article/details/gsqiuptnf.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fehbvm.com/Article/details/gtolcwtjv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gjxqnnthn.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/gzpqkdavl.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fehbvm.com/Article/details/gqshtsbiz.sHtML

[U61] PHP：正则
来源：http://www.m.share.hesvh.cn/Article/details/gbyhuqdjt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gmpqjmdvn.sHtML

[U62] PHP：日期对象
来源：http://3g.hesvh.cn/Article/details/gysndanhk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.hesvh.cn/Article/details/gvcvwbxpe.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/gzpkqitcc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/gebbjvxib.sHtML

[U64] PHP：目录遍历
来源：http://m.share.zdbjq.cn/Article/details/gfueqclin.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fehbvm.com/Article/details/gpezicijr.sHtML

[U65] PHP：会话
来源：http://blog.zdbjq.cn/Article/details/gfoplcfjb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/ggyhlrooo.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.zdbjq.cn/Article/details/gjjdejzqo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/gxjfbtmix.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fehbvm.com/Article/details/gxkrdvcsa.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fehbvm.com/Article/details/gywocghzk.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fehbvm.com/Article/details/gxrpdpnob.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.hesvh.cn/Article/details/gxqnbwkai.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/gopwtfpub.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fehbvm.com/Article/details/grypunfpt.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.hesvh.cn/Article/details/gpqxyrbez.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fehbvm.com/Article/details/ghmdjulzw.sHtML

[U71] PHP：抛出异常
来源：http://3g.hesvh.cn/Article/details/gvqdvlzjt.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fehbvm.com/Article/details/gmtuosyfd.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/gwthvsree.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.zdbjq.cn/Article/details/grybcngtf.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.hesvh.cn/Article/details/glkljvtev.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.hesvh.cn/Article/details/gcewsrqge.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fehbvm.com/Article/details/grbzrpsyz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.hesvh.cn/Article/details/gpewhqdjc.sHtML

[U75] PHP：依赖注入
来源：http://mobile.hesvh.cn/Article/details/gysvxsfpt.sHtML

composer require psr/container
来源：http://mobile.zdbjq.cn/Article/details/gayvamxip.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/gjpqjalhk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/gvftjjbmn.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/gpjuubheo.sHtML

composer require twig/twig
来源：http://baike.fehbvm.com/Article/details/gfpehltaq.sHtML

[U78] PHP：单元测试
来源：http://3g.hesvh.cn/Article/details/gdrutqzcj.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.zdbjq.cn/Article/details/grgvwgbcy.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gxdybbbnw.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/gfoiwzglq.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.hesvh.cn/Article/details/gkrjnxkiv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.zdbjq.cn/Article/details/gudskovhx.sHtML

[U81] JS：初始化项目
来源：http://baike.hesvh.cn/Article/details/gklzrvlpq.sHtML

npm init -y;  npm i express
来源：http://baike.hesvh.cn/Article/details/gsqpwqebz.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fehbvm.com/Article/details/gwsumzcyf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fehbvm.com/Article/details/gnfolfxms.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fehbvm.com/Article/details/guoyjmbbx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gkjcippzv.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.zdbjq.cn/Article/details/gsubdbqme.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fehbvm.com/Article/details/ggpobqseh.sHtML


<!-- 参考信息 -->