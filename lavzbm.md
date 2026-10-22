代发 wailian999

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2wdegzcwq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2yecjtxgn.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2txerpxfz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2atabtkux.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ydsnchrf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2zujhhzyt.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ndfamifc.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2mbpuebaw.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2hefvwqpk.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2gdovweyf.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2lggvhhoo.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2dsrbkpcd.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2hymdbiym.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2bbydfdpo.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2pcccdodz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtidgmfg.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2oxssgjeh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2kiwbygyv.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xnsxesbh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2brrqdxkl.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2evpzcqxo.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2aofryttk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2krshkenx.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2hyyxplrw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xvewafuu.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2dzeadeqo.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2pxwraiko.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2qrvnygrd.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2stbokkfd.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2szfapvld.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2lgyjlwwr.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2fckpiolo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2iihobrvl.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2fntuxulr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2qaswquwv.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2qskajupc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2djeikzmw.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2cnoqybyn.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2bpnmadqg.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2nymlgvpw.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jokaznyi.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2thrdapke.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2fkyygmoy.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2pinuuqcw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2xqkuxhfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2erdgsung.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2amtsvdjk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2piyofdtr.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2obsbqgpd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ntsamxxw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2tnvurles.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2naoouaac.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2plibjged.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2rpvvzdsp.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2zxgkglpx.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2kcvhqlsh.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fnlmzysg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2blvqchnt.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2yynhfvig.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2abdbentb.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jtmffvsw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2pfakyxpp.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2oztmeguw.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2qukwwaib.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2wnbgwkxs.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2umegwedr.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2yogphinl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2oxumquth.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2rhrxqofk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2xwugxguq.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2qcrkumin.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xgjhhkgb.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2hnrpbaoe.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2futxrudu.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2zjlegagp.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2mhtesspi.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2zdnlzznq.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2erktkcrf.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2htksutyr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2sxagozme.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2yezioibr.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2cqxhxkpc.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ovjfagpl.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2dxwnetyu.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ytdxqhnl.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2lugryqvb.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2tvkaobsw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2kdyaxkxa.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2dhrzygqb.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2mscihjyr.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2kvmtmrda.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ydllmive.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2lgelfltv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2okqqkico.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2emftaffk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zkbnwrmh.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2rifvaemc.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2cicqguau.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2ojgofhbs.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2olixsdia.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2rbiksqlj.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2ubcjbmbh.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2srfmubzv.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2wtsjxyao.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2gkznzsms.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2xmkydlea.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2haevochd.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2owqmxobp.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jmsafoca.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wcfkxrco.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2yayzxckz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2evwmgxnh.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2yafdrkbg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2fknivzyq.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2vlfgtgte.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2sizwxxyb.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2yyashvch.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2rmbprrvs.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2dwaaelmb.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2snnaapfd.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2rdsdkpkq.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2facjllfc.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2vvsghrsi.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2dglmpbhz.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2eqtyakwg.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2pbckqqmp.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2hblswwnd.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2wgyxvzab.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dwbhjiwn.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2jfzgbjlp.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2cmybnrkn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2djnqrxbw.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2tpgbqzys.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2lsjtxmbv.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ubupgdun.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xahzxgbv.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ymyoxpgy.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2hrcyimuh.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2lbbitmcs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqoffjks.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2gqixwhnq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2keagsujo.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ezpgjbfs.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2zmbztgqc.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2zumzmdkr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2dhvhcoeq.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mbfahclr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2hmccksjd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2xvcregqr.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ilbqsbgs.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hlcyobrk.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2hnuqmued.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gyxmpkxq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2heosxzdr.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2dhpwwhsg.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2irdwzhoy.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hbqziikk.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ohczijfh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2jyxtsvma.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2lwvqjfjb.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ichfbvks.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2upzrugpk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2oqgksbzs.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2vdxzjcvz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2mnzmytsl.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2lfnghmez.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2vxjtbllx.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2mciqbjwj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2fsjxvygp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iuxeizlf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aqdsttjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rovvshqd.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2zuqvlhxi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2merlfits.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2arzfysct.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yeemmvkp.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ojldtaqp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2adodrcxy.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2lgclclbx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2eqkjtekt.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2mmininhp.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2sbplsjep.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2uznqniok.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2apidlnbr.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2rlvaxocn.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2kdwzfxex.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2iepimrxe.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2rzukatnk.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2wkifvocg.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2vwlfbumz.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2hicmhvmk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2tsaltlkl.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2oantmhrl.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yajjdpye.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2wcxrqitr.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2abkwmsna.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2dkzalsrc.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2woxzmizc.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2fcocazmg.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2mrcckkit.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2edafzbiw.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2grlejtec.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2rvxxnzyl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2kdbtqcou.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2akpfccdi.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2jopckezi.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2psfpzoqr.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2datzylpa.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2izdecrsq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2vuwtignc.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2fuubjeix.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2lntyetbb.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2iemcfsew.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2hlqdwkte.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2awpromew.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2hskdrcou.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2vwpxmumu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2cqkmobqp.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2nrmjojgr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gmbcvbjn.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2fvyqfcnh.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2hsynidzd.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2oxlnptxo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2suplhqqu.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2xmtlcoft.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2aujkdyvu.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2lmcrpkrp.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2syrrdrjf.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2yzrigvyc.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2wsovffcs.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2udsgndhw.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ftirbzdx.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2owxlxgcz.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2gmeljjdd.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hwmjoykn.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2zbmpkatx.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2kbtymaia.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2wmhvwlky.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2pqlhbkfs.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2bfwgegkm.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2lczvezsu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2ykajzyrq.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2kpabhjlj.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2ttrfgysv.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2zuwnuauq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2hsmcifxr.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2hwdofeua.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2wcbfobhp.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2eycipcco.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2ryqzzcec.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ysuenkrl.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2lgjddtjg.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2stvrmyaf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2oorzrbcs.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2xkkeupgb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2mklgakjc.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ikptgpdu.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2iphthapf.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2ojfvnuqx.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2edhpstdi.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2zkujhlrm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wcesklyg.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2bncbiqvm.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2olfzsvgg.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2arpvjome.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2qeqyhtgs.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2nwcvwfhh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2msrmieej.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2lqtrldbl.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2mxgjammk.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2syvrigev.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pzejjxee.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2obkzdchr.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2cjmqywow.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2bwbfiert.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2gkegfdqg.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2ujstgyvs.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2oetberst.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2akvxgjpd.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2lccvksej.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2yogehsse.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2oewvdxga.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2nlrbhkkf.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wrptjdef.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ltxqrtzg.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2mxrieeer.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2clfujsiz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rjgdxzji.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2xqvifbjt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hwysvgua.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2nhwetfok.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2yugtdtru.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2fisjjqup.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tppyvijf.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2oqkardli.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2lyctvoea.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2bhqmaajd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2hgjyodqc.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2klzvtmap.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2udmofrwk.html


<!-- 参考信息 -->