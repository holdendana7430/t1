代发 wailian999

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gorkmxgdh.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytnzuitd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gmzgaqqmi.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpmvuade.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gnvtinjio.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/goqtbiuqq.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gecefqcsa.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdrniapq.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbladwbul.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbqvwhmx.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/ghdeddomv.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtofjoac.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/grmgmugdn.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkgdwlnn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gehqesxno.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gaejlydqe.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/giwmvspqf.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gtltwucrv.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnceuyqff.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkkyyjhk.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrdzrowo.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gkihdkaea.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/geegghnip.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhqtimod.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/glupwselx.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gtvaasorn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gmvqrzrsr.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gjoirbxok.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsiqhcdc.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvirwbzz.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gfyvthwfe.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstjtdtgp.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gtlivcmty.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gqfvngqbt.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/gzjrsadsm.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrklfniu.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrxkamvn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gbljozuju.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gtgxgneyx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwislolz.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuffshqj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaokajpqg.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/girkmyhjo.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhebtbfa.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gdltymsvy.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/guskdwquc.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gtuwqsswv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnxofxdz.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkmhuicc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkiwtwzt.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxmdzdax.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbhevzut.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gdaiupgjx.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfekzvizt.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/geppbqhyq.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfahywew.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvyqkify.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gxzjkapeh.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyaiwvpu.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gbevrvgnu.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gkglwvcow.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gdxqmvhss.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnwkwpwm.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gaktoqoix.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjpdhled.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghobdghon.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gseoeqkyo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gggitihlt.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpevzzri.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gvdmnjysd.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gqinrquas.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gghtaxszr.sHtML

[T23] Swift：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuijbmlp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gswvyfmyg.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxpectzi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gzysylhui.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gmukipcbg.sHtML

struct P { var x: Int }
来源：http://m.share.fanxiaobao.xyz/Article/details/gswtcfjed.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/gbdgtkooj.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gifgadpop.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/geesfggqj.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gojhmnrej.sHtML

[T28] Swift：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gqumsjsdw.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdgdmfxh.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/gbrnjwtnq.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhmdmwpe.sHtML

[T30] Swift：协议
来源：http://blog.fanxiaobao.xyz/Article/details/gylfuucwx.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gcxrnctna.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gbtahtkka.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtluyxsew.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gzjtrgayu.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gboossbrq.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gjctnnncs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdheojed.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/gqunsontn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/gdsecfwke.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/gsolxumwy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdlgukey.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxoasjdom.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gmblglqmg.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvzhtily.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gyrjufjcr.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhaalinp.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbhoxuec.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdgzdcep.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gpohcbtiz.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtunfcdfn.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/gisbcxvph.sHtML

[T41] Perl：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfjxdtnt.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gcedikais.sHtML

[T42] Perl：变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdsquykh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvnyqryi.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gyflfzwmn.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/govkhsqoh.sHtML

[T44] Perl：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdctidlxu.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gempdshsw.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrajvqzr.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzuqvtqxh.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gaedrcxjl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gaxldapfn.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/gkhktajpo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjokiacoh.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gysbqqaxk.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gughnneaf.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcneievp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbuhhqoin.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjognbgh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlywxndz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfaggvhax.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/ghzrshbii.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gcnymvkip.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gkkllelbb.sHtML

val a = 1;  var b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxioolmc.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyogeyecv.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/glimisqrp.sHtML

[T54] Scala：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/goobnnrur.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gtfxvgdvt.sHtML

[T55] Scala：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/guskuwyrs.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gnogmdump.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/gprpvvddq.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gkayryywn.sHtML

[T57] Scala：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gqzdlmyrw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fanxiaobao.xyz/Article/details/glvurowxg.sHtML

[T58] Scala：函数定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gobfslovc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gwddsjenn.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gpxxmtuba.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/goscklzsq.sHtML

[T60] Scala：折叠
来源：http://wap.fanxiaobao.xyz/Article/details/geqafdrql.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fanxiaobao.xyz/Article/details/gxqbrdmso.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gtigodduh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/glacdaoeo.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gbazvtzyl.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkcdxxnj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fanxiaobao.xyz/Article/details/gxixthsic.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/gzbqpwppx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fanxiaobao.xyz/Article/details/goomdwiij.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gwveltgey.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/gmrnemzir.sHtML

