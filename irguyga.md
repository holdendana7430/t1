代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gqviayrsr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gqxjkmjlg.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gxwdvkgsr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gznedroyl.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gfpunxjgs.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gbqjqmgql.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gofqtdvkf.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/gcobizhub.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gtdaclheb.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gpxvpffqt.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gmsgpblbx.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gofcafuzu.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gsosjupyi.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gcrvzyrif.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/gxgpozywx.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/geheepglw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gepodacrp.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gxmyifewv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gafrcvjfv.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gmnpfgzbu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/ggpoccsrm.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/guewzuban.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gtlqkdatm.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gqrhpwfhn.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gfabdsuiv.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gztiznxvq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gqvgulpzi.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gjqddisur.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/grtrnjuqu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdpgqhhzu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gpwqoyjae.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gaeaokjbr.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gtvfprgvf.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/goibhejsd.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/getiathgd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/glvnxmiee.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/gziqpxvhw.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gpkqlvats.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/gfrjxqhjv.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gppnuqoez.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/glylnnshc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gpartknlo.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/ghairlyeq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gbjbpnemw.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gwglktbqi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gztuyrbbq.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/gyiemglok.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gdkcwongu.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/gieermqbm.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/gcrohvgyq.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gohsbrmqg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/gnymuiwld.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/gpoygsalo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/gtcioqrxa.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/glgwqhcln.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gddykxgcc.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gathjlbzv.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gwfsujnzx.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/ggbytvbka.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gprltnygi.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/gameptgll.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.zdbjq.cn/Article/details/giospyziz.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/ghaunzpda.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gsgfbhptt.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/gxzafgvql.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gcyrkwzln.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gzizoxdhp.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gdcktsiuy.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gznjxinws.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/gvessezfu.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gjzmmjgfz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/ghrnqyyup.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gitcauzps.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/ghuiodwhb.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gegminoin.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/gptgsgfuq.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gozgnnmwy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/gpgypmxnz.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gnkdfamwt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/guohysayq.sHtML

[T25] Swift：结构体
来源：http://3g.zdbjq.cn/Article/details/gxrdyhctx.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/gfyzlgbsv.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/garhminwm.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/gnwqvqxne.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gtqgnharc.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/gkhekdhqy.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/ghjoapprz.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/gnkbtfuxv.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.zdbjq.cn/Article/details/gflapmlmx.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gcjdmudxp.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gpnofczjo.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fehbvm.com/Article/details/goorjdtnw.sHtML

[T31] Lua：Hello World
来源：http://3g.hesvh.cn/Article/details/gilclcyhm.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/ggrgbslsd.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/gzfphpumo.sHtML

local a = 1
来源：http://m.share.fehbvm.com/Article/details/gjzaycqtt.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gaticprnq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gkdexmzaa.sHtML

[T34] Lua：遍历表
来源：http://baike.hesvh.cn/Article/details/guxgioncn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/gcfxenaff.sHtML

[T35] Lua：字典表
来源：http://3g.fehbvm.com/Article/details/gsjfbnnzh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gfhhfsnch.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/gejrfudgl.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/gaxsusikh.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/guufugxyb.sHtML

"a" .. "b"
来源：http://3g.hesvh.cn/Article/details/gujcywlyv.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gapsirpxf.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gdtmmxfhb.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gfhqhjnws.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/gmawfrhcu.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/gpdkpmime.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/guzobdjzq.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/gztttyawv.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gtcodrhxn.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/gaqunxeff.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gqcliboht.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/ghgqtdrqm.sHtML

"值: $a"
来源：http://www.m.share.hesvh.cn/Article/details/gqdsnzdxh.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/gwpyxauwj.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsxibgkya.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/guemmblue.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/gwobzahep.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gckiqkwko.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fehbvm.com/Article/details/gkgdyoevh.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fehbvm.com/Article/details/gpyrhrywi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/gaktxetjc.sHtML

[T48] Perl：正则替换
来源：http://mobile.fehbvm.com/Article/details/gzkpfnrlb.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.zdbjq.cn/Article/details/gswqtbucr.sHtML

[T49] Perl：函数
来源：http://www.m.share.fehbvm.com/Article/details/grykwxpjw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gerghwzwd.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gtvzhkxfm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.zdbjq.cn/Article/details/ggpecmgit.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/ggtxxborg.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/gvkopxeyt.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gpctocbyz.sHtML

[T52] Scala：变量
来源：http://m.share.hesvh.cn/Article/details/gwmhsqwfu.sHtML

val a = 1;  var b = 2
来源：http://baike.fehbvm.com/Article/details/gajftnhlm.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gkhyhnikb.sHtML

s"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gufckwogm.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gynmjapma.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.zdbjq.cn/Article/details/grpvmkudg.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gahuuqmzf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/garmcbkrf.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/gjgabajjn.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fehbvm.com/Article/details/gkpowajxr.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gzumafhdw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/gslebqrnt.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/gpenloylc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.hesvh.cn/Article/details/gaboaxodk.sHtML

