代发 wailian999

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gyrzxhqmd.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gpihcxmec.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/gxakemymw.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gcvhndlbm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gcbwvmrgt.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gfmbcrgtd.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gkwtzfudh.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gstqcpmux.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gzlmsoxsk.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gzaekmnwn.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gtslexryv.sHtML

[S54] C++：异常处理
来源：http://wap.hesvh.cn/Article/details/gdidxqifs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.zdbjq.cn/Article/details/gifdoqyyf.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/ghzuueumh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gsiqtlhtu.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gwmudiext.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gnicgxolc.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/gghqarghj.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gtewbxdcj.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gdxvapvgq.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/gmitndrbv.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/gxbwuekdi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/gdlccskze.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/ghuvywhde.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/grthfgbsa.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/guenpraye.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gzpwwqecz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxygucfhm.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/girqpyqpo.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gwrwbsmeh.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gkhdqmozr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gkjwajelg.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gbznkgzcc.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gqbpwdogf.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/ghjbfccge.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gaiioliiy.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gniykxwgz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gomcnvkdg.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/ggghslvhq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gdqanbrwp.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gxhtcxqeb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gsxmuvwnt.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gemedtfwu.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gxiwbskoc.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/gpnnmysbw.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/gqrkkoyyg.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/gcgbsbhve.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gvtsjfsyt.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/gkvxzhlue.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gqolworrm.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/gxbhrwxbn.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gbwutlqfi.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/gernsdzxf.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gojhlltzz.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gqdjclmil.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gnmjqdsjv.sHtML

[T15] Kotlin：接口
来源：http://wap.fehbvm.com/Article/details/ghpivsijj.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/giaayodpa.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/gbgjqjmkd.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gtwpjriij.sHtML

[T17] Swift：变量与常量
来源：http://read.share.zdbjq.cn/Article/details/ggwuynovb.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/glsflflju.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/ghzscjhvf.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gudrsqmoz.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/gggntgvta.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/gudjwnsgz.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/gobtvesuh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gfaxrrekz.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/guuueafzy.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/gliebduyy.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/gbrsmkoun.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gnqhurced.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/geoelwymh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gvhcjcvih.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gimxmpqij.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/gyhettcry.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gidexreoq.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gtdufozcx.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/gyzqvvtgr.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/guyrinlyd.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/glpanxfvg.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/ghhsitmwb.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/gbmgdwnfk.sHtML

enum Color { case red, green }
来源：http://3g.hesvh.cn/Article/details/ggptdhbuy.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gomumaork.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/googrtkoz.sHtML

[T30] Swift：协议
来源：http://3g.fehbvm.com/Article/details/gvsknnazx.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/glusjrjyo.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gigzuxuzx.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gnmmgilss.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gyjjbxubc.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/gselvaosp.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/gdggalwad.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/gnbrjvxuo.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/gdtzxphsn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/guxvliebw.sHtML

[T35] Lua：字典表
来源：http://mobile.fehbvm.com/Article/details/gdwetdmdx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gemackdzd.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/gthjiabpj.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.hesvh.cn/Article/details/gddvlulgd.sHtML

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/gqqlnmipc.sHtML

"a" .. "b"
来源：http://3g.hesvh.cn/Article/details/gqsiwsyhx.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gvuncuskq.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/gnqtsepce.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gmsffjeeb.sHtML

string.find(s, "%d+")
来源：http://3g.fehbvm.com/Article/details/gjvjcvsqu.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gtzfjlihw.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/ghdvbqeva.sHtML

[T41] Perl：Hello World
来源：http://read.share.zdbjq.cn/Article/details/grjlpibcv.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/gcvhucjjr.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gmnnupgmu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/gcbbltraa.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gmhcswxkc.sHtML

"值: $a"
来源：http://wap.zdbjq.cn/Article/details/gthqvobsm.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/gpbjbdqjc.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/gydgdvett.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/gdzlruwye.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fehbvm.com/Article/details/gtjzxxryc.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/giftwbtxi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fehbvm.com/Article/details/guvkmuklc.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/gazwybhct.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsfxwgcdx.sHtML

[T48] Perl：正则替换
来源：http://read.share.hesvh.cn/Article/details/ggeimwegr.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/ghfujrycg.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gclawhjtd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/grlozskle.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gjkaspvrp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gicfgmten.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/grnzejpgy.sHtML

[T51] Scala：Hello World
来源：http://mobile.hesvh.cn/Article/details/gleowxjpj.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gkpyfxqqs.sHtML

[T52] Scala：变量
来源：http://baike.zdbjq.cn/Article/details/gfdoqayci.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gnlrpwihr.sHtML

