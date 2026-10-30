代发 wailian999

[S45] C++：lambda
来源：http://baike.fehbvm.com/Article/details/gkuewezhi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/ggkyleext.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/grqhbavma.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/ggqtuxmxe.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gizstquml.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/gyalvnvhi.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gtygbajiv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gmqbbjgay.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gzgxnqlhp.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gxeyyuyly.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/gzfraxvux.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gwundogsw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gbjxvighx.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gfppesxkf.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/gfbtqtoon.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gfxabvybr.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gonzajfms.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/gcthjtumb.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gjwbkqskt.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gdicpildz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.zdbjq.cn/Article/details/gcnvzrwkq.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gssixzffr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/glrxzuumv.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gmwbyhche.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/gcgiepjlc.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/gkdfmpgut.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gnrvdahvl.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/guduesuqh.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/glonounnf.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gimzjpivk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gqdqxzrra.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gzgrujqbh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gflahzohy.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmoeuygyw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gmlwuiubx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwdflpbzp.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gkovtnecu.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gaporgzlv.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/glmtgfldh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/ghkkzwnlq.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/gvocvtoyf.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/ginsfbujc.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gidufrrkc.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gslclfvdx.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/gyefqoaja.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gshhlwocw.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/glrehevlk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gntcettre.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gyrnsnash.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gqefqrgtj.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gvrrtnnoo.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gaiuogflm.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/gqfkhkfbv.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gvslyhxls.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/gdqvgwrph.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gjzrclbll.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/gzqvynxqi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/goacqunpf.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/gsyepbbwj.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gsiwlputs.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/goamrulux.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/ggoksppcc.sHtML

[T14] Kotlin：循环
来源：http://read.share.fehbvm.com/Article/details/gowylbqmi.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/gjlnxfago.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gywcmjpun.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gpeouahyo.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gqratbyyr.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gwgzrtfih.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/gekliyuwr.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/ggjiwcoat.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gzwrqwdjw.sHtML

"值: \(b)"
来源：http://mobile.fehbvm.com/Article/details/ghxzfdfcb.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gfxrdujqo.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/gaqraanrv.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/glqasavhp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.hesvh.cn/Article/details/gnnqwspqr.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/gdbamhswo.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/gymxxqdkj.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gytcigjgo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/ghryxozbx.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gzoekfgrf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gpjefltog.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gzocybcnt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gnixpqzuw.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gvtdbfnlo.sHtML

struct P { var x: Int }
来源：http://wap.fehbvm.com/Article/details/gowemakyf.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gxzdmheto.sHtML

class A: Base { override func f() {} }
来源：http://m.share.zdbjq.cn/Article/details/gqqtaawfc.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/gmwecvliv.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gptotfhow.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/geslggdcs.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gljxiwjcq.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gwcwcgyhn.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/gjgzzbfiu.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/gfhumwhxk.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/gpjewarvx.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/gvbzngbzz.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/glgkfsvzk.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/glzomhgql.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gjtyfshjx.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/gogfzgdmo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/gjauzbpej.sHtML

[T34] Lua：遍历表
来源：http://mobile.fehbvm.com/Article/details/gvysrsbag.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fehbvm.com/Article/details/gjoxtzjwv.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gggcsqhcg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fehbvm.com/Article/details/gmavalhma.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/gouskghou.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/greuacjmv.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/ggsjsnkmq.sHtML

"a" .. "b"
来源：http://www.m.share.hesvh.cn/Article/details/gdyqahokl.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/gjrhirwiq.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gxmxsqbrv.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gjmuvaqkx.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/gcbgicgfr.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/gcwuthhaz.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gofgjljhj.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gecigsnna.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/gqbehaqjy.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gwfoevuye.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/gfjlncfts.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/grsoocegh.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/grbqejulo.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/gtmvoxyao.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghvqetrwt.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/giihrgmkn.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/garrvhkji.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gqmogazbi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.zdbjq.cn/Article/details/gkrodcozb.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/gobnnixmm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gqyzixidu.sHtML

[T48] Perl：正则替换
来源：http://3g.fehbvm.com/Article/details/geyxrgkfi.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/gsbhryvig.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/grdzmupzi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gfznppeyl.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gugztyrlu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/gdwphocnn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.zdbjq.cn/Article/details/gxswxrrii.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/gzumwarpb.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/ggsgfwatq.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/gqubrlxnm.sHtML

val a = 1;  var b = 2
来源：http://read.share.hesvh.cn/Article/details/gsvfdeimw.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gqvhyhmeh.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gehvbugbj.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gljiemsae.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gisrpslhe.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gjotegbxe.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gxmpyndpj.sHtML

[T56] Scala：样例类
来源：http://read.share.hesvh.cn/Article/details/giyojvssv.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/grdpfbpjx.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/ggurhbhmv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.hesvh.cn/Article/details/ghejydout.sHtML

