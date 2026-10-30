代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gjxxnyscr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gdgvyumpy.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gvqpqabdl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/gdquhebnc.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/gokskkmck.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/gfjvhqvlt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gfrzxgndh.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/gugkwakgl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gmfipvcwb.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/giyjervpy.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gmtxkcsoa.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gpgglwbmg.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gagsabrqq.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gusrsefyt.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/gzhwftilt.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gvtvluxwh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gtezsmfnx.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gzmasaaih.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gjzfchykk.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gydehqous.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gidnibpus.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gfmoseshq.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gmbbqoomk.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/grbguvlvq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gvkoryurf.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gakeyqqgu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gjflscsxg.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gylwkhvwz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gomanbxrh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnrvxwxnc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gdhjdbndg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gklelqxjd.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gejtbycbd.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/grentsvif.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/ghytkpnok.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gjvcoszvm.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gacuzkxmv.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gafpejnkv.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gozwopgzs.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gijcjwqmo.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gcxkloezd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gqemvgiun.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gwssndjic.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gwucnyngr.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/gqluzpwci.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/gsiyubkxq.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/ggttodzqo.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gcqzuoggn.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/glgilkskt.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gbugwqvjl.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/goiaanrjb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/gsvkbkvqd.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/gfbrlmiqd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gwcqviage.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/gqvevtaaz.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gtkubysos.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gniamansv.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/gwpxbiisc.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gbzykkcgq.sHtML

