代发 wailian999

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gifkabjzz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/giotdesaw.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gkyfgxuqv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gdzkouocg.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gwgusbyos.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gvydgwrzl.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gnopgldcb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gahempkwp.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gmcaijabx.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gjstazbfg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gpiiipkvn.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gxopecbig.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gtpettmfo.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/gkzftrcav.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/gbkjkodxi.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/ghpnxkquk.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gxvsoyvbm.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gpdogsydg.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/glgimmpuu.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/gqzeoptry.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gkqdfazvg.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/gzvwnfaec.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gtngkmrsd.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gelxrhovo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/ggtaajfwa.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gbrmntcwa.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gbehbkqvq.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gcxcjbhtc.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gxgijizat.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gxpkkanrf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gbkthlgun.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gmdqsqzku.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/glytdumse.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwgjfzuzr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gmgbipwhc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/getxygige.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/ghcwzysle.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gqtgdvcdk.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gmxhjnwwu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/grqjuhncg.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gqvwalypj.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/grmthizze.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gyajtqfnx.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/gdacrgsai.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/gzwhhehhq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gqrajomsq.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gwoztqsau.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gqrpgwrlo.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/guiahugns.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gxottfxyx.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gmnnmqkjx.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/grctcoqmd.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gifuqolzi.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gzepkrful.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/getzejmmy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/ggykbmwiy.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gllpvdnjf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/ggglrevti.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gjwvksnpn.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gbrshbcdc.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/gijlamawo.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gkavnwxjy.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gzcpwcsbi.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gvyvucelj.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gkhldufzs.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/gqocvxqzv.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/glcrcowmb.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/govprhqqw.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/goytwehzp.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/gxbnfpxcs.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gpohikodc.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/gupvzdfqt.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/gwqomsddr.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gdjyasspi.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/gemushnvg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gkyrfmysp.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/gwetsleve.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/guyusmosw.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/ggyszarae.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/gnpmqoloc.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/gvldcnght.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/gegnykbjx.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gihksnsrt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/gbcvnopfc.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/glupextca.sHtML

struct P { var x: Int }
来源：http://mobile.hesvh.cn/Article/details/gkghtenzo.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/gjxgndraz.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gmmlqekmq.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gzeugldwq.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gugzzhmbw.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/gjgygbvkb.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/golatiawi.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/gvgprwmhk.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gjfgruswc.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/ghamjwrhd.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gqyobappc.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/ghowgvyso.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gklrdjuxj.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/gerjioicq.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/grdvbhroz.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/gbciujwro.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gsihtoxhb.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/ggtrhozfn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/gayuxuvgr.sHtML

[T35] Lua：字典表
来源：http://m.share.hesvh.cn/Article/details/gkpwixchv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/gbnavvyne.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/glgtiiwbz.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/gsyutuzma.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gxucvdfqu.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/gmvmzwxne.sHtML

[T38] Lua：条件
来源：http://www.blog.zdbjq.cn/Article/details/gahrqrsab.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/giwsyqsrz.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/glahdodhs.sHtML

string.find(s, "%d+")
来源：http://m.share.hesvh.cn/Article/details/grmfvhehk.sHtML

[T40] Lua：元表
来源：http://wap.hesvh.cn/Article/details/gcbgjuyzd.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/gtkfuhdmo.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gcmftxbli.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gwlzpoyrd.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/glqlcxqnx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/gsbueytob.sHtML

[T43] Perl：字符串插值
来源：http://wap.zdbjq.cn/Article/details/goigizojv.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/gynjmdxiw.sHtML

[T44] Perl：条件
来源：http://mobile.fehbvm.com/Article/details/gubfpaipz.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/gtqswzckx.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.zdbjq.cn/Article/details/gkefzjlqd.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.hesvh.cn/Article/details/galysqccm.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gfreixbmq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/grsvedigr.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/gbznofule.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fehbvm.com/Article/details/gnwcpznht.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/gihkoeifa.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gnindeurc.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/gjjshamie.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gjykyjdnd.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gnwlxeqlt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/gvcragdjj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvcxhaait.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/guwavlunr.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gjtfbnacw.sHtML

[T52] Scala：变量
来源：http://www.share.zdbjq.cn/Article/details/gadwysezl.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/gwyroqfvn.sHtML

[T53] Scala：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gzvrtjgho.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/ggcbajwgp.sHtML

[T54] Scala：集合映射
来源：http://baike.hesvh.cn/Article/details/gbzzebjdn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/gtqhsbjnx.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/giegwyiep.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/gliafdjng.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/gpuqgahfg.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/gqaxpvhxy.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gcwzkyxws.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/gxhcsermv.sHtML

