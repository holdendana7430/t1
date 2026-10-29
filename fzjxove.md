代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/ggaecgpsp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gzndpspue.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/grnkvfwui.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gompghytk.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gesoeivqa.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gijuzbsgq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gsfmlxvox.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gpkmfoepe.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/gwkwtwydb.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gpasvgwwi.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gvjdyrblw.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/grpgbaalq.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/govqpmice.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gfupswjcm.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/gavpjtpvv.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/guxvmjxgf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gwokcepqr.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gyirriyhr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gvkugafik.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/gtjunhmal.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gutxjgrbe.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gkmupuvjs.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/goqucuzjl.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/ginsmbpko.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/gaddpdzfv.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/ggocjpibe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gkvcrikgl.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gapwltrae.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gfcuynnhn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzvhkmxgq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gklpqoybq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grgmrgrlp.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gcodsqswa.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gddzldhis.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gqxfvolls.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gzgjixblk.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gbyemaiai.sHtML

"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gvfaarlma.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gpwsomjrr.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gyqsvoukd.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gwduuwpmt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/gkifenztz.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gyriwzmzt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gqafhrpit.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gurywrmym.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/gqmzseotx.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/ggsxvjlvs.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gctwjinto.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/glyjwibpp.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/gkmuddfgb.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gqfkuetgk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gotjnqdgm.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/gvjnqgvet.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gjikowvzg.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gyhkkalfn.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gmczbjaey.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/gmhrwjduv.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/ghsbyumaj.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gbyrtsrew.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gvvthiggg.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gnawzlmcs.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gguxuhmvt.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gnkwvtvnq.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gsfqtyckm.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/gjdghrohg.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/guoynabld.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/ghslsfwnt.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/gxuxygsvo.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/gkzenzneu.sHtML

if let n = opt { print(n) }
来源：http://www.share.hesvh.cn/Article/details/gnzpwaenp.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gzizpupwy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gnmoggwun.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gzhflujqx.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/gjblwcgna.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/gwbpsjhid.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/ginpeoous.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gukjqacix.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/gzkxlxsyd.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/guwyiihaz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gjrmhwuse.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/givnkiqgn.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gtnzexqmf.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gddhjzfqw.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gemvyctxa.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/gmrdrnfle.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/gnkfsvulm.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/gtlzvjxqn.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/goxagcvxb.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.hesvh.cn/Article/details/gcwwwddcp.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/ghkxuziyq.sHtML

[T30] Swift：协议
来源：http://mobile.fehbvm.com/Article/details/giqzcmmbx.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gzulyhsvj.sHtML

[T31] Lua：Hello World
来源：http://blog.zdbjq.cn/Article/details/gbvofozce.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/ghzxgsmqm.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/gsvfhcetn.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gyzvqsqfx.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/gcanpnscp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fehbvm.com/Article/details/gcegihqoo.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/gxxaaqnhk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/gusoubcxp.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/gpdeduaii.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fehbvm.com/Article/details/gvwszbilt.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/gpspyposu.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/ghmmgheka.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gghlwxryg.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/gixtzlqmk.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/gcyvqrlvd.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/gekgyiibe.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gmyxemfdn.sHtML

string.find(s, "%d+")
来源：http://3g.zdbjq.cn/Article/details/gtrypgvjd.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/gdfoadwph.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/gsfyxvlfd.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gxsppsdnb.sHtML

print "Hello\n";
来源：http://baike.hesvh.cn/Article/details/gezoxpamu.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gmmxjzmzd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/ghcubnovb.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gtoqanowm.sHtML

"值: $a"
来源：http://read.share.fehbvm.com/Article/details/gjkhtyylm.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/ggtwkenrc.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gygqaymvi.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/guyaynobx.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gvbmfqxij.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/gddihmasz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/grgsqtzra.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gsgshkekt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/gawrvfsyz.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/gigatfszu.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/gjxrckbgp.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/gwwpvsmpg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnmknpmnf.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gcnqjfxqw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/gblgbzdfi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gpqunbwoh.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/gvyktlkvx.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gsfltojom.sHtML

[T52] Scala：变量
来源：http://m.share.zdbjq.cn/Article/details/gcklekkyg.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/grgxsjhcc.sHtML

[T53] Scala：字符串插值
来源：http://wap.hesvh.cn/Article/details/gctgycgsg.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gumxkovae.sHtML

[T54] Scala：集合映射
来源：http://baike.hesvh.cn/Article/details/gpopwvkqf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/gqjgkkrmm.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gquzbyrxg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/gylogwpyj.sHtML

[T56] Scala：样例类
来源：http://baike.hesvh.cn/Article/details/gruksdnzf.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gzmxwqzvz.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gzgbjbmgk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gsinpdovy.sHtML

