代发 wailian999

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3otmdxgpw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mwilbdwp.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3rlrwoqxe.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3kipjpmgt.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3loovdnei.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3uzdzustr.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3cooctwjs.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uvapoexq.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3qvxrnwbc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uyhgxkbd.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3dqwqmnnw.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3edohjowl.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3cxdqkuys.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3tmtmunlu.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3izuszajl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3vtlohagw.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3uejlxtys.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3bgkijvbw.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3wrlznlkz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ujzalclz.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3labuwkev.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3gtxnxzgd.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3csyembjg.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ootaocml.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3lzmoycfi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3gkuxycsx.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3yfilaflk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3edqhdqwp.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3oenqgusz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3qexdotom.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3finqxmyt.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3zcafjeoe.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3injjpano.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3pytnhpax.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3zxymlqlc.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3rpfvajuw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3boiluxsu.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ugizlzaf.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ldkjnlgf.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3uygcgfdx.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmorzuts.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3wnoeojdo.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3kkbkywof.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3wxpzotoq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vffsjpmh.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3uyzvjdxw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3orjibzqs.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3uxozaxid.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3uifhosiy.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3mxkyijpc.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ntxspifv.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3hnumxgtm.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3gkzbyvfg.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3rvjkeqcg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3uiejghnm.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3awhrqblg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3wfsrylpc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3seaykpdb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3uzngxbuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yfnntydv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hkzodqmk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jfpsbrxo.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3dvdzqqzy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3nikbsmrw.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3komlgzew.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3lhwrexji.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3dfcbhyfn.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3geicvwwn.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jcscmcpn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3bmotkoqb.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3xqzoklwz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3hjykdepw.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3nrxujchu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3thqjrkyo.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3pxzylmzz.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3lilbklzd.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3azuqqkfr.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3wahrrfey.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3hntgtcmq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3znrlnfrc.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3ohqozwhx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3uoopizfb.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3yabkmqwi.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ceutwksm.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3pihkinrc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yfvcimje.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ldorukep.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xyloikpe.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3hwsugpzx.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3leipjahp.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jmfmurkk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rdrkyacr.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3bkckjbua.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3eewldlga.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3tyidfmtl.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3oqslcypq.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3klddcyby.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3pecyvcvy.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3chvvidxd.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3gvnpgmcn.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3hxlwlgvw.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3usbbokyz.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3oixgoeio.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3eutrbjpl.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3etzpjzzu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3gvrjmjbr.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3tuorviha.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lwgfcley.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3qgloqmhu.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3qlxupdzt.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3jwrognnw.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3tuaoqsme.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3tlocuxtc.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3txzfvfcd.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vxyqsmuk.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3feruqfdh.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ctyprerr.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3xkgrrpvb.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3uqdjnhio.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3xdqpqktb.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bjxrkide.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dncbcedt.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3dyynijyp.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ykwlosmg.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3oynuwylm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3rhdfgzey.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3lqbvbzuq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3bxiwqdif.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3natqhtvu.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3loiwzsje.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3snrwhsvx.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3rczuputz.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3dbycomqd.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3pnheyhlu.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3gcfihzas.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3xmchvvmj.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yihfhkau.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3jgoqbxrr.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3xnzhbgqk.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3aclvorys.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cperxhpc.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3xcxkjttl.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3rirhqsmz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3jsduehrv.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3swwmxlcv.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3vtowburo.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3dvquuhkp.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjelxvzn.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fxqogpwe.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3xcfcwmgo.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3iudopbpv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3agjnwdid.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3rxkdslib.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzvuvcxo.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3piqpnnyz.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3jeujkqmo.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3kwhggqdf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqidjvck.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mmwwxfjb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3ryrjxpzc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3crbjndch.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3znrvtauk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fhqreghz.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ekkjnhrc.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3pvwnwugi.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vgipqmwu.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3cpkfelwb.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3oubtkllh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3nqokgoau.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dwgafaul.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3ehlgehus.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3tltuxhei.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3sbiwcasz.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qjbwjmnc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3iivhddzu.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3ezrguifu.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3fnkaokmg.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3pxwaytav.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3nzmydrlj.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3axeqnxxd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3gbzursgg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dqxnkwpy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lcplmagf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lgkrdzyi.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3wzoxjsdu.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3jwvuyydw.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3tleodrua.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3edxzmlwn.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3dyubjzvh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3mcmqpszz.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3iuivsslp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3gzwavlsz.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3onsfztju.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xpuimrou.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3jvbltkgb.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3fvumbybr.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3wfdjdnsz.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3hfnyqavk.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3ectqnhhg.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3xzznstpq.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3hzowcwgy.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3bqcdycvw.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3idyqodrj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3vljrmfnb.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3lwgmddqg.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wmgjvruz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3oqnmyyxa.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3mkhnbxde.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3cshfisyh.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3tmdukawo.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3dsijyadv.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3vwyhucpz.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3pthfheic.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3wjclejfb.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3pursunnx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3thlfeztx.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3tikwwoux.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3zxctogsa.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3qkznqvqo.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3sbetustf.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3mkkojokx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3yugtlhcw.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3iffmbvrh.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3vcippvdt.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3tejdutbj.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3frobjaml.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3pizsdcko.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3opgsgxfa.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3ngunuklv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3wdkzlsal.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3yymmimip.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3mweufgib.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3nvfmsvbe.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3rwxldzot.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3svookalw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3hlfhbmgc.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3iuaetreq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3xkxbzhtm.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3fzbdernm.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3ksovmcdb.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3pqmufsod.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3shrkxheo.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3iqprdjuy.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3okxqsqiu.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3kbjxsheg.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3vkqellwq.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3jmabjpnz.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3zuyeajno.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3fmxywqkr.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3vankufoe.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3mfhjnmfv.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ftcdrfau.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3cogyibdh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3wmzysurd.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3kxgljxvg.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3jyzgzhgv.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ihwrazur.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3dgbuwujr.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3rrkwqmry.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3lkjchjzk.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3sbkjznzd.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3zukdpklp.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3iqgxnpxi.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3mqsynefy.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3zpvyntpj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3outdhryy.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3xycgqctx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3phdyooav.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3zblfqjyx.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3pkxeexib.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3xfyseclf.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3pxztpphz.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ydmjdyrc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kpnybudn.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3hvadkcnl.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3bwvbbkfu.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3nhfeioci.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3cqvyaroc.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3itqfgnbj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qcioifrl.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3iacmevyi.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3wrgzuebp.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ziocrpyw.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yffrzxyn.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3fjkqhgor.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3vpnwqdsn.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3wtwrwstv.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3fdqpdsba.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3gbpdextp.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3stdlewvv.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3ofhcquib.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3ffmafgye.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3triarjjg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3yghjmhxr.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3xjxnybnm.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tjmnphke.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ddywdhxm.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3vhgmnsfj.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3oxbxqogb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jvxomznh.html


<!-- 参考信息 -->