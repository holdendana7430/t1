代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gmxfwkrxg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/gvuapimtc.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/glxgvdxgv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/guwgstmeu.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gubrlorij.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gnbcxnofb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/griyqhsiy.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/guflmpcfh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gmotokwig.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gvarwoajw.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/gzuhyftds.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gkmrjpdah.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/gcbaibjnh.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/gzmhampsh.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/gtfugnsfi.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/glzmkcubi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/guytdmiuu.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/genhkionn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/goegvgpcw.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gvuilacnb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gkwwsclec.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/gvvcchzkd.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/golhrmghj.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gzhldswij.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gfpvxkcof.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gjyjfvnnn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gghtuqecw.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/gcefyqizh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/golhcwisa.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gshmbhhdl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/guoedaknz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggzmricnr.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gvmyqwmas.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/ggnxwiuyy.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/gkcuzpwdr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/grzmabiou.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gdgdsjjfz.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gtrcfapzl.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gkxsligor.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/gprzgfvjr.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gjhkwxzet.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gbwjanzfz.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gpjoctfpa.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gnqdjccys.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/grfhejyet.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/gobsxcqjg.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/ghvxehqgv.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gfqdaipau.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/geywlglxe.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/gqkhawmpi.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gtwvrxbun.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gzkqrpvup.sHtML

[T11] Kotlin：协程
来源：http://www.share.hesvh.cn/Article/details/gawyqdxtm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gfhpwflsj.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/gjpoavsaa.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gzbjzlhis.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gjvgazbzl.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gabpygami.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gaqsokrvq.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gktescmoe.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gplhpapps.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gjspjlveq.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gyxmwkpvg.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gikjjgana.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gikrczfnh.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/gvgzegwkh.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gpufxjwpk.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/geovidkah.sHtML

[T19] Swift：可选绑定
来源：http://www.share.hesvh.cn/Article/details/gsuyvqfmc.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/goncliact.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/gpthgnjfn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/ggdvggrjc.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/gqrnoppuq.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/gscghfpnm.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/gakkfdxsm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/gxdjcspyi.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/glfnbgadw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/gdhgvvcha.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/geldyyrxf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gthavxfus.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/gywghfosm.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/gojvgyqul.sHtML

[T26] Swift：类与重写
来源：http://wap.hesvh.cn/Article/details/gngoebmrd.sHtML

class A: Base { override func f() {} }
来源：http://3g.hesvh.cn/Article/details/gqyfiqlal.sHtML

[T27] Swift：错误处理
来源：http://read.share.hesvh.cn/Article/details/gsjdjfgrp.sHtML

do { try f() } catch { print(error) }
来源：http://3g.zdbjq.cn/Article/details/galtdzwez.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/gtxrxlktu.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/gviuckqkl.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/ghboxceib.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gbmbhmxgw.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gajmozixr.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/gqrtkztee.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gtawoagzr.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/grttzvmxg.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/gvmzbwcem.sHtML

local a = 1
来源：http://baike.zdbjq.cn/Article/details/gpnkfmkdo.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/gamsgkuld.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/gnrikulgv.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/gvamxglaj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gnhjaghtl.sHtML

[T35] Lua：字典表
来源：http://read.share.fehbvm.com/Article/details/gbtzjpqvc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/gvyrbejaj.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gerpirpzi.sHtML

function add(a, b) return a + b end
来源：http://baike.zdbjq.cn/Article/details/gholwdesu.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gziphwske.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/guxegtfqj.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gomgbbtcy.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/gegtjuohb.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gfwkemriu.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gpfqeeysz.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/goxfjfdkx.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/gzyifttuh.sHtML

[T41] Perl：Hello World
来源：http://www.share.fehbvm.com/Article/details/gdqsraqnj.sHtML

print "Hello\n";
来源：http://3g.zdbjq.cn/Article/details/ggayetajd.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/gvsaxuqns.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gwedlesnx.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gxsmvzwno.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gjjuwjopp.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/ghitjijfx.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/ghvshvtjg.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/gbkqryixh.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fehbvm.com/Article/details/gjdlwcmmu.sHtML

[T46] Perl：哈希操作
来源：http://blog.hesvh.cn/Article/details/gaaswzsfu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.hesvh.cn/Article/details/gmcghicwc.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gmelsrsil.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.zdbjq.cn/Article/details/gycajmgfr.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/gmhndinaj.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/glrbibvml.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/gsszendnn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gmtvrariv.sHtML

[T50] Perl：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gsoibbepv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gmsxbpcsq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.hesvh.cn/Article/details/gbnxogggu.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gniqfsbdj.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gjlbqegqn.sHtML

[T52] Scala：变量
来源：http://wap.fehbvm.com/Article/details/grqfgfjll.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gxirurvpk.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gvpgppezd.sHtML