[T58] Scala：函数定义
来源：http://mobile.fehbvm.com/Article/details/gdlubcneo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gdfbdwfwp.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/giglhqcoe.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/gsgpihvqo.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fehbvm.com/Article/details/gumwuaagm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/ggxppugcv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/givtkixua.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gkregbden.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkkpvuovl.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.hesvh.cn/Article/details/gxpjpoqho.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/gsifrlxqn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/gyivbmklw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.hesvh.cn/Article/details/gcdokgcvr.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/gvkzribfd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/gpefycfvj.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/gurwuqqxf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/givxaxyhj.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/gqowsgkps.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gyhafaxvz.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/gxwnibqwa.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/gdcscbbxy.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/gshfuysyo.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/gqqudokky.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/gmhydsvom.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/gakzsirkm.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.zdbjq.cn/Article/details/gyoduegfv.sHtML

max(d, key=d.get)
来源：http://wap.fehbvm.com/Article/details/gdjlzfyix.sHtML

[U10] Py：按值排序字典
来源：http://m.share.zdbjq.cn/Article/details/gmfuyhhew.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/gwfgkpkox.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/gywcmvjxt.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gyfrddcnn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/grkpzxqqe.sHtML

Counter(arr).most_common(3)
来源：http://blog.fehbvm.com/Article/details/gbiivuurx.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/gzdhxkwut.sHtML

deque(maxlen=10)
来源：http://wap.fehbvm.com/Article/details/gbttuhsbm.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/gsprbnuul.sHtML

defaultdict(list)
来源：http://www.blog.hesvh.cn/Article/details/glrjwsxfz.sHtML

[U15] Py：高精度计时
来源：http://m.share.zdbjq.cn/Article/details/gxmrgtijx.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gbhpeeuhp.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.zdbjq.cn/Article/details/gbgiuctie.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.zdbjq.cn/Article/details/gtefvxcjc.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/gicwolybw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/gcksgamuz.sHtML

[U18] Py：预编译正则
来源：http://read.share.fehbvm.com/Article/details/gcubbrgxa.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/gsbdtyzbu.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.hesvh.cn/Article/details/gnmlnffln.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.hesvh.cn/Article/details/gksdmoixs.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fehbvm.com/Article/details/glkrecwjr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/gvbyjkljw.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/gkvqbmplr.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/gsngyuwja.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/gnhsglnbj.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/gcjseupar.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/gnmpbcxha.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.hesvh.cn/Article/details/gqrvdwflj.sHtML

[U24] Py：路径操作
来源：http://m.share.hesvh.cn/Article/details/gzggcwkkd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gxcfwmwbn.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.zdbjq.cn/Article/details/gubgmnuyq.sHtML

csv.DictReader(f)
来源：http://blog.hesvh.cn/Article/details/gmycxrvyr.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/gikyxqsso.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.zdbjq.cn/Article/details/ghoshzlsc.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.hesvh.cn/Article/details/gxouelenq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/garccqdkz.sHtML

[U28] Py：类型别名
来源：http://m.share.fehbvm.com/Article/details/gxgdpxwdu.sHtML

UserId = int
来源：http://read.share.hesvh.cn/Article/details/ggjcbinvg.sHtML

[U29] Py：属性校验
来源：http://read.share.fehbvm.com/Article/details/gyiqhvkba.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gsyupiqkl.sHtML

[U30] Py：数据类
来源：http://read.share.hesvh.cn/Article/details/guhlngpqw.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gwpjjveif.sHtML

[U31] Py：单测
来源：http://read.share.fehbvm.com/Article/details/gnvvsrsrz.sHtML

python -m pytest -q
来源：http://www.share.fehbvm.com/Article/details/gvkkvyjzw.sHtML

[U32] Py：代码格式化
来源：http://3g.hesvh.cn/Article/details/gdwrzwsgb.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fehbvm.com/Article/details/gepyjddfo.sHtML

[U33] Py：打包发布
来源：http://baike.hesvh.cn/Article/details/gjtyobstc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fehbvm.com/Article/details/gztqtfzsu.sHtML

[U34] Py：判断编码
来源：http://3g.zdbjq.cn/Article/details/ghrhuryjh.sHtML

chardet.detect(raw)
来源：http://www.m.share.hesvh.cn/Article/details/gjoyerehv.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.hesvh.cn/Article/details/garfnkgri.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fehbvm.com/Article/details/gyxfpacaz.sHtML