[T59] Scala：循环
来源：http://blog.fehbvm.com/Article/details/gezobbudv.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/gycwmbopo.sHtML

[T60] Scala：折叠
来源：http://www.share.hesvh.cn/Article/details/gbpblwvhw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/gtcxioqdq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggulnwtwj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gbfklxbvl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gybjghxjr.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.zdbjq.cn/Article/details/gehsqsttc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/gjuddmruf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/gtqzcgaaw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/glhuzrzbf.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.zdbjq.cn/Article/details/gpkiezzdl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/gyotrryua.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.zdbjq.cn/Article/details/gwglwvira.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/gumipwzai.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/gghruxavl.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gsimupmcm.sHtML

[U06] Py：合并两个字典
来源：http://baike.hesvh.cn/Article/details/gbiuizhfw.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/gzbakrtpy.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/gbxwdtupa.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/gjhlkxdzr.sHtML

[U08] Py：展平二维列表
来源：http://wap.zdbjq.cn/Article/details/gmlobkfjd.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/gytierxwc.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/gpenoullp.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/gtcnvfhcy.sHtML

[U10] Py：按值排序字典
来源：http://mobile.zdbjq.cn/Article/details/gwarhdjdd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/gtdkkahqc.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/gdayvtyqq.sHtML

(x * 2 for x in arr)
来源：http://blog.fehbvm.com/Article/details/gfcrgussg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/gnvtiwrpw.sHtML

Counter(arr).most_common(3)
来源：http://www.share.zdbjq.cn/Article/details/ghzhosgdo.sHtML

[U13] Py：固定长度队列
来源：http://blog.hesvh.cn/Article/details/gulsntxiv.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gxgrqqlyy.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.zdbjq.cn/Article/details/gejdpgwsf.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/ghwuhbouw.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.hesvh.cn/Article/details/gnrbkvjzd.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/ggukhlolt.sHtML

[U16] Py：命令行参数解析
来源：http://baike.zdbjq.cn/Article/details/gjozcbhum.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.zdbjq.cn/Article/details/gcknxxzvu.sHtML

[U17] Py：初始化日志
来源：http://3g.fehbvm.com/Article/details/glkgsilwt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.zdbjq.cn/Article/details/gscwuxpmc.sHtML

[U18] Py：预编译正则
来源：http://wap.hesvh.cn/Article/details/gcimzbfur.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gqxsvuyif.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/ghsqfeipe.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/gadhdqxpo.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/gncvmvgzc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gqtfectpp.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/gdojinuwu.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/gokudbzzh.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/gejtoddjw.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/grkunapfg.sHtML

[U23] Py：分块读取大文件
来源：http://blog.zdbjq.cn/Article/details/ganlblbvf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.hesvh.cn/Article/details/gfkrkylsw.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/gtlyqzcwd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gzslropig.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gcvhkjbxu.sHtML

csv.DictReader(f)
来源：http://wap.fehbvm.com/Article/details/grfpvqxmt.sHtML

[U26] Py：并发下载
来源：http://baike.fehbvm.com/Article/details/gluitnoqf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/grinbffbx.sHtML

[U27] Py：异步 HTTP
来源：http://blog.zdbjq.cn/Article/details/gwuyjcjbf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fehbvm.com/Article/details/gtkasnddk.sHtML

[U28] Py：类型别名
来源：http://www.share.hesvh.cn/Article/details/gtgclgwea.sHtML

UserId = int
来源：http://3g.zdbjq.cn/Article/details/gwidvsvtn.sHtML

[U29] Py：属性校验
来源：http://read.share.hesvh.cn/Article/details/gwysggdxd.sHtML

@property 与 @x.setter 配合
来源：http://www.share.zdbjq.cn/Article/details/gobislbdp.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/gufgoldsi.sHtML

@dataclass(slots=True)
来源：http://www.blog.hesvh.cn/Article/details/gixidfrlo.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/gzzaqobwt.sHtML

python -m pytest -q
来源：http://www.m.share.hesvh.cn/Article/details/gnzupgqix.sHtML

[U32] Py：代码格式化
来源：http://wap.fehbvm.com/Article/details/gpjpvgtcj.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/gbyidabow.sHtML

[U33] Py：打包发布
来源：http://baike.zdbjq.cn/Article/details/guferxsmf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/grmsoxexz.sHtML

[U34] Py：判断编码
来源：http://www.blog.fehbvm.com/Article/details/gggdtpetw.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/gfckygnze.sHtML

[U35] Py：发送邮件
来源：http://www.blog.zdbjq.cn/Article/details/gxdhpzeaw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.zdbjq.cn/Article/details/gyyuvxcmi.sHtML

