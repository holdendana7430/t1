代发 wailian999

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gvbpfrwcl.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gggpivngg.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gkvlrinek.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gmtxkjpyh.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gbrjxywcm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/grjdbevtp.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/gzbfnskrf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/giideivsl.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gmsxxgibw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gjjjiethq.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gbcdoarib.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gxmrqymgo.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/ggcgjmbyc.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gylndfcpi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gopzibxyb.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gxawhqeso.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gouyjughe.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/gowllhcrd.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gswxyphvv.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gcwcdattx.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gqxokkgwx.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/gwmejqnal.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gonmwfppm.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/goxkqnddy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/gltanbynp.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gojiuuoyu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/gdqhvcwfb.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gxfdubosy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/gdsnappjs.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gxokbwwin.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/gaytbjcty.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gazwlsqrx.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gxnfsfftq.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gqcxwjdsk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gwkinkbyf.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/grtkxlopv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gasgrspey.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtjmffvfu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gzixnmsdg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpdygwvzs.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gpjuevico.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gevyvxdxr.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/gyqtjzqic.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gcvtyapoz.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gijcztgjj.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gzazgzhtk.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/gtqlkwmfq.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/gzxjcbtwt.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/gfvbqzppo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gtgwalhwd.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/glmytjdtt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gxcxifowe.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gzwavrfyv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/gxhvzbqak.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/gcxauutfm.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/gtjaszyms.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/gowybpjfg.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gpyzesggf.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/glglbbfof.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/gvgypnzxd.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/gdjoxvucp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/gwyqyyozw.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/gojoqjfhi.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gvqspqwgx.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/grbprahat.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/gfywhtxst.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gjwypktby.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/ggtzqlzyw.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/ghezzsows.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gmzlbshui.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gqicrtuvt.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gbjanionq.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gxssargkm.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gtvwvaqrb.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/geltcchhh.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/gzjhdowqj.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/glohpeujh.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/gjktdfget.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/ghjngfimg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gqrcfoucs.sHtML

[T21] Swift：遍历
来源：http://wap.hesvh.cn/Article/details/gnbxzkovq.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/gpttnxjdv.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/grmiohsyk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gaqmvluys.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/gbgkgfhuk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/gcnwcsazl.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/gbajieskc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/geugnullz.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/gsrxtguux.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gmwsrwqth.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gbjsnleuj.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/grwxtbfdp.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/gaaulsuqp.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fehbvm.com/Article/details/gaqvubfty.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/gobyecozr.sHtML

enum Color { case red, green }
来源：http://3g.hesvh.cn/Article/details/gvkvupzoa.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fehbvm.com/Article/details/gjbfeimis.sHtML

guard let x = opt else { return }
来源：http://www.blog.zdbjq.cn/Article/details/gifagdcls.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gfxjcmncc.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gbxyjmugs.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gqpwovcpl.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gpaqswioz.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/gktelfsvb.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gasujoxno.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/gqeebruza.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.zdbjq.cn/Article/details/gbzqmyeai.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/gjddhkflb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gqpkwehil.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gdqxyhivt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gehxdwavp.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/gzigcuncc.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gydslsdzz.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gaveqrzdf.sHtML

"a" .. "b"
来源：http://www.m.share.fehbvm.com/Article/details/gzvnyyaxf.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/guskaexsf.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/ganagvqxv.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gzosehiga.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/glngifnfh.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/gafzshvjl.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/gtnpaooyh.sHtML

[T41] Perl：Hello World
来源：http://www.blog.hesvh.cn/Article/details/grwlzuslp.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gnyhfzypl.sHtML

[T42] Perl：变量类型
来源：http://mobile.hesvh.cn/Article/details/goitrwosf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.zdbjq.cn/Article/details/gvowkhqtw.sHtML

[T43] Perl：字符串插值
来源：http://blog.fehbvm.com/Article/details/gqptgknzl.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/gmwrxdzar.sHtML

[T44] Perl：条件
来源：http://www.share.zdbjq.cn/Article/details/gzsjgydli.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/gkfqerzvx.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/gkqmukcqh.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.hesvh.cn/Article/details/ggtjeqmyf.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/glptylxsi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/glbhkjkfo.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/gchpscquz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/gvcdmbsuo.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/grrqqjolo.sHtML

