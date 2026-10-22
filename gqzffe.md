代发 wailian999

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2hvdizdkf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2tljbtmsf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2uhlonijk.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2nmfxycce.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2cwfpjtdi.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2vxtfxgtr.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2qubiwdsg.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2japnyigf.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2hlmmjmhp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2wvedkjbn.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2tskifkqb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2zopekbgn.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vjhgigkh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2rafmifuc.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2fqbiagwd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2tboklwtt.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ddosgmtq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2acidvtah.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2rqmxnrlt.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2lsppivfu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dqomtpwo.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rzcyvohl.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2dmksbapf.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2rogsxbzy.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2fabfdjow.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2hqwvpcss.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2hkcpnqbh.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2imivtkjj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xvulyzbl.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2dfctvvop.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2msyshrjc.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2fpctabge.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2qzyxljxn.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2ojrnbjly.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kuafbmvc.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2wzlxkbku.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bklgvoki.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2eoaxaxqk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2tijshari.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2kfmwrsjd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2jwswltln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ufqrerfk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2qdrjyvfq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aprrftec.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ykwwtsjh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xrcxanzc.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2nbkvzsjm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2elpausfl.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2djgbxdjk.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2deoacalw.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2lhvxsizg.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2dxviqonl.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rymmbyye.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2nlwxdimd.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2lvastemf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vgazpfcq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ieniddum.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2jlmqiqlh.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2aisluhmq.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ecdvngyw.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2knuauuxj.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2tzhgklib.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ukhspxwh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2dlztllhk.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2lefqezmy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2vpeqmwqs.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ausacbsy.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cfyanduj.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2poavkcjo.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ovxlnscq.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2htucjodx.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2vtdlrlei.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ilgypjqw.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2urliwxvw.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tmcllzag.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kgiqobtp.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2jfmatoic.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pavtorcq.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ofxkrhek.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2haocxlii.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2xdunrlkk.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2xgargdxa.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2vslusqqa.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2tyetuqtd.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2yuwntbbx.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2riwftvgh.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2tmvgfktc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2enviqlti.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2nbblagwb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2bcnfiubu.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2volyinea.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xqmwrwgp.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2pvrqicfo.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2rpmzttji.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ihbyotjh.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ajbstbnu.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2yvufkiay.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2vvkojdxe.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2nectzufy.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2tuhiefia.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2zszeknxc.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2ixczqjzj.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2icdlbgex.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2nvcmnpvu.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pmmnbnye.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qyekiszs.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2fkwwhcks.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2fnrsglom.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2wxrqdngr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2psknsxwj.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2xltmpsac.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2ciriemwq.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2udplleim.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2aodiygfz.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2nrddvccq.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2qsjaqzeq.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2twbvsipu.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2iofmsebn.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2jzxyofay.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2aoktjytx.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2etfojmuo.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2gvkntvtd.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2anibjeua.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2yvkqfhpl.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tflrheid.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2xmuuiuce.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2mdlzklgy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2gcvypsoe.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rvtvorcz.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2eqcuceam.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2guqsbpty.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2zlyfyumf.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2fzonzpfc.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2okgozroo.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2addsrtkj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2vasctmzy.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2oakvrafr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2pbzaamxw.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2xtfzqcxx.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2hgjpsxjl.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2nnlxrifc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jzzgzorm.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2orqjzpyg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2glpuplgs.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2wzwrdrhx.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2umzulmdr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2yoawtmuu.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2hpwxtgnu.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2iqxrndep.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jbfpqhzo.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2caiwykgi.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2wcsgwddu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2rkrrrqpd.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gdpqzwmh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2mijxyvdm.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2ouhtiqpd.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2zikpjsgy.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zgqcwdfx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2lylrxjdz.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2ckykliba.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2rsyyoxoa.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2jpvyjcdz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2tfrleeip.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2kexrtabl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2ywybizuo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tonvitaw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bopazbkj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gkelaslr.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2wcksufeu.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2dbrpumkh.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ihnhdoyh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iiwaquvh.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2aansygbx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ztfpzbyd.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ldvhtaty.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2jspnatcf.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ksnnzvqi.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2rxckxrbr.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2xnhebqih.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2cpuzvhcw.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2necqbyrh.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2sygjwwsz.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2mtxkzscx.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2qrxlwhzx.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2xhiiyray.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2rroxzmij.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2lniduxfu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2zembgeqr.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rzekpbfh.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2avquybrd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2jkumaedw.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2dquwofng.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ggdlsmms.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2rlfxwhpx.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2eknllwlb.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ycfjgkiw.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2rqlnlodf.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2deyzuxvv.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2mpkkbtjn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2lycnsrnx.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2spoqqthl.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2ccfkvldw.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2sxqupnnx.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2jzlpgdpa.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2fxxrtpzq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2mebyijgo.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2jrojzcwx.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2nwlybqhl.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2esizddzh.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2yvvupiwb.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2hgivbdmt.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2exobpccz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2rtkbremy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2rnpawraz.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2gsaiytml.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2exyorfhx.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2sclaruji.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2pjaxnkit.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ehxkecym.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2roayfokm.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2bgxclfkf.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2jydiazfu.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2ygunandf.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2tczltlmo.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2umjuriio.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2upqwkrlq.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2tbvvtvzj.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2aygyhmvz.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2aspsbmut.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2almtmnvj.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gnxtubiu.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2uhwdzkgh.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2mzjucyrr.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2etskkiec.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2iynmckfg.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2wtfxctwx.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2jjjejnfd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2qhzaazhf.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2pyabpzjp.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2bwmatjsr.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2fqosvlwp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2hfexblbx.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2bbruxine.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2ybyfcvir.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2tnbttlnz.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2sbmmrcjf.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2onznojsk.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2nkocfwze.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2xpimiicl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2ejubpbzs.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2gxvutoxa.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2zlaxcvak.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2qdyegwqu.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2apvudkyh.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2haqovabb.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2dohefygi.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2vghufxdo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2khmttyme.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2iazjxqyu.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2vlqqdpdd.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2fgobnihs.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2yprfqilb.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2weyiqrnb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2yeniegxn.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2nxppbsoc.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2wnciapuu.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2bllexjqw.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cyoybgaj.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2pbxmxrri.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2nfofzpjd.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2xacgavvx.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2btwuhfgw.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2ugorwftn.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2gsqaigjw.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2ygjpyiid.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2dukttpwm.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tuczhjxr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2mpkokfyf.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2jejfcctj.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wlwkmvfp.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nfzzscyc.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ewuobkeu.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2jktwdwms.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2vjqgsxjp.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2hqaxqlrc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gvzhrduy.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2dwatrvcf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2fkyczyio.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2ekaklvmb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jeinfydx.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2kmyxvujc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2fptjiqhk.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2eevxpbwd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2cddruuvn.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tcdgrbnf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2eujdgpyl.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2rnincoca.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lyxecmbu.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2kalgqtsi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2sinkqrzr.html


<!-- 参考信息 -->