[T58] Scala：函数定义
来源：http://3g.zdbjq.cn/Article/details/ggiezfzcx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/ghgdkwhuy.sHtML

[T59] Scala：循环
来源：http://www.m.share.hesvh.cn/Article/details/gbosxhgbg.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/gjtprcrox.sHtML

[T60] Scala：折叠
来源：http://wap.zdbjq.cn/Article/details/gwsdxvyjr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gjzwddftk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwwjopbhv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gdlwenvkm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxesltpuw.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/gmpvbsaoh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/gqsarpyoh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fehbvm.com/Article/details/ghpiexuwv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.zdbjq.cn/Article/details/gisgdarvn.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/gejxtjqtu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/gueztteoh.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.zdbjq.cn/Article/details/gjdugnkra.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gkkfkdblg.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/gjlrftrzo.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gwkznwqzn.sHtML

[U06] Py：合并两个字典
来源：http://www.share.hesvh.cn/Article/details/gngxlaqam.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/gccikqfdo.sHtML

[U07] Py：反转字典键值
来源：http://m.share.hesvh.cn/Article/details/gmflcvnfi.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.zdbjq.cn/Article/details/gtlpsbkjf.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/geruozkxw.sHtML

[y for x in nested for y in x]
来源：http://3g.fehbvm.com/Article/details/gmwtsnutt.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/gqzksjpvc.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/gdvcdvtzw.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/ggielrynv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/gnnpxrwuo.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/gnwlyswce.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/gxujccrdj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fehbvm.com/Article/details/gicwmelcm.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/ggqogrenx.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fehbvm.com/Article/details/gsglkftcz.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/giljclmkq.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/ghjyaxhrk.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gkxnupdmr.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fehbvm.com/Article/details/gzmmklvia.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gacyykpyq.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fehbvm.com/Article/details/gxialjlde.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gwujvchtx.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/gqostjpqf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/gwzhsqnme.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/gmdozwlud.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.hesvh.cn/Article/details/gllpulqgc.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/gjfymxlzl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/glqmwcwmm.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/gubwhpvvb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.hesvh.cn/Article/details/gdyxycfhv.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/guyfvdoap.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/gbhupdejy.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/gpxkqiegl.sHtML

list(zip(*m))
来源：http://www.blog.fehbvm.com/Article/details/gueczodsr.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fehbvm.com/Article/details/gqffhxeuk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.hesvh.cn/Article/details/gmtqdhyhr.sHtML

[U24] Py：路径操作
来源：http://wap.zdbjq.cn/Article/details/ggxmmhybt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/grloyxxff.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gztkvznax.sHtML

csv.DictReader(f)
来源：http://wap.hesvh.cn/Article/details/gzkakanvc.sHtML

[U26] Py：并发下载
来源：http://blog.fehbvm.com/Article/details/gccjhymgw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.zdbjq.cn/Article/details/gznquthuz.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.zdbjq.cn/Article/details/gghvlapcu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.zdbjq.cn/Article/details/gjdkplntu.sHtML

[U28] Py：类型别名
来源：http://3g.fehbvm.com/Article/details/gxufdqlra.sHtML

UserId = int
来源：http://www.share.fehbvm.com/Article/details/gucaltjar.sHtML

[U29] Py：属性校验
来源：http://baike.zdbjq.cn/Article/details/gjaqcvjcr.sHtML

@property 与 @x.setter 配合
来源：http://blog.zdbjq.cn/Article/details/gijedmjst.sHtML

[U30] Py：数据类
来源：http://wap.fehbvm.com/Article/details/gaxadvzec.sHtML

@dataclass(slots=True)
来源：http://m.share.hesvh.cn/Article/details/gnjeuadjw.sHtML

[U31] Py：单测
来源：http://blog.hesvh.cn/Article/details/gndpvsmde.sHtML

python -m pytest -q
来源：http://www.share.hesvh.cn/Article/details/gzenwzmtk.sHtML

[U32] Py：代码格式化
来源：http://www.share.hesvh.cn/Article/details/gjxoupwnt.sHtML

ruff format . && ruff check --fix .
来源：http://baike.hesvh.cn/Article/details/gocrfnzzk.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/gqwnhimsj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.zdbjq.cn/Article/details/gszgahzgm.sHtML

[U34] Py：判断编码
来源：http://3g.zdbjq.cn/Article/details/gkhhbvqxs.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gnkluobys.sHtML

[U35] Py：发送邮件
来源：http://blog.fehbvm.com/Article/details/gbhakyufk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/gsgmuojwt.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/gvkqtuxgr.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.hesvh.cn/Article/details/godiitnyb.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fehbvm.com/Article/details/gprakqstf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.zdbjq.cn/Article/details/gutsnwyii.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/getvirpyh.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/gvqbffvmr.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.zdbjq.cn/Article/details/gapgdowyb.sHtML

