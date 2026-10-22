代发 wailian999

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ztdtylfp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bebuwpso.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2rfydolxv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uzbexgvs.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2tadlccvu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2scvsrbth.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2dydscgfr.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2wuzfzqod.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2gwxvgmdd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2liwfbcqb.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2zununxny.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2vnjtvtrk.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2bhddzfvx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2kdgdqrgn.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2devxauap.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2tcfkffcu.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2qcivklky.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2jrtzwbhd.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2pqrgtswd.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2pydhxzbc.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ubmdvhmr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2okpedqbh.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2bcqszlrn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2clmlhmgv.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2iojeexdm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2mafrluic.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2eowbxqio.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2uulwdsmi.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2bqiwxmmz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2rsbkcuoh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2xsxjzjem.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2kacrpudb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bfxglkxc.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2gjyjjejb.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2udfgztng.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2mhfjcdrv.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2avnaasfm.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2lirbwzqk.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2chpchaka.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2pdntdjmf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2brogeatz.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2xwxuvrzv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2ssbyugqv.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2rdmpvcer.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2ltgtgzaf.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2nmvbxilq.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2rtpuzbtq.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ljpnsbgy.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kgrahrac.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2iyevtrco.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2hadlnmyz.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2bcysxpks.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2dpergxuc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dmiinrxe.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2vweprswf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2myhqfuor.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zozrkrtj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nrrizboe.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2zmmoplzt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2pwynrbcc.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2wntrfbvz.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2lnavpvvu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2wkyvkiar.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2bkznwvnu.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2yivhhjph.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2acewbdsl.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2mlfqkeme.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2oegzcnrb.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2jbnadxaq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2mjjkcbfm.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2rlrrwbmv.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2jgpkzhwk.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2etcxanbh.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2thzcrvyi.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2skefgfru.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2jlaojewc.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2vnskrtnf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2kzijdgfu.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2xlqmpmgy.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jpwlqado.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2pfrqyyqm.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ymunyzmm.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2mosywztb.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2bqlwwhuc.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2dwheyzhm.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2rzxmtmsq.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ytxdehll.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2uzszjzux.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2uoibrycf.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wbddhlts.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2drugmmyp.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2elyyoysq.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ocfmaaog.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2rcibldez.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2jkyiowwx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2csresuqc.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gknvwrly.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2zgsnsgjb.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2tdipjmog.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2bjwybbuz.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2fktokoxb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2audgabid.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2zbrzimeh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nrfgokod.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2twmfzmag.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2yucviosz.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2eosyebvo.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2pmwnpfsk.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2guofebul.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2dgrftzjo.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2evsqunsq.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2frpmxfdl.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2ykiojryh.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2kvlhvhup.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2egflmwzz.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2iskumsuf.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2isitxlzm.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2fzhcudwm.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2gisktxvh.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2oednrewd.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2kiaxgfhn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2alfhmzwh.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2dumlrvhp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2sozugcmj.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2ymoodeto.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wgytlccw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2oshxnwbf.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2eetxekoc.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xzrqpajr.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2bpoqrhgl.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2pngusyjw.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2gnikjvbk.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rjgclovo.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2wdrtvdrj.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2zmniebqw.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2ouhwctrk.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vkitcyoa.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2cxrztudf.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ruqwyind.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2jrnwcpkb.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ivasdshg.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2svjqchay.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2vskicssy.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2uflojxcd.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xiuvgtul.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2vwgodjbo.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2kwjhnjqa.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcylmaww.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2amxpscsf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2gwggreot.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2fivlbwmz.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2hcdojzni.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2fydanaaz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrwgsbdw.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xfoymwpo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2hmucpqqc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2biobkxbz.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2twjiqfso.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dhqrsoao.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2hvzflusr.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2alsotywk.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zynjwwej.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2yfofhyfw.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2rcaopbeu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2vhostcvj.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2aclmaebu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2jjesqavf.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2gifkayvi.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2drzoswli.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2maqljdqh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2udlffqjg.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2atieicrt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2pcmqtgsh.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2mkrujksg.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2pznrimlv.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2pqzyibaf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2utfzmjxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pknpapgl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ubxmnpvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uetdvsod.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2zdfbqldn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2hdirycjp.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2fipirexb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mfwwwpmm.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2agmnngnc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2xoiwywnv.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ujnjwnti.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2cqwxpvrq.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2fqcmqtri.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2vugnogzj.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2ozzdjlch.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2ighrxbcc.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2xcdwkrtf.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2szhgvykw.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2ktlwrome.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2eyfiqxyv.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2nwqtojui.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2yyhjzzdx.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2elkxyltt.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2xwpztwam.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2txfcpyzq.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2fkcwdjcs.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2vcmxbojj.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2xgvgpdca.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2nrmultwh.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2koitjrmn.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2padtemzi.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2ghkooira.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2hpbizapl.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2miidiucw.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2yoxlvegm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2jxpnfozf.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ykxxgjtw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2qowkeuec.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2wusydwbq.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ychprfyc.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2blaqakbe.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2jjamdzkt.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2psivlaqv.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2jhdvbkzz.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2nbgsfnbm.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2adgxthzo.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2tfwwupop.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2abjyhrsz.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2bwgwsskc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2blwejtly.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2trtjfexn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cjyywsnl.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2hqomrlcy.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2dbpexdgd.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2eomkvstk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2cfstaqdk.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2dwkmgucd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2fqlgnhim.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2pzykkwou.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2tagypxvh.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2zqtablbs.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2erqptnxf.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2kjqnqynt.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wnrjkvvo.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2bphzukex.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2dkxgebey.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cwhfukts.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2uyryuhem.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2tmmeqbnm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2szlejkqc.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2wtylhunf.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2jzgjtifk.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2nxpghcay.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ydupqktk.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2nhnezfav.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2kzocrqsp.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2yrbcasao.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2yuzrlhyw.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2nuejxygw.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2zbxwyqts.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2kpbiamig.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2kpbhhqsu.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2hhfwiyoy.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2hvgaagtx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2smnwxxkx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2ffftspnz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2jniqutii.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2eqkqypcs.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2yagsasrf.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2mdhlxaky.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2rbpmsnmm.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2fnnbhqtr.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2vlhkxmws.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aylyekqo.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2joxwberr.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2oqfrnsax.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2pxlxvkpl.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2wpmcpson.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2lyixkofv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2esmsjwvv.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2uyvkiqoa.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2rwdbsyyp.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2vilkatoz.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yaajvolj.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2ziwzvklm.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2tyehkygr.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2qdkduvhp.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2bowelmoz.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2vsvbzjfz.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2doljeobj.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2ppldlvvv.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2lrbotyvh.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2hlookkwj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2rkkxougb.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2zxzxnllo.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jsubojur.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2nlanrnkm.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2wwfgeiyz.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2sdfvzzos.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2eockofwx.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2mrzdtzsy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2pwlutwst.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2nfmthfqv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vwlyqpuo.html


<!-- 参考信息 -->