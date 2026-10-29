代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gxgchrcrn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gjpqfibja.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gnqaeaolw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gybhlqtnv.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/ghwxoqnec.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/ggfnvhgvj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gitbefqvb.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gskdzafjz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gzbeuipnx.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gplzwgtpi.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gfbgvjfdy.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/guznbxzhe.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/gycoytxnd.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/grvdgcomf.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gqqgtnkah.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gqmwbugyp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/galdcmkga.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gqoaezzdd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gaajbzrgq.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/gpjfkkezj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/grofflltl.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/gxfegqxhg.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gkruhmjyu.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gkokbwqrq.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gjbtzoevf.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gocbocrry.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gjfxazbuy.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/gtbrvjrfn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/grjjkdxgf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjvecvkno.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gevffrdzk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gchemywgd.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gipgafwdx.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gbgddopka.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gkfojzfwd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/guizexbad.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/ghdtkuotv.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gtpldckja.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/gsalazrox.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/gyayhgwfk.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gbiydzyeg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gdamdqvvu.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/ghvspbwmo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gwovjeaxo.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gzgeyvucs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gbhoosors.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gipbijeki.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/ggengrjef.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gydcmnjab.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gnesbesba.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/gugeeivgj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gyjrkwnfh.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gbpwfuivu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/gqhpldnjf.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gyvvihkqd.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gsenkrkzp.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/gxewgchoo.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/gpvnnnvmm.sHtML

[T14] Kotlin：循环
来源：http://blog.zdbjq.cn/Article/details/ghxlsunct.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/gokgpdddb.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gcijzsclm.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/giyifdmhc.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gsmcjyakm.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gsdwvprpx.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gbkwxorpm.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/gddjrjvmd.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/glnbvnbom.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/ggzgvjftt.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/grosyolzz.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gwkiuunio.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/ggufeoqah.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/gkuoahako.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gofjrwmdp.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/gsihnvpgd.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gbbutcbyc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gcwabrtcz.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gzksapevt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/gopqwknlk.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/ghhpjhsqz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gvwgjejpr.sHtML

[T25] Swift：结构体
来源：http://wap.zdbjq.cn/Article/details/gwcueefmd.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gncdsrfyu.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gwixglxpt.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.hesvh.cn/Article/details/gqfeafvgu.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gfsskppdo.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/gttdmksxp.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/gawkwuqmy.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/geuwlsspl.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/gtbyweobl.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gqcdfxmwb.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gmrbkaiwo.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gtqsylerb.sHtML

[T31] Lua：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gsiwnjbqq.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gqpxzhrea.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gnkclntut.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/gvpxtasym.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/gaqrzneej.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/ggyfveclv.sHtML

[T34] Lua：遍历表
来源：http://www.share.hesvh.cn/Article/details/gfrrylfjd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.zdbjq.cn/Article/details/gexsvouom.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gikkpscin.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fehbvm.com/Article/details/glcyhtzzh.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/gfrekjnqn.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/ghkpqswmp.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gntwylood.sHtML

"a" .. "b"
来源：http://www.m.share.zdbjq.cn/Article/details/gehazhwcv.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/grkeulbvd.sHtML

if x > 0 then print("正") end
来源：http://m.share.zdbjq.cn/Article/details/gvxgjwhxg.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/ghfcmfxxq.sHtML

string.find(s, "%d+")
来源：http://m.share.zdbjq.cn/Article/details/gbihovtaq.sHtML

[T40] Lua：元表
来源：http://3g.zdbjq.cn/Article/details/gmajzoxfb.sHtML

setmetatable({}, { __index = base })
来源：http://blog.hesvh.cn/Article/details/gcthhupnu.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/gvtfduevm.sHtML

print "Hello\n";
来源：http://mobile.fehbvm.com/Article/details/gomicapts.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gtdbuujae.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/gcgacegvi.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/ghmedflyp.sHtML

"值: $a"
来源：http://www.blog.hesvh.cn/Article/details/gwixmwxgk.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/gwtakejrt.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.hesvh.cn/Article/details/gokbpvdvm.sHtML

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/gwkgvzkmo.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/gdejjykok.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/giubyjial.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.hesvh.cn/Article/details/gmegvgqeu.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/ghhsprauk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/gztbdwlsa.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/gcoqzrbwi.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gzmajouux.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/gpgpmlgfs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gwcgnbnhe.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gmkqiyudc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/gxapmyyto.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/gdazbaino.sHtML

[T51] Scala：Hello World
来源：http://blog.hesvh.cn/Article/details/gtkuoahcw.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gshqyitmq.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/gmtugqccu.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/ggnarprwt.sHtML

[T53] Scala：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gfgcdiuso.sHtML