$s =~ s/old/new/g;
来源：http://wap.hesvh.cn/Article/details/gdbcmoktq.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/gkilypkig.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/ghpfrhwmp.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gacytwphq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/gkphxbbfo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fehbvm.com/Article/details/ggkftohik.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gwtcptkav.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gjqvswfaj.sHtML

[T52] Scala：变量
来源：http://wap.fehbvm.com/Article/details/geswayogl.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/goounsgbj.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gfgabbndg.sHtML

s"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gtjekpmoq.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/gsmszwnon.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/gvsqeqzwe.sHtML

[T55] Scala：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gyflvbfux.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/grivrtvuh.sHtML

[T56] Scala：样例类
来源：http://read.share.hesvh.cn/Article/details/gmihhpwve.sHtML

case class User(name: String, age: Int)
来源：http://blog.hesvh.cn/Article/details/gpjknwfia.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gyuaotksl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/gaploipqf.sHtML

[T58] Scala：函数定义
来源：http://www.share.hesvh.cn/Article/details/ghhnhlgxk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.zdbjq.cn/Article/details/gyllutvaz.sHtML

[T59] Scala：循环
来源：http://blog.fehbvm.com/Article/details/ghfpbydzf.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gtbuszksr.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/gichwkqcu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/gfrizakeq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gljinxmmq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gihvqvzpx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghbcznxit.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/ghentnnsj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/gfuxqnngw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/gmjwqsyra.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fehbvm.com/Article/details/gonybsepl.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gfhncjtww.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fehbvm.com/Article/details/gpqqwxnok.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fehbvm.com/Article/details/gdahwkpwo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/gpypavuuc.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fehbvm.com/Article/details/gzjyuzfij.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gqsbsvvwk.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/gzuvaksmq.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/ghbxomztw.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/giainyupa.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/gzqhyspkq.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/ghxmtvnxw.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/gxydljgms.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/guzvbbckq.sHtML

max(d, key=d.get)
来源：http://www.blog.fehbvm.com/Article/details/gcbpxwxjf.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/gizpokvxi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.hesvh.cn/Article/details/gjaavzmdm.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/gqqixckdg.sHtML

(x * 2 for x in arr)
来源：http://www.share.zdbjq.cn/Article/details/goekqgnsm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/guvpurypq.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fehbvm.com/Article/details/gdtgwymeu.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fehbvm.com/Article/details/goqutmktf.sHtML

deque(maxlen=10)
来源：http://blog.zdbjq.cn/Article/details/gfimpelqc.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.zdbjq.cn/Article/details/gcflvewco.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/ghltxrtwl.sHtML

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/gcmznquqz.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/gklwswdso.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.zdbjq.cn/Article/details/gtbyhqyah.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.hesvh.cn/Article/details/gbzxmkgzw.sHtML

[U17] Py：初始化日志
来源：http://blog.zdbjq.cn/Article/details/gtwtmxdrq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.hesvh.cn/Article/details/gmwtkilql.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/gikauneog.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/gtljekbrj.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/glwpytglp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/gfflaaiqu.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/gxlkctlid.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gaadrcpzd.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/gqaehqutx.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/gddwthsfa.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/ghscmibjc.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/gzkxemugl.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.hesvh.cn/Article/details/grtqgwkpg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/glsjyhhzt.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/ghjqugiul.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gevrknpqo.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.zdbjq.cn/Article/details/gnglhjidd.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gawkrtvwm.sHtML

[U26] Py：并发下载
来源：http://read.share.hesvh.cn/Article/details/ggdyzdbjb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fehbvm.com/Article/details/glradsrbv.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fehbvm.com/Article/details/gdfemprff.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/gmrqqfclm.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/gfxhiawxg.sHtML

UserId = int
来源：http://www.m.share.fehbvm.com/Article/details/gupwfarox.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/gzzvzgjon.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/gjygmyesh.sHtML

[U30] Py：数据类
来源：http://3g.zdbjq.cn/Article/details/grrgyygal.sHtML

@dataclass(slots=True)
来源：http://blog.hesvh.cn/Article/details/gijorxogk.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/gdbnqydlx.sHtML

python -m pytest -q
来源：http://3g.fehbvm.com/Article/details/gtjhggcfj.sHtML

[U32] Py：代码格式化
来源：http://read.share.hesvh.cn/Article/details/gjjrxqihy.sHtML