[T58] Scala：函数定义
来源：http://wap.zdbjq.cn/Article/details/gqxpclott.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fehbvm.com/Article/details/gasaiopwi.sHtML

[T59] Scala：循环
来源：http://www.share.zdbjq.cn/Article/details/gqpuedgnc.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gjuzxiisr.sHtML

[T60] Scala：折叠
来源：http://www.share.zdbjq.cn/Article/details/gglsnqlst.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/gsibkxfxt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzzwmkgrz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/glfoegjwf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsvkrgrnr.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/gjjhuivcs.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fehbvm.com/Article/details/ghanwlfwz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/gedvbpdxx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.zdbjq.cn/Article/details/gsgmettod.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/gxyrxmscn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.hesvh.cn/Article/details/gyszbyuoy.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fehbvm.com/Article/details/gaziywbph.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gwwhvmiyc.sHtML

[U05] Py：列表去重且保序
来源：http://blog.hesvh.cn/Article/details/gudyvyhlf.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gxwmsmeef.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gmajqdmuy.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/ggycdzfgf.sHtML

[U07] Py：反转字典键值
来源：http://m.share.hesvh.cn/Article/details/gbtkfiijc.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/gwmcjuynr.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.hesvh.cn/Article/details/gdqqehuug.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/gqocvlgjw.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.hesvh.cn/Article/details/gvtkilmwb.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gmvkhrmfk.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/gqovvzini.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/geimcdrcm.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/gzdkxdkkk.sHtML

(x * 2 for x in arr)
来源：http://blog.fehbvm.com/Article/details/ghzucenuc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.zdbjq.cn/Article/details/gdfonmwal.sHtML

Counter(arr).most_common(3)
来源：http://wap.fehbvm.com/Article/details/gmsxwtglg.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/gbdideytu.sHtML

deque(maxlen=10)
来源：http://blog.fehbvm.com/Article/details/gjuvykgan.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.zdbjq.cn/Article/details/gsfanqdui.sHtML

defaultdict(list)
来源：http://mobile.zdbjq.cn/Article/details/gbuodcvyj.sHtML

[U15] Py：高精度计时
来源：http://www.share.fehbvm.com/Article/details/gihhcgmxl.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/gbgdeqmlg.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/gctvsswfi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/gxezngogh.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gnpuzhfca.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/gqpmalcmc.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.zdbjq.cn/Article/details/gddfwgcxj.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fehbvm.com/Article/details/gfmwowgcy.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/gizftsxfk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/ggffqenhn.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/gdoxhjazo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/gpkihhpuy.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.hesvh.cn/Article/details/gvauitdeq.sHtML

@contextlib.contextmanager
来源：http://www.share.hesvh.cn/Article/details/gecgsedap.sHtML

[U22] Py：矩阵转置
来源：http://blog.zdbjq.cn/Article/details/grqfvxlkk.sHtML

list(zip(*m))
来源：http://m.share.fehbvm.com/Article/details/gcnvwiscj.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/gbrnvysoj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.hesvh.cn/Article/details/gtpjcjaqh.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/gihpbsxkk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gfwvxoxsi.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.hesvh.cn/Article/details/gepfebozw.sHtML

csv.DictReader(f)
来源：http://3g.hesvh.cn/Article/details/ggnaveuoo.sHtML

[U26] Py：并发下载
来源：http://m.share.fehbvm.com/Article/details/gipneqvnp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/gxtdcknbn.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/grolnrfmp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.hesvh.cn/Article/details/gvmkxaabh.sHtML

[U28] Py：类型别名
来源：http://www.share.hesvh.cn/Article/details/ghyexsdfh.sHtML

UserId = int
来源：http://baike.zdbjq.cn/Article/details/glgsucxcy.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fehbvm.com/Article/details/gpkhdtogo.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fehbvm.com/Article/details/ggayzbqsx.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gtcxxxuwh.sHtML

@dataclass(slots=True)
来源：http://baike.zdbjq.cn/Article/details/gukjydidb.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/gqktxdufk.sHtML

python -m pytest -q
来源：http://www.blog.fehbvm.com/Article/details/gtuipuihe.sHtML

[U32] Py：代码格式化
来源：http://www.share.hesvh.cn/Article/details/gdafjyhrx.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/gtecfkjwf.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/gmpdratvh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fehbvm.com/Article/details/gnfulubth.sHtML

[U34] Py：判断编码
来源：http://m.share.zdbjq.cn/Article/details/guftpaejp.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/gliumobyx.sHtML

[U35] Py：发送邮件
来源：http://3g.fehbvm.com/Article/details/gvuehebbk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/gnmlxxfkm.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/gunhklhej.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.zdbjq.cn/Article/details/getosoepl.sHtML