s"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gchpjyqvf.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/ghodtyfyw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.zdbjq.cn/Article/details/goegzgpek.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gyyzqcdst.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.hesvh.cn/Article/details/gawguyduv.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/gbwlfxscl.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/gayhmsbzg.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gbikwblzb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gtqqkabpm.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/gxwmongsp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.hesvh.cn/Article/details/ghyrrqddl.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/golzxmdea.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/gemfcggcx.sHtML

[T60] Scala：折叠
来源：http://www.blog.zdbjq.cn/Article/details/gltnxdcpp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fehbvm.com/Article/details/gtolseytk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcdwvpaje.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gyohxyjsu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsjahrmyt.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gquhwpkmc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/glrbuuqzp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/gihhpmqsv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gqzsipfdr.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fehbvm.com/Article/details/gneyybgdd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gludumqsj.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.zdbjq.cn/Article/details/guzwwczcn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gsmzrtazx.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/glbmhrfmn.sHtML

list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gszecoahi.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/gzzxgmpsp.sHtML

{**a, **b}
来源：http://m.share.hesvh.cn/Article/details/gtvoacleq.sHtML

[U07] Py：反转字典键值
来源：http://baike.zdbjq.cn/Article/details/gfnvuyeeq.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/gyecqestk.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gvidjblyj.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/grhegtedh.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.zdbjq.cn/Article/details/gqpscbcem.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/guuqfmjjd.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.hesvh.cn/Article/details/gessqlzhe.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gzibkyoek.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fehbvm.com/Article/details/gynradhbw.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gztrjxctt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/gszvavvlr.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/glshhxcwb.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/gclbksqxc.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gmdjcraue.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/grpyqgfdm.sHtML

defaultdict(list)
来源：http://m.share.fehbvm.com/Article/details/gbayyvfpv.sHtML

[U15] Py：高精度计时
来源：http://baike.zdbjq.cn/Article/details/gydtoyldf.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/gbcsvnxqk.sHtML

[U16] Py：命令行参数解析
来源：http://baike.zdbjq.cn/Article/details/gvetxkcjc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/ghniowuqg.sHtML

[U17] Py：初始化日志
来源：http://read.share.hesvh.cn/Article/details/gmuhpaivl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.zdbjq.cn/Article/details/gqylvjwjs.sHtML

[U18] Py：预编译正则
来源：http://3g.hesvh.cn/Article/details/gresqvaij.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gjdjstrfp.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gfvgvhsbi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/gxooxkkle.sHtML

[U20] Py：缓存函数结果
来源：http://baike.zdbjq.cn/Article/details/gjkbdrynw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.hesvh.cn/Article/details/grufkdmou.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.hesvh.cn/Article/details/gvsraaytn.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fehbvm.com/Article/details/gzklnxccj.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/gihyjrqqz.sHtML

list(zip(*m))
来源：http://mobile.zdbjq.cn/Article/details/gatkmaphp.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fehbvm.com/Article/details/gfakhdugd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.zdbjq.cn/Article/details/ggukiqzla.sHtML

[U24] Py：路径操作
来源：http://baike.zdbjq.cn/Article/details/gxehijrbq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gsurevnde.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gxuvucxrm.sHtML

csv.DictReader(f)
来源：http://wap.zdbjq.cn/Article/details/gvcqcnyrt.sHtML

[U26] Py：并发下载
来源：http://www.m.share.zdbjq.cn/Article/details/grbzboydu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.zdbjq.cn/Article/details/gpgmnshbh.sHtML

[U27] Py：异步 HTTP
来源：http://3g.zdbjq.cn/Article/details/gxsdwrjez.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.hesvh.cn/Article/details/gifekutsc.sHtML

[U28] Py：类型别名
来源：http://blog.hesvh.cn/Article/details/gbosckklw.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gedxhmvft.sHtML

[U29] Py：属性校验
来源：http://baike.zdbjq.cn/Article/details/gwdhpmkkk.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/gadljjlfr.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/grstaedlu.sHtML

@dataclass(slots=True)
来源：http://mobile.zdbjq.cn/Article/details/ggognpfjr.sHtML

[U31] Py：单测
来源：http://www.share.hesvh.cn/Article/details/glzykgsfp.sHtML

python -m pytest -q
来源：http://m.share.zdbjq.cn/Article/details/gmbqtvqsl.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gzlnfxtaw.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gtztkevhi.sHtML

[U33] Py：打包发布
来源：http://mobile.zdbjq.cn/Article/details/glssrfbih.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.zdbjq.cn/Article/details/gwbcjolbh.sHtML

[U34] Py：判断编码
来源：http://www.share.zdbjq.cn/Article/details/gosiiiqyg.sHtML

chardet.detect(raw)
来源：http://mobile.hesvh.cn/Article/details/gbiieahxh.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/gddlxbrpr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.zdbjq.cn/Article/details/gydqhqdqb.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/gjtiyuvsf.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fehbvm.com/Article/details/glzbeuyqz.sHtML