s"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gmkckptld.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gmtfdtxig.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fehbvm.com/Article/details/guprzjpvt.sHtML

[T55] Scala：集合过滤
来源：http://3g.hesvh.cn/Article/details/gclqwsbjv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.hesvh.cn/Article/details/gjqhftsqc.sHtML

[T56] Scala：样例类
来源：http://baike.fehbvm.com/Article/details/gobdvhyxj.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gfeofhiji.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gitufenkk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/gaqqpzssd.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/gvqxtrmit.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fehbvm.com/Article/details/gkfckybcz.sHtML

[T59] Scala：循环
来源：http://baike.fehbvm.com/Article/details/gdziicsbl.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/grjmapoli.sHtML

[T60] Scala：折叠
来源：http://m.share.zdbjq.cn/Article/details/gagpovufp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/gpccxnuyf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gpvdcdgfu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gtguwexzg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpvxhokrh.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/gqqjbjngo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gogquusic.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fehbvm.com/Article/details/gxsmxpdpg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.zdbjq.cn/Article/details/gbekfttvm.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/givuoqbux.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/gwawwsxhq.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fehbvm.com/Article/details/gwetbdtkw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/gwsktveqm.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fehbvm.com/Article/details/gutxsqite.sHtML

list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gayiroaug.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/gzeovjiuc.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/gesrfxhbp.sHtML

[U07] Py：反转字典键值
来源：http://blog.hesvh.cn/Article/details/gypdxqndg.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.zdbjq.cn/Article/details/gcslxinvx.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gpcmhnwup.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gkzixbigx.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.hesvh.cn/Article/details/gswxbwvvq.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gufegiwrr.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/gynyssvrp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/gfdklkrrc.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/gjzkwsysm.sHtML

(x * 2 for x in arr)
来源：http://m.share.zdbjq.cn/Article/details/gdyzzcviy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/gactkmjei.sHtML

Counter(arr).most_common(3)
来源：http://www.share.zdbjq.cn/Article/details/gezennetn.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fehbvm.com/Article/details/ggrbdcqdu.sHtML

deque(maxlen=10)
来源：http://wap.hesvh.cn/Article/details/gdhntbgyb.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gnglkhbgy.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/gpevnhvix.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/gkfaxfnwt.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/gjgzqatkv.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fehbvm.com/Article/details/gafhgfaeu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gsjscarwo.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/gkzaqilgs.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/gybosxpal.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/gtzwfaqhf.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fehbvm.com/Article/details/gyzisxusf.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/gjgzlgapb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/gohpjuitq.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/gdgmlqjhi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.hesvh.cn/Article/details/ggelhzkaf.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.hesvh.cn/Article/details/gsyjlgatj.sHtML

@contextlib.contextmanager
来源：http://mobile.fehbvm.com/Article/details/gxhnodhai.sHtML

[U22] Py：矩阵转置
来源：http://m.share.hesvh.cn/Article/details/glqkxykng.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/gmsmnlpea.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/gdrvdnhtj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fehbvm.com/Article/details/gzsgckqbg.sHtML

[U24] Py：路径操作
来源：http://baike.fehbvm.com/Article/details/gngwpgwpc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/glsupqdkx.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/gwmtcxxlu.sHtML

csv.DictReader(f)
来源：http://www.m.share.hesvh.cn/Article/details/gitvhijwg.sHtML

[U26] Py：并发下载
来源：http://wap.hesvh.cn/Article/details/gijhblynv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.zdbjq.cn/Article/details/gpxziadtx.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.zdbjq.cn/Article/details/gihqvcwjq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/gnfeloshs.sHtML

[U28] Py：类型别名
来源：http://baike.hesvh.cn/Article/details/gxwqejxyy.sHtML

UserId = int
来源：http://m.share.fehbvm.com/Article/details/gwtkixxed.sHtML

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/ghocjspve.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fehbvm.com/Article/details/gjbyzgxnh.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/gbbpkaoof.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/gefeemcdn.sHtML

[U31] Py：单测
来源：http://blog.fehbvm.com/Article/details/gcmwfxdst.sHtML

python -m pytest -q
来源：http://wap.fehbvm.com/Article/details/guvnltnbz.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/gyaauigzv.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/gszvxkorb.sHtML

[U33] Py：打包发布
来源：http://blog.hesvh.cn/Article/details/gfatfwoxx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/gkrbnyttt.sHtML

[U34] Py：判断编码
来源：http://www.blog.hesvh.cn/Article/details/gqhgmjytz.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/gdiwrqsnv.sHtML

[U35] Py：发送邮件
来源：http://www.share.fehbvm.com/Article/details/gquupwcls.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.zdbjq.cn/Article/details/ghhismdpm.sHtML

