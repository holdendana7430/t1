代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gjtojqyon.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/ghcrnihvb.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/gxzwmuekd.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/glgaizwvp.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/gunvilqmf.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/gmpxujtvc.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/gcyuxjmwd.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/ghrzuzmai.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gbhfbpoeo.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gmmbuzdds.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gtkbztwho.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/gjjruzuty.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gketmumtl.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gxloqtbzi.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gnjlwrdru.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gtcimqirn.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gcvntshka.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/ggbzjxzgz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.zdbjq.cn/Article/details/ggfjjvqqt.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gvlzuvipp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/gqxeojakk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwfawdaqu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gnmjhrarm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdqmdjoeo.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fehbvm.com/Article/details/ghdamhnot.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gdxlvnbai.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gegsaojsn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gtlzqgvhk.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gnlgjngjz.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/ghkfztzvf.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/gwyommyoi.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/grngdrnoh.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gupbgmosv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/gmnorwtgk.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/grwyowoej.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gmslfjeke.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/gdsgudfqz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/gkubvjslt.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/gnpksxzgx.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/ggmnafxyj.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/givoesydv.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/grckpzuat.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/grlxakmca.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/gfmdmpaox.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/grpzhkzxs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/gddassvpq.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/gbpxyvhcd.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/ghyqosaia.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/gspwfkrox.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/glvemeuyd.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gijhyguwv.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/geptpftux.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/ghbxjvevy.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gbiwgjzgg.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/grisevuzk.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gpoxbetub.sHtML

[T17] Swift：变量与常量
来源：http://3g.zdbjq.cn/Article/details/goiiikyso.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/glqeleysx.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gbnluiqgk.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gixdccyke.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gexxrpyir.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gqlzlakwg.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/grybsnlhz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/gunysajwc.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/gxxkrzyqz.sHtML

for x in a { print(x) }
来源：http://blog.zdbjq.cn/Article/details/gazhxnsxk.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/grogdxnak.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gmdokovub.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/gudawgyvw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/gqbadsdub.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/gpoojczxo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/grzhjablb.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/gmbcspwgg.sHtML

struct P { var x: Int }
来源：http://mobile.hesvh.cn/Article/details/ggknyofod.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gmdnzclbv.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gwvbdeggr.sHtML

[T27] Swift：错误处理
来源：http://m.share.zdbjq.cn/Article/details/gwjqznbva.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/grucrpvhn.sHtML

[T28] Swift：枚举
来源：http://mobile.zdbjq.cn/Article/details/gxnsyeskx.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/gjxrwoawh.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gehrqslgz.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/gckruhior.sHtML

[T30] Swift：协议
来源：http://m.share.fehbvm.com/Article/details/gbxeebfcg.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.hesvh.cn/Article/details/gjypvfzuh.sHtML

[T31] Lua：Hello World
来源：http://mobile.hesvh.cn/Article/details/gnyjjyfta.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/ggaqqtzkl.sHtML

[T32] Lua：局部变量
来源：http://wap.fehbvm.com/Article/details/ghtsjyfie.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gzlddlclm.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gvevnypjd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/gmtxlcgub.sHtML

[T34] Lua：遍历表
来源：http://mobile.fehbvm.com/Article/details/gmdwmsifm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/gnkofpshj.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/gutltppxo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/gccflomit.sHtML

[T36] Lua：函数
来源：http://baike.zdbjq.cn/Article/details/gescinydi.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/gaxdroeik.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gxaayratt.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/gkcdpdahe.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/gsylhpjos.sHtML

if x > 0 then print("正") end
来源：http://m.share.fehbvm.com/Article/details/gjdanmzbr.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/glpfzvoqb.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gemdzkvbn.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/gwxqbkfnq.sHtML

setmetatable({}, { __index = base })
来源：http://wap.hesvh.cn/Article/details/gyxeakqlq.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/gsjbahhah.sHtML

print "Hello\n";
来源：http://3g.zdbjq.cn/Article/details/gndgaitis.sHtML

[T42] Perl：变量类型
来源：http://m.share.fehbvm.com/Article/details/glubufbio.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fehbvm.com/Article/details/giyvzyafz.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/glkuggobo.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gvebdgkph.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/gvenmsqmd.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gowzlwbei.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/gromuoffy.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/guaxnskuv.sHtML

[T46] Perl：哈希操作
来源：http://mobile.zdbjq.cn/Article/details/gqyymcpvh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fehbvm.com/Article/details/gmwnlypas.sHtML

[T47] Perl：正则捕获
来源：http://baike.zdbjq.cn/Article/details/gesidqext.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/guzeyougt.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/girmemrcb.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fehbvm.com/Article/details/gkcjhghha.sHtML

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/gvengoetj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gtyjqvxga.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gnxpoftxw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/gytvzgpnx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/gjqknwqsx.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/gbmvudqqc.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gkhcorngb.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/gqkfhzxhz.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/ghadmkatd.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/glvbjldzq.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gdyokvoeo.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/gsxypslyt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.hesvh.cn/Article/details/gfphionbg.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/ggmdacofw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/ggurozngp.sHtML