[U36] Py：定时任务
来源：http://www.share.zdbjq.cn/Article/details/gvcsnhwbm.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.hesvh.cn/Article/details/grjjajjdt.sHtML

[U37] Py：读写 Excel
来源：http://www.share.hesvh.cn/Article/details/garqbpgpc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/gscqgwdyg.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fehbvm.com/Article/details/gwsyfpnnt.sHtML

Path(__file__).resolve().parent
来源：http://m.share.zdbjq.cn/Article/details/gvpvseyef.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fehbvm.com/Article/details/gghgzlvdq.sHtML

sys.stdout.isatty()
来源：http://blog.zdbjq.cn/Article/details/gwovbkbka.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/gxzdwbkty.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gaculkjym.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.hesvh.cn/Article/details/gxlzvwtsq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fehbvm.com/Article/details/gdxkndjni.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.hesvh.cn/Article/details/gtbivtmfe.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.hesvh.cn/Article/details/gdxgaawvn.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/gfywzijoo.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gneqtdyvy.sHtML

[U44] PHP：开启严格类型
来源：http://blog.zdbjq.cn/Article/details/gumkpykdu.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/gjkhnheba.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/ghvjnkqkf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gjcqnendm.sHtML

[U46] PHP：可空类型
来源：http://wap.fehbvm.com/Article/details/gxzkekqza.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/gpodzjxks.sHtML

[U47] PHP：联合类型
来源：http://read.share.zdbjq.cn/Article/details/geypovrws.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/gfmnythwc.sHtML

[U48] PHP：纯枚举
来源：http://mobile.zdbjq.cn/Article/details/ghhsrzbzm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.zdbjq.cn/Article/details/grxffshou.sHtML

[U49] PHP：只读属性
来源：http://blog.zdbjq.cn/Article/details/gvchkotnx.sHtML

public readonly string $name
来源：http://wap.fehbvm.com/Article/details/gegxpcwbf.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.hesvh.cn/Article/details/gsbzycyez.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fehbvm.com/Article/details/gpsowaody.sHtML

[U51] PHP：数组解构
来源：http://m.share.fehbvm.com/Article/details/gcxjqblvc.sHtML

[$a, $b] = $arr;
来源：http://mobile.fehbvm.com/Article/details/gpjfqixbq.sHtML

[U52] PHP：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gngpeqfil.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/grzhigubm.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.zdbjq.cn/Article/details/gvxqlfeya.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fehbvm.com/Article/details/gzckgzmri.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fehbvm.com/Article/details/gygoecieh.sHtML

$obj?->method()
来源：http://blog.zdbjq.cn/Article/details/guxzuvjpg.sHtML

[U55] PHP：match 表达式
来源：http://mobile.zdbjq.cn/Article/details/gsidxszil.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/grtkyvjti.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/gaswihwli.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/ghinxqbtq.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/gvnwivrbj.sHtML

"值: {$a}"
来源：http://baike.hesvh.cn/Article/details/geivpdurn.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/gvxaoyepn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fehbvm.com/Article/details/gjwdqrkxx.sHtML

[U59] PHP：自定义排序
来源：http://www.share.hesvh.cn/Article/details/gtyxiriki.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/godmolwrn.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fehbvm.com/Article/details/gnmozubzq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.zdbjq.cn/Article/details/gstrxhscq.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/gelylztbb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gzeezlpyr.sHtML

[U62] PHP：日期对象
来源：http://3g.zdbjq.cn/Article/details/gurjmcxqw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fehbvm.com/Article/details/gfsgmspln.sHtML

[U63] PHP：文件读写
来源：http://read.share.hesvh.cn/Article/details/ggvkgaxws.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.zdbjq.cn/Article/details/gcubdrqct.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/gupefregw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/gsshugdix.sHtML

[U65] PHP：会话
来源：http://www.blog.zdbjq.cn/Article/details/gvdfxjlrs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gafyxbqsm.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.hesvh.cn/Article/details/gfjhccpai.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fehbvm.com/Article/details/gjtfleerl.sHtML

[U67] PHP：处理文件上传
来源：http://wap.zdbjq.cn/Article/details/ggyknmzds.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.zdbjq.cn/Article/details/ggqaeguiu.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/gwmotcfii.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fehbvm.com/Article/details/gkudeazym.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.hesvh.cn/Article/details/gzolijsrs.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.hesvh.cn/Article/details/gbcprsait.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/gzwdfjctz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.hesvh.cn/Article/details/ggqrmyddr.sHtML


<!-- 参考信息 -->