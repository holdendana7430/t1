代发 wailian999

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/ggskhwahu.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gngphjtgi.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gprmatyvn.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gpbhbivls.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gtsmmrvgp.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gthuklphy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/grruvovpp.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/guodorbnf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gatpjkbqa.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gtvqrnbdh.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/gtettokbj.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gjjhzhzsm.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gjsumoxie.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/ghbfnnkrk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/gcdrtjifu.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gyrkefppn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gjpmirgga.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gncpsdwlm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gzxeofyub.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkugbjmqq.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/gigplfjqn.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gyhvcddfb.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/ghojcsqnc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gkxplrzew.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gnmdadxlw.sHtML

"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gpcxcyqzb.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/govrlnjis.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/grafbgtyv.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gprwjarog.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gbrartusq.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gwplgnwzq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/ghxtspbix.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gelervanu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gblnyxhgs.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gzuutnwcm.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gcknskyox.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gjikdnvxp.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gdfzodrik.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/gcfiuthnb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/gxzcnrmfc.sHtML

[T11] Kotlin：协程
来源：http://3g.hesvh.cn/Article/details/gfxyyxasc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/grmyffldk.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gvugdwhvy.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gqanjuphx.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/gqmblkems.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gjxnnoajs.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/gprxasbuq.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gihtnsrvr.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/ghfcdvmmv.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/gnxjafwch.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/gztuqysdh.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gvloazubb.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gttjendkh.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gwwsxcdlp.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/giaxclgyz.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/gskromari.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gqufedswc.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gjjrtxgzj.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/gcgpjluut.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/gbpmrbqmb.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/gvoevidrv.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gwzkpddfu.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/gombzhrve.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/gxvdclnnf.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/gusxhplrh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.hesvh.cn/Article/details/gdpreaggg.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/gjhrktuol.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gadkwiyvh.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gacpwwkks.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gofruirli.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/gewmwjpap.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/gcbfcuolk.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/gciohrwdt.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gvdzerpkd.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gihlvxcwl.sHtML

enum Color { case red, green }
来源：http://www.share.fehbvm.com/Article/details/gbdosetib.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fehbvm.com/Article/details/gxfdylgxa.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gqpfhqlex.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/gryiduwib.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gicqnwnzo.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gdtijxcsv.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/goaqkhfrh.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/giyblmgyq.sHtML

local a = 1
来源：http://read.share.zdbjq.cn/Article/details/grvbzzbab.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fehbvm.com/Article/details/gkeelqbfj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/ghalqyuxh.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/ghxkxxpvx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/gzkdsxpgs.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gwhwlvqix.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fehbvm.com/Article/details/gwkckkqlx.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gcrfaqohk.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.hesvh.cn/Article/details/gqcfnoqqk.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gezmctusy.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/grundofsj.sHtML

[T38] Lua：条件
来源：http://read.share.zdbjq.cn/Article/details/goijzfkno.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gpnryuucs.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gtjxdnhsc.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/grangqwov.sHtML

[T40] Lua：元表
来源：http://wap.zdbjq.cn/Article/details/gaiczxmhp.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/gdasocpps.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/gelfxswlm.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/ggmnsvpcq.sHtML

[T42] Perl：变量类型
来源：http://m.share.hesvh.cn/Article/details/gjsjpaskv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/giajwwbze.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gmbomtole.sHtML

"值: $a"
来源：http://wap.zdbjq.cn/Article/details/givssxegk.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gjaojgisn.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/gxomwbirw.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gpstsnvml.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/gbdhkgsgd.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/gzxiqpbnv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.hesvh.cn/Article/details/gvlevsbcd.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/gpftovqbc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/gshcdgrzg.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/gwzpewtxf.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gonjvkmgl.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/grbfknbsx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gekugyjct.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/guolzcqzh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/gqxymvrbw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gsjwsrqzv.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gnaaicimh.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gzywziprm.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gbmnrxfrs.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gpikjkozo.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/goiajqofj.sHtML

s"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gxqwujbyj.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gxrfbtawd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/gqosertzk.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gxgkosihk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/gjmofxykc.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/gacrdodsi.sHtML

case class User(name: String, age: Int)
来源：http://blog.hesvh.cn/Article/details/gbocrmkca.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gaqygzusd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gqsvafrkb.sHtML

[T58] Scala：函数定义
来源：http://mobile.zdbjq.cn/Article/details/gfibwsemq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gymrfmzzu.sHtML

[T59] Scala：循环
来源：http://baike.fehbvm.com/Article/details/gwebhdgss.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.zdbjq.cn/Article/details/guvvrzybv.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/grzovecnj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gzltobgns.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gafhjmmjv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/gduknjvqy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdsamnjdn.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/gdplzluvg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/gyqercysd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fehbvm.com/Article/details/gowacayfs.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/glatckbta.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.zdbjq.cn/Article/details/ghkeyepni.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/gqqnkoccx.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/graqebpwx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/gbsvdspby.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fehbvm.com/Article/details/gerqxtcra.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/ghuhjicmg.sHtML

