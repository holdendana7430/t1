代发 wailian999

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rmyqfajk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2twlaunwk.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2ianwaeto.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ockfrste.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2amdkbabm.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ecnzubdh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2bjtaybfn.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqewgsqz.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2tdlvjngx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2qalopxve.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2qblqkihj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbjshojg.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ejrvoiwi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2jhzequlj.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dbwrwuku.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2ibkewibf.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2xqfpqoai.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ltquovtn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2rgajzeve.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2zhrxecmw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rrjhczfc.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2snhlobuc.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2zfllgozd.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2dwtxnyvm.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwhaudvu.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ppyvxavx.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2vwpnkfrd.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2quusrgys.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xncfqoqh.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ikbrndbn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2skvhxivn.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2jflxqevs.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ciebdqnm.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2lnlyurxm.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ndibbpdn.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2qiwsydcj.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2qqcznidl.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2pjrwxkfx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2gqheonah.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2fblaoiun.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ixuwtomi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lkzcmgvc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2uwiuepzu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vnezxegw.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gcqhleei.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lnxyceit.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2bipwfgkk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2bspfqybh.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2falpmsex.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2gswffmxc.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2mjnwdbhg.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2rlcngofb.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2rcjgvfjf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2adspacee.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2iczvtfld.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2pvxmazcv.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lephuahp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2lmqmmfhn.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2puhldjqo.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2pbcdrszf.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2hojmtzfi.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ymlctqmp.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2kqczwssg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2tvjtpjhx.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2gjjveavt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2lbyloult.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2frlbdyrp.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2umdnjttp.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2lvzjkhpj.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iwpnzhtf.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2mznpyfmu.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qrtgllcx.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2pqoqcrie.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2vjiaajin.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zhyrpzir.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nuzhbdwg.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2dcbjabji.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2unaopisr.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2lfpkddvh.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2xqtcwhmd.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2dtziglkk.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2rmyluvhi.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2clwbzitm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2tjuccevd.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2woxebrzb.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2rytvbool.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2fziitcxv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nqonhbst.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ebolfrsv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ncuvfrzb.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2yxgnsvrg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bnszknvg.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2jgsppekw.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2cguytgzp.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2urppzepl.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2hosvhozv.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2behmmzpa.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2wssaklkq.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2voglhdts.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2mixtkfdv.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2hfpxyagk.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2shwdcqie.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2loftiewe.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2cchsogqt.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xvxolkgo.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2odpkfeut.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2izfsgjuw.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2khrluzmq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ngxeapqi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2fxkselgo.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2xjzfstco.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2ydfkiyvf.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2euwdvzko.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bpzzlunr.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ooylypzv.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2grbrrkzv.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2pywsmjva.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2rwselhxj.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2hollzfuf.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2lqxiacfx.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2rjnnucsv.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2mziylrni.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2bbaxgogh.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2exmxsxlc.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ggcburup.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2mhqnaooe.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2efkmgiwc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2fjculzul.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vhmvybgt.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2abphcdyn.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2lvhydmhp.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2teirevuo.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2dkkntstl.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2utasbxmh.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2yewypanl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2snwjjkjy.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2pihgpfts.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjnwlojt.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2mmolbock.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2drzvzsgl.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2uvefzjmc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ttgymxkz.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2epudvhaj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2adfrygvw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2tiottphs.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jqqqcdcu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2botybvol.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2jwgxrxbo.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2rjwjpxnt.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2deendcuo.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2etqcxtqp.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2wmbgkbrd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2mqlsxwfc.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2esqbnpkj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2kskmssdp.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2bkkawbtt.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2sfoyzzpd.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2mbgmhcmc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2tdwebaqf.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2zjxsiqfc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2tzoyelmw.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2djaayrzy.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zboiitmy.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2luupqwzi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2atuelucz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gwqbotmn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lnnqqvye.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xbblfolo.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2wyzzuhaq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2ogfxhlix.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2bksvixev.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2diqqfsio.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2yvznrzmm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2akqjzogi.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2fuqmcamu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2pstlrmpo.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2yvjfholx.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cmcdbmha.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2yckhmjgj.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2xbbzztnw.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2enofwucu.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ansmikzl.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2yrmhmetz.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2kjjtolub.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2exyytolm.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2ycksgmcc.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2sromnpno.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2hvubfjay.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2umjpdqtd.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rcpyjcqb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2vsofnbac.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dxfmnabd.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2yglaehig.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2vsqvzmzx.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2tfuqohfb.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2bzfinuyj.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2uxjznebk.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2ljtgyxuc.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2aqbyucwr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2qybqvtwz.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2kuqhthmj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2vsfohtjg.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2kpklgehw.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2taahhvmx.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2vegqzqur.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2kanclcue.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2ujaylekm.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2tazhmlfd.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2wqbskyli.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2hxtbsnuh.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2ymxrvgzu.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2gyclgbto.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2zelwagpp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2sdsstifs.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2vybjnmlr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ghfvfoia.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2nciwnghn.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2dlndpmeq.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2tnydjlgr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2tulzpfch.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2fljywqqy.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2tfndulgm.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2llumrykf.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2ocnjerhk.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2cajbnwva.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2mnkwfauv.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2obqfvifb.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2xfzuhkxp.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2dqqqljta.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2ypccwolf.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2hdvbuncj.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2gvjktjny.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2qmccpkth.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2kzohfgwv.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2qgojescd.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ekcgwubf.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2uckkthgb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2yejagdtt.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2akdnyihe.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2sxumuukx.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2zyivqaom.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2ogvzoysc.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2egqxeram.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2xnjxsvnp.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2qmaniqap.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2likwkjkb.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2ezyqypal.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2aiehwhqx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2agfljvql.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2uwnyejys.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2nsxjnqmh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2ulagieah.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2unzugrmy.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2snoetyax.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2tnhzztym.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2onuyxdds.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2qecjteeh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2unpmetdr.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2ojpegiho.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2xlhbcbjl.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2czpumujd.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2rgfyjrfb.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2vlovttax.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zryuffun.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2kosvchyv.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2zcyajvlg.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2fdzajxdp.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2logiycqw.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2yysooctc.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2vyhnkfcm.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2aernrknt.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2cfrcuejw.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2btrxvtyz.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2cfeldhsy.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2oqpfcsha.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2hgvwwqao.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2rvoxffle.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2gsiowotd.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2nczvbmzc.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jzityrqs.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2omksyixc.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2xjwevzpy.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2wtbwaxzm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2casdlngx.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2rnsiadrg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qrembtcz.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2xahlxvfc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jdewrqbx.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2ijnkpqzr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rmygdppe.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2rdfkcxsz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2gldnlpbp.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2fzqgyclc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2erjqwnyf.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2pscbvthg.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2zszicqzi.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2mdvjireq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qjdjjatp.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2glmijdef.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2qrqwchar.html


<!-- 参考信息 -->