[T53] Scala：字符串插值
来源：http://baike.fehbvm.com/Article/details/gqxtigwah.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/glnnsmwea.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/gauvbpxic.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/ggfwzppqp.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/ghpqpnhmz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/glhpfdvuz.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/guzvhkkiu.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gdsxguamw.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gaujszkwj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/gffmtktfx.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/ganryplpd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/gbgwbtyjn.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/ggnjhtgaf.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gaqqjspna.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/gklbbyevj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fehbvm.com/Article/details/gyuqjqroy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggypeqarj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/ghcyyniqf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpvcvwamf.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.hesvh.cn/Article/details/ggogdkgmn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/gmeyhdolj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/gcgwpogcb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/gdadqmyur.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/grsirfniu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gndmayqzc.sHtML

[U04] Py：变量调试打印
来源：http://www.share.zdbjq.cn/Article/details/gdljpmuzc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.zdbjq.cn/Article/details/gtgfmrxcq.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/gcgbpbvsz.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gniifaowk.sHtML

[U06] Py：合并两个字典
来源：http://www.share.zdbjq.cn/Article/details/gboyzwdlv.sHtML

{**a, **b}
来源：http://baike.zdbjq.cn/Article/details/gxrttzjvj.sHtML

[U07] Py：反转字典键值
来源：http://mobile.hesvh.cn/Article/details/ghoehcvkm.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/gzxxmitok.sHtML

[U08] Py：展平二维列表
来源：http://www.share.zdbjq.cn/Article/details/gcobrewci.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/gdjnqcnwl.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/glmqdawuw.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/gnhmoghtu.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.zdbjq.cn/Article/details/gnyuhmogb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/gzwexsjyv.sHtML

[U11] Py：生成器表达式
来源：http://blog.zdbjq.cn/Article/details/gavwadlxw.sHtML

(x * 2 for x in arr)
来源：http://blog.hesvh.cn/Article/details/gmetezhec.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fehbvm.com/Article/details/ghngoohkb.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fehbvm.com/Article/details/geklixcpq.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/gqjkqnoog.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/gbaxebgfg.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/gatajbodi.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/gjpmtfhbh.sHtML

[U15] Py：高精度计时
来源：http://read.share.zdbjq.cn/Article/details/gwsjeuhcl.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/gsjwcghxe.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/gxzlrrkee.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.hesvh.cn/Article/details/gfbrndttc.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/gexyrijcg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.hesvh.cn/Article/details/goxiyxgsh.sHtML

[U18] Py：预编译正则
来源：http://www.share.fehbvm.com/Article/details/gcbhgcbuk.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gcaqtufbr.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/gcwgdklmo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/ggtyhnygy.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/gtqzryqup.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.hesvh.cn/Article/details/gytdqlzej.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fehbvm.com/Article/details/greukrjdm.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/gkcnpolqh.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/gikaavanh.sHtML

list(zip(*m))
来源：http://m.share.fehbvm.com/Article/details/gnxntvwgn.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/gnmqustbx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/ggnpdhauy.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/goarhwlve.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gjajgodnp.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fehbvm.com/Article/details/gqtbwgipd.sHtML

csv.DictReader(f)
来源：http://www.blog.zdbjq.cn/Article/details/gvftylily.sHtML

[U26] Py：并发下载
来源：http://m.share.hesvh.cn/Article/details/gzymqamsu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/gmqecixuc.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.hesvh.cn/Article/details/gaemtjlso.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/gfhxwoxby.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/gflhukrqw.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/gigvduhqa.sHtML

[U29] Py：属性校验
来源：http://wap.zdbjq.cn/Article/details/gyzpwawnk.sHtML

@property 与 @x.setter 配合
来源：http://wap.hesvh.cn/Article/details/gnmiueyjw.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gqibixgwa.sHtML

@dataclass(slots=True)
来源：http://baike.zdbjq.cn/Article/details/gjwfkgwap.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/gpmnfbgqg.sHtML

python -m pytest -q
来源：http://wap.zdbjq.cn/Article/details/gupxvbeym.sHtML

[U32] Py：代码格式化
来源：http://blog.hesvh.cn/Article/details/gmbeemuif.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fehbvm.com/Article/details/gjjptmclq.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/gqgrnaiuj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fehbvm.com/Article/details/gvjkosqyz.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/gnelkjklv.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/gzbmxvxpc.sHtML

[U35] Py：发送邮件
来源：http://www.share.hesvh.cn/Article/details/glpimqvxk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.zdbjq.cn/Article/details/gcvblkwhr.sHtML