[U36] Py：定时任务
来源：http://mobile.hesvh.cn/Article/details/gernocftx.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fehbvm.com/Article/details/gbzqflfgt.sHtML

[U37] Py：读写 Excel
来源：http://blog.zdbjq.cn/Article/details/gisibvwjz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.zdbjq.cn/Article/details/gtxqzsbmn.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/grotbpbsw.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gedtqovtn.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/gkbgtprpl.sHtML

sys.stdout.isatty()
来源：http://blog.zdbjq.cn/Article/details/gslglzaoj.sHtML

[U40] Py：打印到标准错误
来源：http://baike.hesvh.cn/Article/details/gaspdktzg.sHtML

print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/glitrzhcd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.zdbjq.cn/Article/details/gpqpscquq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.hesvh.cn/Article/details/gdslrckmk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.hesvh.cn/Article/details/gfzeucygc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/gezoootgb.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/gtfqljoio.sHtML

namespace App\Http;
来源：http://www.blog.hesvh.cn/Article/details/gqluhrddb.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/glghuyosi.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/gwhgmgdin.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/grloxyvti.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gontqdcro.sHtML

[U46] PHP：可空类型
来源：http://wap.hesvh.cn/Article/details/gdwsglrtc.sHtML

?string $name = null
来源：http://www.share.zdbjq.cn/Article/details/gotjcaybp.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/gdrvdyeok.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gdkuvqxga.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/gixfktkko.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.hesvh.cn/Article/details/gheckieon.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.hesvh.cn/Article/details/gafrhqdbu.sHtML

public readonly string $name
来源：http://mobile.zdbjq.cn/Article/details/groqfrtfq.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fehbvm.com/Article/details/gaqgcnvrq.sHtML

public function __construct(private int $id) {}
来源：http://baike.zdbjq.cn/Article/details/gtcycmuxe.sHtML

[U51] PHP：数组解构
来源：http://3g.hesvh.cn/Article/details/gdxkeglbj.sHtML

[$a, $b] = $arr;
来源：http://www.share.fehbvm.com/Article/details/gcdipinxi.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gtcwzhean.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fehbvm.com/Article/details/giaouetrz.sHtML

[U53] PHP：空合并运算符
来源：http://3g.hesvh.cn/Article/details/gtoltroug.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/gqnetlezb.sHtML

[U54] PHP：空安全调用
来源：http://mobile.hesvh.cn/Article/details/gzycdirkn.sHtML

$obj?->method()
来源：http://baike.hesvh.cn/Article/details/grdfmlqol.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fehbvm.com/Article/details/gjuxboumm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gzquycivr.sHtML

[U56] PHP：命名参数
来源：http://wap.zdbjq.cn/Article/details/gvnzgrvgw.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gzpdqlvyt.sHtML

[U57] PHP：字符串插值
来源：http://baike.fehbvm.com/Article/details/ganhjmzqh.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gzxhbzxfx.sHtML

[U58] PHP：数组三件套
来源：http://baike.hesvh.cn/Article/details/gviwkgvph.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fehbvm.com/Article/details/gderlwngh.sHtML

[U59] PHP：自定义排序
来源：http://read.share.zdbjq.cn/Article/details/gvetfojzh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gtkzwjpfg.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.hesvh.cn/Article/details/gcxyievga.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.hesvh.cn/Article/details/gdxfjnryo.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/gqsqxemvd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gzmtlxdvc.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.hesvh.cn/Article/details/ghqxodchh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/gsvfntdqx.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/gctqbdrve.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/gpkyotuqg.sHtML

[U64] PHP：目录遍历
来源：http://mobile.hesvh.cn/Article/details/gkxoanabv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fehbvm.com/Article/details/ggpkeglae.sHtML

[U65] PHP：会话
来源：http://blog.zdbjq.cn/Article/details/glksdhacd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.hesvh.cn/Article/details/ghbeduadk.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.hesvh.cn/Article/details/gjaocxjde.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.hesvh.cn/Article/details/gtilbvetl.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fehbvm.com/Article/details/gutsktunc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.zdbjq.cn/Article/details/gsikuvnhb.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.zdbjq.cn/Article/details/gtjkmfazu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fehbvm.com/Article/details/gzyhdlrmq.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.zdbjq.cn/Article/details/gbipsbzap.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.hesvh.cn/Article/details/gmegiabio.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fehbvm.com/Article/details/gxcnficas.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.hesvh.cn/Article/details/gvjirrtan.sHtML

[U71] PHP：抛出异常
来源：http://mobile.hesvh.cn/Article/details/gskehdlxj.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gxecaxkht.sHtML

[U72] PHP：写错误日志
来源：http://read.share.zdbjq.cn/Article/details/gkaelorhb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.zdbjq.cn/Article/details/gmuagcflc.sHtML


<!-- 参考信息 -->