[U04] Py：变量调试打印
来源：http://3g.fanxiaobao.xyz/Article/details/gnfvveeak.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvediaym.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidfrzpih.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqqtydwq.sHtML

[U06] Py：合并两个字典
来源：http://wap.fanxiaobao.xyz/Article/details/gbjptnlcl.sHtML

{**a, **b}
来源：http://3g.fanxiaobao.xyz/Article/details/gbnksuqij.sHtML

[U07] Py：反转字典键值
来源：http://3g.fanxiaobao.xyz/Article/details/gfujsmvdo.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhcxseom.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisqivtws.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/gbncwlmhs.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fanxiaobao.xyz/Article/details/gupnzpkmr.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/gcjizsvru.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrbvcsgo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fanxiaobao.xyz/Article/details/ghwonexjd.sHtML

[U11] Py：生成器表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gvuyhmrcx.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxznvpght.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqfxupqk.sHtML

Counter(arr).most_common(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gyeowfybc.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gzezbtpbt.sHtML

deque(maxlen=10)
来源：http://blog.fanxiaobao.xyz/Article/details/gzdmmjcmq.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gjemxmcxk.sHtML

defaultdict(list)
来源：http://mobile.fanxiaobao.xyz/Article/details/grmcyjrlk.sHtML

[U15] Py：高精度计时
来源：http://read.share.fanxiaobao.xyz/Article/details/gvndtxdjr.sHtML

t = time.perf_counter()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpllhdbrc.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqquwzkhr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmcnoiap.sHtML

[U17] Py：初始化日志
来源：http://baike.fanxiaobao.xyz/Article/details/gepgxuvbr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/ggndkrvxs.sHtML

[U18] Py：预编译正则
来源：http://blog.fanxiaobao.xyz/Article/details/gbttgawqq.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxztvxuu.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpkpojxy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fanxiaobao.xyz/Article/details/gxwipfigo.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpvpkzem.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fanxiaobao.xyz/Article/details/gcbgrhawb.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fanxiaobao.xyz/Article/details/gsgtwixgd.sHtML

@contextlib.contextmanager
来源：http://wap.fanxiaobao.xyz/Article/details/glbgpcxgn.sHtML

[U22] Py：矩阵转置
来源：http://wap.fanxiaobao.xyz/Article/details/gkgysktvr.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/gubdcdecz.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdltvrev.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/ggarsyfjf.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gjstmpsmt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwtewftm.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqykeoyu.sHtML

csv.DictReader(f)
来源：http://wap.fanxiaobao.xyz/Article/details/gnzxexeek.sHtML

[U26] Py：并发下载
来源：http://3g.fanxiaobao.xyz/Article/details/gkuvecgcq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudruqhsx.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/gxnzgmxzu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgszhtbs.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/ghbhoduna.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/gxcufgkvm.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/glfdpzjvu.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fanxiaobao.xyz/Article/details/glaunkkwn.sHtML

[U30] Py：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnsnzlnp.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhjmrbza.sHtML

[U31] Py：单测
来源：http://www.share.fanxiaobao.xyz/Article/details/gqppeitre.sHtML

python -m pytest -q
来源：http://www.blog.fanxiaobao.xyz/Article/details/goncuthyw.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gtytfcmzm.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fanxiaobao.xyz/Article/details/gocvikekp.sHtML

[U33] Py：打包发布
来源：http://www.share.fanxiaobao.xyz/Article/details/gxaeeepwr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fanxiaobao.xyz/Article/details/gfdadcslj.sHtML

[U34] Py：判断编码
来源：http://baike.fanxiaobao.xyz/Article/details/gahujqtzo.sHtML

chardet.detect(raw)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcszfipii.sHtML

[U35] Py：发送邮件
来源：http://m.share.fanxiaobao.xyz/Article/details/gcebfhybu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fanxiaobao.xyz/Article/details/glnqjcjvf.sHtML

[U36] Py：定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/grpvvnofs.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyqelprl.sHtML

[U37] Py：读写 Excel
来源：http://baike.fanxiaobao.xyz/Article/details/gqydfmrkj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkcfpuiu.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gleeabamu.sHtML

Path(__file__).resolve().parent
来源：http://baike.fanxiaobao.xyz/Article/details/gfdnovktk.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fanxiaobao.xyz/Article/details/giqjbahdk.sHtML

sys.stdout.isatty()
来源：http://baike.fanxiaobao.xyz/Article/details/gpvghldok.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fanxiaobao.xyz/Article/details/gwivhvgpq.sHtML

print("err", file=sys.stderr)
来源：http://blog.fanxiaobao.xyz/Article/details/gubkcydan.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxyaywam.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmabumdgb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcyobvvd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fanxiaobao.xyz/Article/details/gluayjfor.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqhjmglh.sHtML

namespace App\Http;
来源：http://wap.fanxiaobao.xyz/Article/details/gtfzlflzl.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fanxiaobao.xyz/Article/details/gjopwjrfc.sHtML

declare(strict_types=1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtoyxayc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fanxiaobao.xyz/Article/details/gxbjakzzc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gejrnsizw.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkaxuzju.sHtML

?string $name = null
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwgeacsl.sHtML

[U47] PHP：联合类型
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxfluyrr.sHtML

int|string $id
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkfizsoq.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gggrrhezw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkabygdg.sHtML

[U49] PHP：只读属性
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcvyzznc.sHtML

public readonly string $name
来源：http://wap.fanxiaobao.xyz/Article/details/gnugzmhya.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fanxiaobao.xyz/Article/details/gfuongkna.sHtML

public function __construct(private int $id) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gqkueuljq.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnlkmzgx.sHtML

[$a, $b] = $arr;
来源：http://wap.fanxiaobao.xyz/Article/details/ghseomllg.sHtML

[U52] PHP：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gcueggzos.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gokayvdhg.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwrjxscf.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fanxiaobao.xyz/Article/details/gkimklyau.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjwngxaz.sHtML

$obj?->method()
来源：http://wap.fanxiaobao.xyz/Article/details/gbhyyaaus.sHtML

[U55] PHP：match 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gqswizzcj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fanxiaobao.xyz/Article/details/gjrmylmpo.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwkkigbp.sHtML

f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/godavooqi.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshdghgvb.sHtML

"值: {$a}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjrgfhtx.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fanxiaobao.xyz/Article/details/guiehghsn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/ghpnvbasy.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuwzuwea.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtytrlgbl.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggudvnluw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fanxiaobao.xyz/Article/details/glxxkseto.sHtML

[U61] PHP：正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gzscjhory.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/grgzlmpzv.sHtML

[U62] PHP：日期对象
来源：http://blog.fanxiaobao.xyz/Article/details/gqcdpbjgg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnnkhjso.sHtML

[U63] PHP：文件读写
来源：http://baike.fanxiaobao.xyz/Article/details/gkdoshmqm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfubommfc.sHtML

[U64] PHP：目录遍历
来源：http://blog.fanxiaobao.xyz/Article/details/ggtcqrulk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fanxiaobao.xyz/Article/details/gytsolmtx.sHtML

[U65] PHP：会话
来源：http://blog.fanxiaobao.xyz/Article/details/ghskemwak.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gxxfjbvxb.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhsknqib.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghiqulhnj.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fanxiaobao.xyz/Article/details/gehvfxbbc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fanxiaobao.xyz/Article/details/gnxadgbcf.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fanxiaobao.xyz/Article/details/gqclndmoq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fanxiaobao.xyz/Article/details/giwzfjlqx.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfnqyzir.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fanxiaobao.xyz/Article/details/gkyjuouys.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fanxiaobao.xyz/Article/details/gkhiirruw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fanxiaobao.xyz/Article/details/glonpzgwc.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gweyumwgb.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxbceael.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcdjjxks.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fanxiaobao.xyz/Article/details/guuekfxum.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fanxiaobao.xyz/Article/details/glmxquace.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fanxiaobao.xyz/Article/details/gdioykioq.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxqnoorv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fanxiaobao.xyz/Article/details/gyzrvtage.sHtML


<!-- 参考信息 -->