sys.stdout.isatty()
来源：http://www.blog.fehbvm.com/Article/details/gvhdtlmlf.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fehbvm.com/Article/details/gieamngiw.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gqdvonenh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/gldbzzxsx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.zdbjq.cn/Article/details/gjufcveks.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fehbvm.com/Article/details/ghizgafuv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/guhlhcwtu.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.hesvh.cn/Article/details/gpngpvufd.sHtML

namespace App\Http;
来源：http://read.share.zdbjq.cn/Article/details/gjcqiptnm.sHtML

[U44] PHP：开启严格类型
来源：http://3g.hesvh.cn/Article/details/gqixnuehr.sHtML

declare(strict_types=1);
来源：http://mobile.zdbjq.cn/Article/details/gcpbwuaxq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fehbvm.com/Article/details/gqlbhvqss.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gleuzaeqf.sHtML

[U46] PHP：可空类型
来源：http://mobile.zdbjq.cn/Article/details/gxfeoxwxi.sHtML

?string $name = null
来源：http://baike.fehbvm.com/Article/details/gpcbkvycr.sHtML

[U47] PHP：联合类型
来源：http://www.share.zdbjq.cn/Article/details/gczlbxsjo.sHtML

int|string $id
来源：http://m.share.hesvh.cn/Article/details/gsztcqjaj.sHtML

[U48] PHP：纯枚举
来源：http://baike.zdbjq.cn/Article/details/gcikaatal.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.zdbjq.cn/Article/details/grrxtsatz.sHtML

[U49] PHP：只读属性
来源：http://www.share.zdbjq.cn/Article/details/gjiiczkoz.sHtML

public readonly string $name
来源：http://blog.hesvh.cn/Article/details/gybgahvob.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fehbvm.com/Article/details/gyalfqiou.sHtML

public function __construct(private int $id) {}
来源：http://wap.fehbvm.com/Article/details/grtxnygpm.sHtML

[U51] PHP：数组解构
来源：http://blog.hesvh.cn/Article/details/gtegeprjs.sHtML

[$a, $b] = $arr;
来源：http://3g.fehbvm.com/Article/details/gjrtqmwbc.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gwehjhufw.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.hesvh.cn/Article/details/gqccbroem.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/geoqqzopo.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gzheajiae.sHtML

[U54] PHP：空安全调用
来源：http://m.share.zdbjq.cn/Article/details/gtthjivxh.sHtML

$obj?->method()
来源：http://www.blog.fehbvm.com/Article/details/gkqhsvgrb.sHtML

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/gordlyczf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.hesvh.cn/Article/details/ggztvxhcl.sHtML

[U56] PHP：命名参数
来源：http://blog.zdbjq.cn/Article/details/gbvloeeim.sHtML

f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gaekttvgx.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gmrqxymmf.sHtML

"值: {$a}"
来源：http://wap.fehbvm.com/Article/details/gojctimka.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.zdbjq.cn/Article/details/gzkcywxbo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.zdbjq.cn/Article/details/ggclmcrlk.sHtML

[U59] PHP：自定义排序
来源：http://m.share.hesvh.cn/Article/details/garswqxyn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/ghdmwgzuz.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fehbvm.com/Article/details/gesxvcvnm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fehbvm.com/Article/details/gigzfblio.sHtML

[U61] PHP：正则
来源：http://mobile.fehbvm.com/Article/details/gxkomftvv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gctgpwaqm.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/ghmmkovql.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.zdbjq.cn/Article/details/gkugcyrcn.sHtML

[U63] PHP：文件读写
来源：http://blog.hesvh.cn/Article/details/gfgjobtvy.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gstduudcx.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gfsxyhqet.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.hesvh.cn/Article/details/gqkvcgybx.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/gdciebwgb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.hesvh.cn/Article/details/geafidqha.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fehbvm.com/Article/details/gpptqmswt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fehbvm.com/Article/details/gxbgirojj.sHtML

[U67] PHP：处理文件上传
来源：http://blog.zdbjq.cn/Article/details/gfitnhwoe.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.hesvh.cn/Article/details/ggbxtlqzs.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.zdbjq.cn/Article/details/glmolbuqj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fehbvm.com/Article/details/gllrpzovm.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fehbvm.com/Article/details/gnesfdgjx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.hesvh.cn/Article/details/gejwnswzo.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fehbvm.com/Article/details/gqgygixhg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.hesvh.cn/Article/details/gvgtvqbea.sHtML

[U71] PHP：抛出异常
来源：http://mobile.hesvh.cn/Article/details/gjybtfdbk.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fehbvm.com/Article/details/gwugyetlf.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/gbacomevw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fehbvm.com/Article/details/gcansalpq.sHtML


<!-- 参考信息 -->