[U06] Py：合并两个字典
来源：http://baike.zdbjq.cn/Article/details/gutllvpah.sHtML

{**a, **b}
来源：http://3g.zdbjq.cn/Article/details/gifezefpl.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/gtfpoklgj.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.hesvh.cn/Article/details/gvvemaryz.sHtML

[U08] Py：展平二维列表
来源：http://www.share.zdbjq.cn/Article/details/gljavpnxo.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/gtuxhsmwy.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gpuzgyeeh.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gxoekigkq.sHtML

[U10] Py：按值排序字典
来源：http://m.share.zdbjq.cn/Article/details/gemgvnwae.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.hesvh.cn/Article/details/ghzgdwhcc.sHtML

[U11] Py：生成器表达式
来源：http://baike.hesvh.cn/Article/details/gisyeqxxo.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/gpyihqjhy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/gvjhvhvas.sHtML

Counter(arr).most_common(3)
来源：http://mobile.hesvh.cn/Article/details/gukpvkroe.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fehbvm.com/Article/details/gsuqkxgbg.sHtML

deque(maxlen=10)
来源：http://wap.hesvh.cn/Article/details/gknaxbisi.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/gbkjmvdts.sHtML

defaultdict(list)
来源：http://www.share.hesvh.cn/Article/details/ggflpsujd.sHtML

[U15] Py：高精度计时
来源：http://wap.fehbvm.com/Article/details/gyuejzgnm.sHtML

t = time.perf_counter()
来源：http://read.share.zdbjq.cn/Article/details/gmnfegojw.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fehbvm.com/Article/details/gythabyrg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.hesvh.cn/Article/details/gxtokybtj.sHtML

[U17] Py：初始化日志
来源：http://blog.zdbjq.cn/Article/details/gsvpaaypp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gkpsibdyy.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/glsvgnymt.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gjyzatjxn.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/gnloaiajg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/gqbbmmdmn.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.hesvh.cn/Article/details/githobfup.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.hesvh.cn/Article/details/goxuglkil.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/giqhsndly.sHtML

@contextlib.contextmanager
来源：http://www.share.fehbvm.com/Article/details/gjospzhja.sHtML

[U22] Py：矩阵转置
来源：http://wap.fehbvm.com/Article/details/gzoebwrye.sHtML

list(zip(*m))
来源：http://www.blog.zdbjq.cn/Article/details/goqrenzpe.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.hesvh.cn/Article/details/gglsqqmhj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/grnpanopn.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/gkxpfsgwn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gdpruxvys.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.zdbjq.cn/Article/details/gaivlzbhj.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/gvbcogeke.sHtML

[U26] Py：并发下载
来源：http://3g.fehbvm.com/Article/details/gvshylbqg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.zdbjq.cn/Article/details/gpbgephsn.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/gvglrcfyp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.zdbjq.cn/Article/details/gezbydvmw.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/gioyojull.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/gqlpbycuo.sHtML

[U29] Py：属性校验
来源：http://www.m.share.zdbjq.cn/Article/details/gxcwnjizt.sHtML

@property 与 @x.setter 配合
来源：http://3g.fehbvm.com/Article/details/ggulknidi.sHtML

[U30] Py：数据类
来源：http://blog.hesvh.cn/Article/details/gozlzxoes.sHtML

@dataclass(slots=True)
来源：http://m.share.fehbvm.com/Article/details/gcayzyhrk.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/gzywswrww.sHtML

python -m pytest -q
来源：http://www.share.fehbvm.com/Article/details/gtuoawzun.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/glxuxycvu.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/gckkuymws.sHtML

[U33] Py：打包发布
来源：http://wap.hesvh.cn/Article/details/gxkmhlybg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.zdbjq.cn/Article/details/gclooxmmd.sHtML

[U34] Py：判断编码
来源：http://m.share.zdbjq.cn/Article/details/gnlsrrblm.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/giexjrigr.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gmhxemoss.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fehbvm.com/Article/details/gadoqrupp.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/gbeyjkzlf.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.zdbjq.cn/Article/details/gkgwprjkd.sHtML

[U37] Py：读写 Excel
来源：http://read.share.zdbjq.cn/Article/details/gmhrtrluk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.hesvh.cn/Article/details/guiurgzwv.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.hesvh.cn/Article/details/gopqpxdvy.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/gcabkcwxq.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.zdbjq.cn/Article/details/gjkjwfeby.sHtML