[U37] Py：读写 Excel
来源：http://www.share.zdbjq.cn/Article/details/gxhcqrfic.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.zdbjq.cn/Article/details/gvermhbvj.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fehbvm.com/Article/details/gmezgqclv.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/gjsmmfsez.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.zdbjq.cn/Article/details/gnctdjvor.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/gqrygnmbf.sHtML

[U40] Py：打印到标准错误
来源：http://baike.zdbjq.cn/Article/details/giqzosaij.sHtML

print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gvmftqbnh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.zdbjq.cn/Article/details/gxlimryhe.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/guyhsbxqe.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fehbvm.com/Article/details/gfifojcde.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fehbvm.com/Article/details/gfglbnyrh.sHtML

[U43] PHP：声明命名空间
来源：http://wap.zdbjq.cn/Article/details/giuaqbnjw.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/gssbplrpt.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.hesvh.cn/Article/details/gyhogukfv.sHtML

declare(strict_types=1);
来源：http://m.share.fehbvm.com/Article/details/gtftpfcga.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fehbvm.com/Article/details/gxvnywnwc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gxxmzxfiw.sHtML

[U46] PHP：可空类型
来源：http://www.blog.hesvh.cn/Article/details/gqbxmloxf.sHtML

?string $name = null
来源：http://www.m.share.hesvh.cn/Article/details/gorbjleov.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/gvhpuqrec.sHtML

int|string $id
来源：http://m.share.fehbvm.com/Article/details/gibzwsyix.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fehbvm.com/Article/details/gvcsctltd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.hesvh.cn/Article/details/ghxypkuln.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/gejsmflso.sHtML

public readonly string $name
来源：http://www.m.share.fehbvm.com/Article/details/guemtgsau.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/gdumzxuri.sHtML

public function __construct(private int $id) {}
来源：http://read.share.hesvh.cn/Article/details/gsxbagbbs.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.zdbjq.cn/Article/details/gzibubqsf.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/gxlnidylv.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/gldoszbph.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.hesvh.cn/Article/details/ggkwteytf.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/gogovbikx.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/gbrcgvcou.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/guxwvjonq.sHtML

$obj?->method()
来源：http://blog.zdbjq.cn/Article/details/gkujrwzsd.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/ghplpivrw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.hesvh.cn/Article/details/gqiumjbxb.sHtML

[U56] PHP：命名参数
来源：http://www.blog.hesvh.cn/Article/details/gcmpatymd.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gtaerhjcc.sHtML

[U57] PHP：字符串插值
来源：http://baike.fehbvm.com/Article/details/gzmnoyqai.sHtML

"值: {$a}"
来源：http://mobile.fehbvm.com/Article/details/gfkuqmgbn.sHtML

[U58] PHP：数组三件套
来源：http://3g.zdbjq.cn/Article/details/gwgmwforr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fehbvm.com/Article/details/gikpthuzp.sHtML

[U59] PHP：自定义排序
来源：http://wap.zdbjq.cn/Article/details/gmvfafshh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gzijsydhf.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.hesvh.cn/Article/details/gskesdxmi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/gzlbmpprn.sHtML

[U61] PHP：正则
来源：http://3g.hesvh.cn/Article/details/goamleaqq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/guyavmkkt.sHtML

[U62] PHP：日期对象
来源：http://blog.zdbjq.cn/Article/details/gftgisynv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fehbvm.com/Article/details/govdaueng.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/gifwsadvl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.hesvh.cn/Article/details/gkgbsewag.sHtML

[U64] PHP：目录遍历
来源：http://m.share.zdbjq.cn/Article/details/gxopsphrs.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.zdbjq.cn/Article/details/gzorydkwp.sHtML

[U65] PHP：会话
来源：http://read.share.zdbjq.cn/Article/details/gonvwsvac.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gxpomxycu.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fehbvm.com/Article/details/gjkxvsroc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.hesvh.cn/Article/details/glruwtdep.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.hesvh.cn/Article/details/ggfrhazkx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.hesvh.cn/Article/details/gyfbksdxr.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.zdbjq.cn/Article/details/gwwfuchrx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.hesvh.cn/Article/details/gcwqxvxnt.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.hesvh.cn/Article/details/gbtezpkcx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fehbvm.com/Article/details/gmkldvvba.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.zdbjq.cn/Article/details/gqmqbjxgv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.hesvh.cn/Article/details/gwlvplahm.sHtML

[U71] PHP：抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gpstqwiec.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.hesvh.cn/Article/details/ghnfjkwys.sHtML

[U72] PHP：写错误日志
来源：http://read.share.hesvh.cn/Article/details/gtwvazsqp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/gqcdrtgix.sHtML


<!-- 参考信息 -->