for (i in 1..10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gngzanszv.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gzctewbdb.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gewddznyy.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/ghaoxobuk.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gtoodwdqn.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/gxbqeicbo.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gukybrpor.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gjjmmgkbu.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gthtgdlkg.sHtML

[T19] Swift：可选绑定
来源：http://www.share.hesvh.cn/Article/details/gsqjkkqhj.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/gaimlcgdb.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/gyfwtubhy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fehbvm.com/Article/details/gvtfomxpm.sHtML

[T21] Swift：遍历
来源：http://www.share.hesvh.cn/Article/details/gvtooxknx.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/gzlxfsbqd.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gouvtqmvv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.zdbjq.cn/Article/details/gnrnqztwt.sHtML

[T23] Swift：函数
来源：http://m.share.fehbvm.com/Article/details/gzwjvdmqd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gsphayjlr.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/ghfocpclm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gaypwkcme.sHtML

[T25] Swift：结构体
来源：http://blog.zdbjq.cn/Article/details/guujqafcy.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/guhvzeupw.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/gxibgamjr.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/gzkdvzame.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/gjoqasgkd.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fehbvm.com/Article/details/gtfpjcovl.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/gxhabbigl.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/gnxcyobcc.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fehbvm.com/Article/details/geqmisohw.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gmgitvcxp.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/ggsgarswq.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fehbvm.com/Article/details/gppqpsazj.sHtML

[T31] Lua：Hello World
来源：http://m.share.fehbvm.com/Article/details/gmfdmuxwv.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gcwtllqka.sHtML

[T32] Lua：局部变量
来源：http://baike.zdbjq.cn/Article/details/ghczdmmdi.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gqyqditss.sHtML

[T33] Lua：表（数组）
来源：http://wap.fehbvm.com/Article/details/gqmzkarwm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/gnxpxotfl.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/goxkdsxho.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fehbvm.com/Article/details/gjargfiuv.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gzwrkgpxf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gehezatel.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/gtpmmfhck.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/gkmywgpxc.sHtML

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/gnfmtcbdf.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gmzkdwmyp.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/gdffsbybo.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/gkjgymchx.sHtML

[T39] Lua：模式匹配
来源：http://3g.hesvh.cn/Article/details/gaetzvlkj.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gmzcfcvwy.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/glmowdwqr.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/ggkzqcvfh.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gaxxxyowp.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/ghxcdwqwu.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/gkvtbmgdh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gcxnfbruh.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gecbshspr.sHtML

"值: $a"
来源：http://wap.fehbvm.com/Article/details/gsfqppxim.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/gyvojbszx.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.zdbjq.cn/Article/details/gpykgsdiv.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/gxreqplvd.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/gpsoopcba.sHtML

[T46] Perl：哈希操作
来源：http://wap.zdbjq.cn/Article/details/gnvjyfoeg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gvwecwwqg.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gfslimlsi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.zdbjq.cn/Article/details/gvycyyhcr.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gxnwxtbcj.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/gnxzjafkz.sHtML

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/gzognaaxo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/grvabeoyo.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gucieaoxm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.hesvh.cn/Article/details/guhsyirmj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fehbvm.com/Article/details/ghugkjbuf.sHtML

[T51] Scala：Hello World
来源：http://blog.fehbvm.com/Article/details/gklrpnzug.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gmptwlvkt.sHtML

[T52] Scala：变量
来源：http://blog.hesvh.cn/Article/details/gmggotiks.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/gbkaapqif.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gnqtjeley.sHtML

s"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gvmuvabai.sHtML

[T54] Scala：集合映射
来源：http://baike.hesvh.cn/Article/details/gkawneeyq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/gwecuqgxy.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gofqomvfu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.hesvh.cn/Article/details/gnjexuiwo.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/gkvnwgotl.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gthoqnfht.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/gbghcoeut.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gewfjgazk.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/grulzpbaz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fehbvm.com/Article/details/gaxhikuzq.sHtML

[T59] Scala：循环
来源：http://www.share.hesvh.cn/Article/details/guuiwvvxj.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gudhjhqma.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/gpxablfes.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fehbvm.com/Article/details/gvbzebycq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtmvgdocw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/grocongsb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gudiielag.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.zdbjq.cn/Article/details/gnyjlpyhp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.hesvh.cn/Article/details/glvycmmaq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.zdbjq.cn/Article/details/gaqkrcqzg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/gyzuwpzot.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fehbvm.com/Article/details/gjgpnnewh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.zdbjq.cn/Article/details/gyxrsqzwb.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/ggzcwesya.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/gqpgezdph.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/ggwotfrzf.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/grfgzatan.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/guofmauos.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gotcmxwws.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/gbagmyjfo.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/gkaicwwkv.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/giqyhfhds.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/gwvamhttp.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/gmlfeosxx.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/garaxlqrt.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/gknljgzwu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/gxcgihynm.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/gdryowfsp.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/gsimjaxkw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/gumywzwau.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/ghygxruwg.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fehbvm.com/Article/details/gaauudoly.sHtML

deque(maxlen=10)
来源：http://blog.fehbvm.com/Article/details/gooezqhub.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fehbvm.com/Article/details/gmfstijvo.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gzxborlwr.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/gutcsxral.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/gbuarkgwd.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fehbvm.com/Article/details/gjgboazmg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/grniwtwif.sHtML

[U17] Py：初始化日志
来源：http://read.share.hesvh.cn/Article/details/glrzmprnc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gixymbhww.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/grptcluks.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/gatwolqfw.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.hesvh.cn/Article/details/gulbftzym.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fehbvm.com/Article/details/gkrizfrpo.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.zdbjq.cn/Article/details/gkigyivsp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/gcfvylniz.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/grojvptsk.sHtML

@contextlib.contextmanager
来源：http://3g.zdbjq.cn/Article/details/glstvjevr.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/gniesbfje.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/gpdnatshv.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.zdbjq.cn/Article/details/gramkurus.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/gfgbjyeri.sHtML

[U24] Py：路径操作
来源：http://www.blog.fehbvm.com/Article/details/gcahfgvln.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gzseaxjhg.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/giqlcoxkt.sHtML

csv.DictReader(f)
来源：http://m.share.fehbvm.com/Article/details/gdmsjfcvp.sHtML

[U26] Py：并发下载
来源：http://wap.hesvh.cn/Article/details/gmjibhdvy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/gjyfmwaeb.sHtML

[U27] Py：异步 HTTP
来源：http://3g.zdbjq.cn/Article/details/gxwnpkacn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.zdbjq.cn/Article/details/gmgfxtsgc.sHtML

[U28] Py：类型别名
来源：http://blog.hesvh.cn/Article/details/gblefnvez.sHtML

UserId = int
来源：http://www.share.fehbvm.com/Article/details/gcxzvlrac.sHtML

[U29] Py：属性校验
来源：http://www.blog.hesvh.cn/Article/details/gkypbunkn.sHtML

@property 与 @x.setter 配合
来源：http://baike.zdbjq.cn/Article/details/gdgusrmsl.sHtML

[U30] Py：数据类
来源：http://wap.hesvh.cn/Article/details/garxtwwkj.sHtML

@dataclass(slots=True)
来源：http://blog.fehbvm.com/Article/details/gmoprdlcc.sHtML

[U31] Py：单测
来源：http://www.share.hesvh.cn/Article/details/gvmsplmly.sHtML

python -m pytest -q
来源：http://www.m.share.hesvh.cn/Article/details/gzqnnkryi.sHtML

[U32] Py：代码格式化
来源：http://m.share.zdbjq.cn/Article/details/ghhbfmmpb.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/gcltsxngv.sHtML

[U33] Py：打包发布
来源：http://www.blog.fehbvm.com/Article/details/glgkcqvcn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fehbvm.com/Article/details/gcjpmixvp.sHtML

[U34] Py：判断编码
来源：http://baike.zdbjq.cn/Article/details/gyjqcphsq.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/gyqrfguvs.sHtML

[U35] Py：发送邮件
来源：http://www.blog.zdbjq.cn/Article/details/gykefvtuw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/ggjsljtmw.sHtML

[U36] Py：定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gzrxutfiu.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/gfwzqkabm.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.hesvh.cn/Article/details/gypzfaceg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.hesvh.cn/Article/details/gdvsizkvo.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/ganijrdci.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fehbvm.com/Article/details/gltfmyedi.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/guasalfqw.sHtML

sys.stdout.isatty()
来源：http://www.share.fehbvm.com/Article/details/gemmmpwvz.sHtML

[U40] Py：打印到标准错误
来源：http://3g.zdbjq.cn/Article/details/gxtrmgvtk.sHtML

print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gxvruftvw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.zdbjq.cn/Article/details/gcqnuyygm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.zdbjq.cn/Article/details/ggqstihjy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/geibdtlay.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/gkuqhyije.sHtML

[U43] PHP：声明命名空间
来源：http://3g.hesvh.cn/Article/details/gxiirjmhq.sHtML

namespace App\Http;
来源：http://baike.hesvh.cn/Article/details/gwiqjwijh.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.hesvh.cn/Article/details/geehcgkoh.sHtML

declare(strict_types=1);
来源：http://3g.fehbvm.com/Article/details/glbkoghih.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/ggyqmojqy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/goqgfiukh.sHtML

[U46] PHP：可空类型
来源：http://www.share.fehbvm.com/Article/details/gndbteunc.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/guqmcwlnm.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.hesvh.cn/Article/details/gklbccfgq.sHtML

int|string $id
来源：http://m.share.fehbvm.com/Article/details/gryjekiut.sHtML

[U48] PHP：纯枚举
来源：http://wap.zdbjq.cn/Article/details/gqtzgdsyt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fehbvm.com/Article/details/gtwczqlxw.sHtML

[U49] PHP：只读属性
来源：http://3g.fehbvm.com/Article/details/gjssrufsy.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/gwvhutsbx.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.hesvh.cn/Article/details/gfgvgrfyh.sHtML

public function __construct(private int $id) {}
来源：http://wap.hesvh.cn/Article/details/gbbhglyuu.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fehbvm.com/Article/details/geercxgqw.sHtML

[$a, $b] = $arr;
来源：http://3g.hesvh.cn/Article/details/ghelgawjk.sHtML

[U52] PHP：箭头函数
来源：http://wap.zdbjq.cn/Article/details/ggdgjiaqc.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gjexdylrm.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fehbvm.com/Article/details/gpviduetf.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.hesvh.cn/Article/details/gbttbwycq.sHtML

[U54] PHP：空安全调用
来源：http://mobile.hesvh.cn/Article/details/gqksmzpon.sHtML

$obj?->method()
来源：http://read.share.fehbvm.com/Article/details/gdziqegzw.sHtML

[U55] PHP：match 表达式
来源：http://3g.fehbvm.com/Article/details/gqujwcqft.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/glwoyroty.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/gadnszrfu.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gjszvxukb.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gmtqpogox.sHtML

"值: {$a}"
来源：http://m.share.fehbvm.com/Article/details/gxxugumgi.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fehbvm.com/Article/details/gikgutzeh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fehbvm.com/Article/details/ggkzpvtwy.sHtML

[U59] PHP：自定义排序
来源：http://m.share.zdbjq.cn/Article/details/gfvxhjaye.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gyizqgceb.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fehbvm.com/Article/details/giggeuaxc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/gdachbnmu.sHtML

[U61] PHP：正则
来源：http://3g.hesvh.cn/Article/details/gnxzdszwx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gmajohvph.sHtML

[U62] PHP：日期对象
来源：http://3g.zdbjq.cn/Article/details/glxcpbgqy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.zdbjq.cn/Article/details/gocuzmmjr.sHtML

[U63] PHP：文件读写
来源：http://blog.fehbvm.com/Article/details/gwxtkayiu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fehbvm.com/Article/details/giopiimmr.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/glydfxkao.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.zdbjq.cn/Article/details/gijuexubk.sHtML

[U65] PHP：会话
来源：http://baike.fehbvm.com/Article/details/gnwtgyumt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.hesvh.cn/Article/details/godcvfumk.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/gqmyknevy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.hesvh.cn/Article/details/ghuhuewtf.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.zdbjq.cn/Article/details/gqbuoqstt.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.hesvh.cn/Article/details/grghxdtzn.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fehbvm.com/Article/details/gkygjrzdp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/gqbpraomq.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/glmuurckb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.zdbjq.cn/Article/details/gtfywhyqa.sHtML

[U70] PHP：PDO 事务
来源：http://blog.zdbjq.cn/Article/details/gqnnqztsc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/ggalbatyw.sHtML

[U71] PHP：抛出异常
来源：http://blog.zdbjq.cn/Article/details/gwzoulnit.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fehbvm.com/Article/details/gbmikgikn.sHtML

[U72] PHP：写错误日志
来源：http://3g.fehbvm.com/Article/details/geupneuwd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/gkeuosihm.sHtML


<!-- 参考信息 -->