sys.stdout.isatty()
来源：http://wap.hesvh.cn/Article/details/gpumruwag.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fehbvm.com/Article/details/gvmrgbanh.sHtML

print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gxltvwgpr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.hesvh.cn/Article/details/gljpfhkge.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/ghbdcoamj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.hesvh.cn/Article/details/garatcywz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.zdbjq.cn/Article/details/gbawnpzhg.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/golyvmqty.sHtML

namespace App\Http;
来源：http://wap.fehbvm.com/Article/details/gmbnbvmrt.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fehbvm.com/Article/details/gleinfyax.sHtML

declare(strict_types=1);
来源：http://www.blog.zdbjq.cn/Article/details/gqmdvtexr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.zdbjq.cn/Article/details/ghodeybje.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gdoujxegm.sHtML

[U46] PHP：可空类型
来源：http://mobile.fehbvm.com/Article/details/gmwncfurm.sHtML

?string $name = null
来源：http://m.share.fehbvm.com/Article/details/gcsdiowdd.sHtML

[U47] PHP：联合类型
来源：http://3g.fehbvm.com/Article/details/gihpkuiju.sHtML

int|string $id
来源：http://www.share.zdbjq.cn/Article/details/gezcbctoo.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/gxghuktxe.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.hesvh.cn/Article/details/gxlpzmbwy.sHtML

[U49] PHP：只读属性
来源：http://baike.zdbjq.cn/Article/details/gfrnafinj.sHtML

public readonly string $name
来源：http://mobile.hesvh.cn/Article/details/ggzalxuij.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fehbvm.com/Article/details/ghbxsygct.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/gzewgnaub.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/gapjshssi.sHtML

[$a, $b] = $arr;
来源：http://read.share.hesvh.cn/Article/details/gtypuejqm.sHtML

[U52] PHP：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gzhsiyfrt.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.hesvh.cn/Article/details/guvrbiifq.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.zdbjq.cn/Article/details/ghtymivgb.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fehbvm.com/Article/details/gdgqeokds.sHtML

[U54] PHP：空安全调用
来源：http://read.share.zdbjq.cn/Article/details/gldeuyeff.sHtML

$obj?->method()
来源：http://blog.fehbvm.com/Article/details/gavsqoqnj.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fehbvm.com/Article/details/gknxlsohf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/gswkvaxvz.sHtML

[U56] PHP：命名参数
来源：http://www.share.zdbjq.cn/Article/details/gffilddjm.sHtML

f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gewmuprnn.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gilxesmti.sHtML

"值: {$a}"
来源：http://mobile.hesvh.cn/Article/details/gukfjnzod.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/guytscsgr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/ggtbgphsa.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.hesvh.cn/Article/details/gmijghqip.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gxcnvehbx.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/gabgttajp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.zdbjq.cn/Article/details/gbnvyyasj.sHtML

[U61] PHP：正则
来源：http://3g.zdbjq.cn/Article/details/geaxvxibb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gtkhrxexj.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/gerhimpzs.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.hesvh.cn/Article/details/gyjiyznnh.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/gojbvsydg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/gozufuisp.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/gfwszexff.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fehbvm.com/Article/details/gfbpkmtzo.sHtML

[U65] PHP：会话
来源：http://read.share.fehbvm.com/Article/details/gwkfqguxc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gnrqptbld.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fehbvm.com/Article/details/gipwdcsfa.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.zdbjq.cn/Article/details/gnfklekmu.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.hesvh.cn/Article/details/grbuofwyq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.hesvh.cn/Article/details/goveyyjxy.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fehbvm.com/Article/details/gzahrprab.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.zdbjq.cn/Article/details/gantenvdj.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fehbvm.com/Article/details/gfnnrzbdc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.zdbjq.cn/Article/details/gcdqkjhzk.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fehbvm.com/Article/details/gqvyyzuwp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/gxzjxalyh.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/glrboryuh.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fehbvm.com/Article/details/gjrkhyucf.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fehbvm.com/Article/details/groibxkvp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/giyiezecd.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.zdbjq.cn/Article/details/gbjtcrxme.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/gtbqnkepg.sHtML

[U74] PHP：读取环境变量
来源：http://wap.hesvh.cn/Article/details/gukyfqmrm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.zdbjq.cn/Article/details/gkqrscnuy.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fehbvm.com/Article/details/gwxjjabja.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/gmdfbfdzn.sHtML

[U76] PHP：简单路由
来源：http://3g.zdbjq.cn/Article/details/gnuhzyopw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fehbvm.com/Article/details/gohgppcme.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fehbvm.com/Article/details/gtavtrnwh.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/ghzmucgds.sHtML

[U78] PHP：单元测试
来源：http://baike.fehbvm.com/Article/details/gklmzygpi.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fehbvm.com/Article/details/gomcmlggx.sHtML


<!-- 参考信息 -->