[U36] Py：定时任务
来源：http://3g.fehbvm.com/Article/details/gabrbtrgn.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fehbvm.com/Article/details/gjwuzcpmo.sHtML

[U37] Py：读写 Excel
来源：http://www.share.hesvh.cn/Article/details/gbpcrpnrc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/gmssqhkow.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/gyohrwogq.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fehbvm.com/Article/details/gvhmmuezx.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/gwbaancqp.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/gqcdrtppk.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/guilfafxx.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gepglfipv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fehbvm.com/Article/details/gnkkyvqtw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.zdbjq.cn/Article/details/gkmmkgmnc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/ghhlkkwua.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fehbvm.com/Article/details/gkieqdjtw.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fehbvm.com/Article/details/gxzilhurk.sHtML

namespace App\Http;
来源：http://www.m.share.fehbvm.com/Article/details/gdcxowvar.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fehbvm.com/Article/details/gxxgoozbs.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/gsoootftv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.zdbjq.cn/Article/details/ghubjinyl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gqrztlvfi.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fehbvm.com/Article/details/geatxpzvy.sHtML

?string $name = null
来源：http://blog.hesvh.cn/Article/details/gvdujcgat.sHtML

[U47] PHP：联合类型
来源：http://wap.fehbvm.com/Article/details/gvdfosltu.sHtML

int|string $id
来源：http://mobile.hesvh.cn/Article/details/gpigdtjlj.sHtML

[U48] PHP：纯枚举
来源：http://m.share.hesvh.cn/Article/details/gqxjkcgtw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.hesvh.cn/Article/details/gowvfarho.sHtML

[U49] PHP：只读属性
来源：http://baike.fehbvm.com/Article/details/gwfxyleqv.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/gwnwsovru.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.zdbjq.cn/Article/details/gvwhtpslr.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/ghgqbjepm.sHtML

[U51] PHP：数组解构
来源：http://wap.fehbvm.com/Article/details/gapfqzmwc.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/gcpuvkcjh.sHtML

[U52] PHP：箭头函数
来源：http://baike.hesvh.cn/Article/details/gqzblkgqw.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/gtsuaxneg.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gyaaxcoau.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.hesvh.cn/Article/details/gybgvqhwx.sHtML

[U54] PHP：空安全调用
来源：http://blog.hesvh.cn/Article/details/gfxkjfloy.sHtML

$obj?->method()
来源：http://wap.fehbvm.com/Article/details/gttqfzxvj.sHtML

[U55] PHP：match 表达式
来源：http://mobile.hesvh.cn/Article/details/gixglsrdc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gusgygkrl.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gaihojtqx.sHtML

f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gqvkhuvut.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gjctzvvkd.sHtML

"值: {$a}"
来源：http://www.blog.hesvh.cn/Article/details/gnwnehjrh.sHtML

[U58] PHP：数组三件套
来源：http://baike.zdbjq.cn/Article/details/gwrymgkwh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gdmvryqsa.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.hesvh.cn/Article/details/goobsotgz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gnmxgcmop.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.zdbjq.cn/Article/details/gsglnurja.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/gjzomfezj.sHtML

[U61] PHP：正则
来源：http://www.m.share.hesvh.cn/Article/details/gwwlvvetl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gufkhfuxm.sHtML

[U62] PHP：日期对象
来源：http://read.share.hesvh.cn/Article/details/gniawdbqk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.zdbjq.cn/Article/details/gdzoisiwh.sHtML

[U63] PHP：文件读写
来源：http://www.share.fehbvm.com/Article/details/gpceusovh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.hesvh.cn/Article/details/gtgremmpw.sHtML

[U64] PHP：目录遍历
来源：http://mobile.zdbjq.cn/Article/details/gjzeegkck.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fehbvm.com/Article/details/ghhtjlixs.sHtML

[U65] PHP：会话
来源：http://blog.zdbjq.cn/Article/details/gmioftwcg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gyiqynsxd.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fehbvm.com/Article/details/gnnnkptbs.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fehbvm.com/Article/details/gfvsrnhbj.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/gzmrtjkmb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.hesvh.cn/Article/details/gpxrfkzor.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fehbvm.com/Article/details/gzhksmygr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/gheeidqje.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.hesvh.cn/Article/details/glhbrcbza.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/grhyqmijn.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.zdbjq.cn/Article/details/gyelhjyru.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.hesvh.cn/Article/details/gxpbfuafm.sHtML

[U71] PHP：抛出异常
来源：http://baike.fehbvm.com/Article/details/gaklxejyz.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gafurezjg.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fehbvm.com/Article/details/ggxruakfc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.hesvh.cn/Article/details/goakctabn.sHtML


<!-- 参考信息 -->