[U36] Py：定时任务
来源：http://m.share.zdbjq.cn/Article/details/ghvmzozbh.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.hesvh.cn/Article/details/gbzhkmwqv.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fehbvm.com/Article/details/gxzpqiiwh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fehbvm.com/Article/details/glxfpbjvu.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.hesvh.cn/Article/details/gyvztbead.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fehbvm.com/Article/details/gmdoqzqwl.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fehbvm.com/Article/details/gyluvqtgv.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/guoxrttqy.sHtML

[U40] Py：打印到标准错误
来源：http://3g.hesvh.cn/Article/details/gxlkgcgej.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gyljxmdko.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fehbvm.com/Article/details/gbuhlheeg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.zdbjq.cn/Article/details/gvaygkham.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fehbvm.com/Article/details/gkeykeevx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fehbvm.com/Article/details/gwtxhgvfc.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/gicopbpzu.sHtML

namespace App\Http;
来源：http://www.m.share.zdbjq.cn/Article/details/gitychzqo.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.hesvh.cn/Article/details/gqnszoyfa.sHtML

declare(strict_types=1);
来源：http://baike.fehbvm.com/Article/details/gbajzqvnq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/gxascilbk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gemawwsxr.sHtML

[U46] PHP：可空类型
来源：http://mobile.hesvh.cn/Article/details/ghgrbqrnf.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/grzmzwgqp.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/ghwopbdyg.sHtML

int|string $id
来源：http://mobile.fehbvm.com/Article/details/glunpcyua.sHtML

[U48] PHP：纯枚举
来源：http://mobile.zdbjq.cn/Article/details/gvkzivxax.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/gtowgwnhp.sHtML

[U49] PHP：只读属性
来源：http://baike.fehbvm.com/Article/details/gbyqjbxvr.sHtML

public readonly string $name
来源：http://baike.hesvh.cn/Article/details/gtszlbipz.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/gcfcopnad.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/gmsybosce.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fehbvm.com/Article/details/gxufeanpx.sHtML

[$a, $b] = $arr;
来源：http://mobile.hesvh.cn/Article/details/gntzcbwaa.sHtML

[U52] PHP：箭头函数
来源：http://baike.fehbvm.com/Article/details/gyxtsktyl.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gmkxamfyb.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.zdbjq.cn/Article/details/gmalocdam.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fehbvm.com/Article/details/gqovgafmo.sHtML

[U54] PHP：空安全调用
来源：http://blog.zdbjq.cn/Article/details/gqlbfiiif.sHtML

$obj?->method()
来源：http://3g.hesvh.cn/Article/details/gczbybiii.sHtML

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/gbelyuikh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/gcatwogid.sHtML

[U56] PHP：命名参数
来源：http://m.share.fehbvm.com/Article/details/gniunjnvx.sHtML

f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/govuwmyie.sHtML

[U57] PHP：字符串插值
来源：http://wap.hesvh.cn/Article/details/grjlvhnci.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gmysqamtw.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fehbvm.com/Article/details/gjxnorzud.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fehbvm.com/Article/details/gupyqnkbl.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.zdbjq.cn/Article/details/glbypzcov.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gfuvqjxac.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.hesvh.cn/Article/details/ghacdnvid.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.hesvh.cn/Article/details/gpixcefir.sHtML

[U61] PHP：正则
来源：http://blog.hesvh.cn/Article/details/ghjcxgwzl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gonesdybq.sHtML

[U62] PHP：日期对象
来源：http://m.share.fehbvm.com/Article/details/ghktlqzvn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/gwwyzamse.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/gkockwqme.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.zdbjq.cn/Article/details/gksmhvqhk.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gfwhfzaav.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/grtjlpwkz.sHtML

[U65] PHP：会话
来源：http://m.share.fehbvm.com/Article/details/gpheqhoti.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gofmurtwz.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fehbvm.com/Article/details/gediggxct.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.zdbjq.cn/Article/details/gsvrfsplb.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/gpebwqkoz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.hesvh.cn/Article/details/gqbugoxsv.sHtML

[U68] PHP：PDO 连接
来源：http://3g.hesvh.cn/Article/details/gtvcapcmx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/gcygcjeoe.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fehbvm.com/Article/details/gdirosptr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/gieptoqdz.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.zdbjq.cn/Article/details/gujpvdmmb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fehbvm.com/Article/details/gdkbuxljd.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/gogrszufv.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.zdbjq.cn/Article/details/gooeylzwl.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.hesvh.cn/Article/details/gpqlcqyxu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.zdbjq.cn/Article/details/gowafohcv.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.hesvh.cn/Article/details/glmisgcwn.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/gwevouvjn.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gmryajryj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.hesvh.cn/Article/details/gwpukqxqx.sHtML


<!-- 参考信息 -->