ruff format . && ruff check --fix .
来源：http://wap.zdbjq.cn/Article/details/gjdlprvos.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/gcfvdvocu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fehbvm.com/Article/details/giducavvx.sHtML

[U34] Py：判断编码
来源：http://m.share.hesvh.cn/Article/details/gliivgdra.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/gdxunzpej.sHtML

[U35] Py：发送邮件
来源：http://www.share.hesvh.cn/Article/details/gdqqqssuf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/gvinzbjew.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/gqgocnogq.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fehbvm.com/Article/details/gvoyrkwzm.sHtML

[U37] Py：读写 Excel
来源：http://blog.zdbjq.cn/Article/details/gcwcmigvs.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.zdbjq.cn/Article/details/gkeiheulc.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/gfovunpmy.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/gyigglvmp.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/gqmmxaeap.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/gzuvaeqxy.sHtML

[U40] Py：打印到标准错误
来源：http://3g.zdbjq.cn/Article/details/gbbarnakb.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/geifcmkxp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.hesvh.cn/Article/details/gikzeqcxh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fehbvm.com/Article/details/ggpiygclj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.zdbjq.cn/Article/details/gilexazcd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.hesvh.cn/Article/details/gzjshciig.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/gucwbvtqg.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/gleyevgwy.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/gxemtpmvh.sHtML

declare(strict_types=1);
来源：http://www.share.hesvh.cn/Article/details/gueatdygw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.zdbjq.cn/Article/details/gcyrzvqet.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gxfznuxyf.sHtML

[U46] PHP：可空类型
来源：http://baike.fehbvm.com/Article/details/gzhdfrnjt.sHtML

?string $name = null
来源：http://blog.fehbvm.com/Article/details/ggjwhstoo.sHtML

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/gzllrynit.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gtjbpruen.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fehbvm.com/Article/details/gtamwnlhw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fehbvm.com/Article/details/ghcbbnoej.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/gwlzdqpbf.sHtML

public readonly string $name
来源：http://m.share.fehbvm.com/Article/details/gvrfisxgf.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.hesvh.cn/Article/details/gxlpnncwp.sHtML

public function __construct(private int $id) {}
来源：http://blog.zdbjq.cn/Article/details/gxtdfvinv.sHtML

[U51] PHP：数组解构
来源：http://m.share.zdbjq.cn/Article/details/gbpygrwcl.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/gdlimlcng.sHtML

[U52] PHP：箭头函数
来源：http://3g.hesvh.cn/Article/details/gjyvgabuv.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gaqrirxfd.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/ghyjbanit.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/gdcfvhodl.sHtML

[U54] PHP：空安全调用
来源：http://www.share.zdbjq.cn/Article/details/gyioolhwy.sHtML

$obj?->method()
来源：http://www.share.hesvh.cn/Article/details/gvfzzigwe.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fehbvm.com/Article/details/gcebbggpe.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.zdbjq.cn/Article/details/gmjztmzvt.sHtML

[U56] PHP：命名参数
来源：http://www.share.zdbjq.cn/Article/details/grzdzfenm.sHtML

f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gazlvannp.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gvrrtfphn.sHtML

"值: {$a}"
来源：http://baike.hesvh.cn/Article/details/grjwndzii.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.hesvh.cn/Article/details/gwvupeebv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gxecaxsxj.sHtML

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/gtfxmolvu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gvskjmjxs.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fehbvm.com/Article/details/gpntqlaxq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/gmlhsbuby.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/giraxisim.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gkdlfcqmf.sHtML

[U62] PHP：日期对象
来源：http://baike.fehbvm.com/Article/details/gulghlsns.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.hesvh.cn/Article/details/gmltpyztj.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/glhrqdqfa.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.hesvh.cn/Article/details/gyknhvsjs.sHtML

[U64] PHP：目录遍历
来源：http://wap.fehbvm.com/Article/details/gohtvxwsn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fehbvm.com/Article/details/gamdateja.sHtML

[U65] PHP：会话
来源：http://www.m.share.fehbvm.com/Article/details/gsvfylhtv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.zdbjq.cn/Article/details/guxzevcsw.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fehbvm.com/Article/details/gwqwoguhw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.zdbjq.cn/Article/details/glouaoebr.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/gayiwbtoi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/gkujluqnt.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fehbvm.com/Article/details/gecezauae.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/gsmhvjuwj.sHtML


<!-- 参考信息 -->