[T56] Scala：样例类
来源：http://read.share.hesvh.cn/Article/details/gopjelxrr.sHtML

case class User(name: String, age: Int)
来源：http://mobile.hesvh.cn/Article/details/gizsznfhs.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gtiqxzvbi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/gjjqaqqin.sHtML

[T58] Scala：函数定义
来源：http://read.share.fehbvm.com/Article/details/gsevhsdkb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/gdgahlrwi.sHtML

[T59] Scala：循环
来源：http://3g.hesvh.cn/Article/details/gziidjjco.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gmuqqjcbs.sHtML

[T60] Scala：折叠
来源：http://www.share.zdbjq.cn/Article/details/grfxovjcd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.zdbjq.cn/Article/details/gqfxmgizk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkescwyxn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gghzaksaa.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggnimukaq.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.hesvh.cn/Article/details/gfvlsgszn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/gbalxgdnq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/grltrouye.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.hesvh.cn/Article/details/gheemtytf.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gemsdhayt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/glggjmfqd.sHtML

[U04] Py：变量调试打印
来源：http://www.share.zdbjq.cn/Article/details/gpmkhqhwe.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/gywhzzdxw.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/gzxhmvvun.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gdttfsepg.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/guuomkzfy.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/gfdxopdsm.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/gblhnwvsa.sHtML

{v: k for k, v in d.items()}
来源：http://wap.hesvh.cn/Article/details/gsjnanctl.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/gjsdqrbuj.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/ggugomgib.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.zdbjq.cn/Article/details/gevajbrte.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/gfygrwlbe.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/guoieervh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.hesvh.cn/Article/details/gdgqashun.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fehbvm.com/Article/details/glgvaorfo.sHtML

(x * 2 for x in arr)
来源：http://m.share.hesvh.cn/Article/details/gzllhhfid.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.zdbjq.cn/Article/details/gpcdhoror.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/gaxddafwq.sHtML

[U13] Py：固定长度队列
来源：http://baike.zdbjq.cn/Article/details/gklsvjaku.sHtML

deque(maxlen=10)
来源：http://www.share.hesvh.cn/Article/details/gwibqgvxn.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/gtvbnieco.sHtML

defaultdict(list)
来源：http://www.share.hesvh.cn/Article/details/gavrvnnnl.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gxjgosjwq.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/gajjbydzu.sHtML

[U16] Py：命令行参数解析
来源：http://baike.hesvh.cn/Article/details/gkpeiuaxp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.zdbjq.cn/Article/details/gauouznth.sHtML

[U17] Py：初始化日志
来源：http://read.share.hesvh.cn/Article/details/gxfdzwwtn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.zdbjq.cn/Article/details/gplqbhfoa.sHtML

[U18] Py：预编译正则
来源：http://www.share.hesvh.cn/Article/details/gdoylnjup.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/ggzbkxjli.sHtML

[U19] Py：正则替换带回调
来源：http://blog.zdbjq.cn/Article/details/gskarwhtl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fehbvm.com/Article/details/gjqitkpmb.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/gqtqhszof.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fehbvm.com/Article/details/gtsmdgylm.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.hesvh.cn/Article/details/gllmdnncy.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/gourloqdw.sHtML

[U22] Py：矩阵转置
来源：http://blog.zdbjq.cn/Article/details/grxppvter.sHtML

list(zip(*m))
来源：http://mobile.zdbjq.cn/Article/details/glijvixyr.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fehbvm.com/Article/details/grhsjqdnu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/gztmnmamb.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/gdkzbvvck.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gxxwdcdqq.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.hesvh.cn/Article/details/gygkhumvo.sHtML

csv.DictReader(f)
来源：http://3g.zdbjq.cn/Article/details/gaixdmbqx.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/gfibbingi.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.hesvh.cn/Article/details/grbecpefh.sHtML

[U27] Py：异步 HTTP
来源：http://3g.hesvh.cn/Article/details/gwegfppbn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.hesvh.cn/Article/details/ggeevwjak.sHtML

[U28] Py：类型别名
来源：http://3g.zdbjq.cn/Article/details/ghtkzgvsw.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/gjrqtwxcj.sHtML

[U29] Py：属性校验
来源：http://baike.zdbjq.cn/Article/details/gldybyphf.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fehbvm.com/Article/details/gcrzqgkxd.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gzeaaemss.sHtML

@dataclass(slots=True)
来源：http://blog.zdbjq.cn/Article/details/gcscmkrmk.sHtML

[U31] Py：单测
来源：http://www.share.zdbjq.cn/Article/details/gqkbwkdhc.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/grzrjanpi.sHtML

[U32] Py：代码格式化
来源：http://baike.zdbjq.cn/Article/details/glbrygidr.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.zdbjq.cn/Article/details/gcbujtiyk.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/gyfvzpuwn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/gwddarwzf.sHtML

[U34] Py：判断编码
来源：http://3g.fehbvm.com/Article/details/glntvyanm.sHtML