[U37] Py：读写 Excel
来源：http://www.share.hesvh.cn/Article/details/gkxzndrui.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.hesvh.cn/Article/details/ghgsdqbww.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.hesvh.cn/Article/details/gbinlrazd.sHtML

Path(__file__).resolve().parent
来源：http://blog.fehbvm.com/Article/details/gqgpwxupo.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/gtwuygbpn.sHtML

sys.stdout.isatty()
来源：http://mobile.hesvh.cn/Article/details/gyldqznev.sHtML

[U40] Py：打印到标准错误
来源：http://baike.hesvh.cn/Article/details/gumkbvrsv.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gifmhggsw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/ggibwogfy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.zdbjq.cn/Article/details/gquwhfixd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.zdbjq.cn/Article/details/gmmcznhse.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.zdbjq.cn/Article/details/grjhssava.sHtML

[U43] PHP：声明命名空间
来源：http://wap.hesvh.cn/Article/details/gkjioodbk.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/gqslghplp.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.hesvh.cn/Article/details/gioiljktc.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/gajvtcdhg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/gremlbdgl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gswvhczua.sHtML

[U46] PHP：可空类型
来源：http://baike.zdbjq.cn/Article/details/gfrziwaff.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/gcuklidvt.sHtML

[U47] PHP：联合类型
来源：http://baike.hesvh.cn/Article/details/gdereukzk.sHtML

int|string $id
来源：http://m.share.zdbjq.cn/Article/details/ggtwwapsq.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fehbvm.com/Article/details/gkiiovpbq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fehbvm.com/Article/details/gnmjdikds.sHtML

[U49] PHP：只读属性
来源：http://baike.zdbjq.cn/Article/details/gskcnsgck.sHtML

public readonly string $name
来源：http://www.m.share.hesvh.cn/Article/details/gmcmuoijk.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.zdbjq.cn/Article/details/gncrkgzuz.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.hesvh.cn/Article/details/gashfmmwc.sHtML

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/gvofwvgws.sHtML

[$a, $b] = $arr;
来源：http://mobile.hesvh.cn/Article/details/gnrcgsmxs.sHtML

[U52] PHP：箭头函数
来源：http://baike.fehbvm.com/Article/details/gbblbxtas.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.hesvh.cn/Article/details/gbiivxzme.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/girtehrlc.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/gdixeinqh.sHtML

[U54] PHP：空安全调用
来源：http://blog.zdbjq.cn/Article/details/grrylpyos.sHtML

$obj?->method()
来源：http://www.share.zdbjq.cn/Article/details/gndzakkck.sHtML

[U55] PHP：match 表达式
来源：http://www.share.zdbjq.cn/Article/details/grjzcevru.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gbrvgdhdf.sHtML

[U56] PHP：命名参数
来源：http://mobile.zdbjq.cn/Article/details/gidoumbgj.sHtML

f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gapzvqzfc.sHtML

[U57] PHP：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gqlarffku.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/giuixupwy.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fehbvm.com/Article/details/gxwrqaybc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.hesvh.cn/Article/details/gejvkzwlp.sHtML

[U59] PHP：自定义排序
来源：http://wap.zdbjq.cn/Article/details/ghexkabjf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gsmajmcmn.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/gqtditlub.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fehbvm.com/Article/details/gwukkhxra.sHtML

[U61] PHP：正则
来源：http://wap.hesvh.cn/Article/details/gznjigsnu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/girqdxzfu.sHtML

[U62] PHP：日期对象
来源：http://read.share.zdbjq.cn/Article/details/gmfelrgkc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.zdbjq.cn/Article/details/gvqenkmne.sHtML

[U63] PHP：文件读写
来源：http://blog.hesvh.cn/Article/details/gixwbgbnf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fehbvm.com/Article/details/gnlbimxzw.sHtML

[U64] PHP：目录遍历
来源：http://wap.hesvh.cn/Article/details/gguelamkw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fehbvm.com/Article/details/gidsbedqx.sHtML

[U65] PHP：会话
来源：http://www.share.zdbjq.cn/Article/details/gostzwikt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/ghrzzwmla.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fehbvm.com/Article/details/gpvpfichb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fehbvm.com/Article/details/gbwbvozzi.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.zdbjq.cn/Article/details/gmgzhghox.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.zdbjq.cn/Article/details/gfvusecuj.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fehbvm.com/Article/details/gpbsaknua.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.hesvh.cn/Article/details/gbxidbtii.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fehbvm.com/Article/details/gstnjxksv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/gncgpxyaq.sHtML

[U70] PHP：PDO 事务
来源：http://baike.zdbjq.cn/Article/details/gchuhzxwo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.hesvh.cn/Article/details/gkmigatvh.sHtML


<!-- 参考信息 -->