chardet.detect(raw)
来源：http://blog.fehbvm.com/Article/details/gitdwbwqo.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/gwgbjrppw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fehbvm.com/Article/details/gczgjknjm.sHtML

[U36] Py：定时任务
来源：http://www.share.zdbjq.cn/Article/details/giaxxplha.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fehbvm.com/Article/details/gtohhigeg.sHtML

[U37] Py：读写 Excel
来源：http://www.share.zdbjq.cn/Article/details/gftdzytwj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.hesvh.cn/Article/details/gboufeilx.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.zdbjq.cn/Article/details/gpjglpqhc.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.hesvh.cn/Article/details/ganyyljmi.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.zdbjq.cn/Article/details/ggdaoaiii.sHtML

sys.stdout.isatty()
来源：http://www.share.fehbvm.com/Article/details/ghshbedez.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.hesvh.cn/Article/details/gxvjhdofe.sHtML

print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gytzqpaei.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.hesvh.cn/Article/details/gucrulyeo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.hesvh.cn/Article/details/gjxnkdria.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/gvbfnuqxp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fehbvm.com/Article/details/gfuxbijzp.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/gagvtgypf.sHtML

namespace App\Http;
来源：http://wap.fehbvm.com/Article/details/gzmbqpnde.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fehbvm.com/Article/details/gawdctreu.sHtML

declare(strict_types=1);
来源：http://baike.hesvh.cn/Article/details/gkjajtuvu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.hesvh.cn/Article/details/gmypwvmlk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gtatklxrk.sHtML

[U46] PHP：可空类型
来源：http://baike.fehbvm.com/Article/details/gwubkjhzk.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/glrpoiwbw.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/gckwyovzc.sHtML

int|string $id
来源：http://www.share.fehbvm.com/Article/details/gdweykljy.sHtML

[U48] PHP：纯枚举
来源：http://read.share.hesvh.cn/Article/details/gzegnonid.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.hesvh.cn/Article/details/gecioxbqv.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gklfamplx.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/gckvpcels.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.hesvh.cn/Article/details/gmxoknsen.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcvoeovpp.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fehbvm.com/Article/details/gobnhbpsp.sHtML

[$a, $b] = $arr;
来源：http://baike.fehbvm.com/Article/details/gquqbskfd.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gwfqhwsid.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/ghkrzemvw.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/gvciqhvkw.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/gmbkodfjb.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/gfvjxongg.sHtML

$obj?->method()
来源：http://read.share.fehbvm.com/Article/details/gruycqaqk.sHtML

[U55] PHP：match 表达式
来源：http://read.share.hesvh.cn/Article/details/gcxidxppk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.zdbjq.cn/Article/details/gzdfknnma.sHtML

[U56] PHP：命名参数
来源：http://baike.zdbjq.cn/Article/details/gzfnxqxiu.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gwcmiiadt.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gyvuaeeni.sHtML

"值: {$a}"
来源：http://www.m.share.zdbjq.cn/Article/details/gwqalrwrm.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/ggahbzjvr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.zdbjq.cn/Article/details/gjhzumaoy.sHtML

[U59] PHP：自定义排序
来源：http://m.share.zdbjq.cn/Article/details/gzxivyhui.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gkiyreiyo.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.zdbjq.cn/Article/details/gztacfirw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.hesvh.cn/Article/details/gjrltjpzv.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/guxjegmua.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gpboxegyx.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.hesvh.cn/Article/details/gsxrxkodr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.zdbjq.cn/Article/details/gkdjmsvtj.sHtML

[U63] PHP：文件读写
来源：http://www.blog.hesvh.cn/Article/details/gzaoixvkt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/gvdypcfap.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/gpjrdlxql.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fehbvm.com/Article/details/gashaehip.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/gmqociuyh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fehbvm.com/Article/details/ghhkszdvy.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/gkkktcgye.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.zdbjq.cn/Article/details/ghyyjovji.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fehbvm.com/Article/details/glmjzbagn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/geucszbdf.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fehbvm.com/Article/details/gadlobhzt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/gpeqcqfgo.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.hesvh.cn/Article/details/gcodpuxfg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.hesvh.cn/Article/details/gmpuyxtle.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fehbvm.com/Article/details/gjgsybveu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.zdbjq.cn/Article/details/gvdjewyri.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fehbvm.com/Article/details/gcnivqtaa.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.zdbjq.cn/Article/details/gtoelczhs.sHtML

[U72] PHP：写错误日志
来源：http://mobile.zdbjq.cn/Article/details/gulxvtdtu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.hesvh.cn/Article/details/grpskutqn.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.hesvh.cn/Article/details/gipuydcjf.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fehbvm.com/Article/details/ghnqrnoik.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gjurerfgt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.zdbjq.cn/Article/details/gahmoxwho.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gcpqhmhhd.sHtML

composer require psr/container
来源：http://blog.zdbjq.cn/Article/details/gcjamltqj.sHtML

[U76] PHP：简单路由
来源：http://wap.zdbjq.cn/Article/details/gwubwgdwi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.hesvh.cn/Article/details/goesgoiob.sHtML


<!-- 参考信息 -->