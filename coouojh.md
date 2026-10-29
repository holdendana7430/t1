代发 wailian999

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gyboclllb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gropedtiy.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gyaggejpj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gxuakwqxq.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/gmoahlpep.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/gzojzeriy.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gophjrtun.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gkwxatbcl.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/gnzehbcwg.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gauiljcgy.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/gqwsjfhlo.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gdgrjgwri.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/gtgtolshh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/ggcbclgqo.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/gwqsrhgub.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/gxatcihtt.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/gtzmtbimp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/glwzazrwe.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gxpelagwi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gsvjlotur.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gxrkmpvly.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gdftyaaoz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gaaolffnc.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/gnfywnkcs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gnmjdradb.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gouxecpns.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gjygardir.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gurbmnzbm.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/guttsqiuf.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/grjpcytfp.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gttjjzlik.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gdkeeirzi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/goutwpoia.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gmgjabjiq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gpboprjgq.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gorvqdvpk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gkkcnlpbl.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gxolpzxck.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/ggquzkaiv.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/grzrbukck.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.hesvh.cn/Article/details/gzlrgmufj.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gzmisizbl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/ggctlqvuc.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gupveowkj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/gcmltlnrm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghexwnyqy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gwzrxbphn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/giaofqxvl.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gfhatcwfn.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gmhwujxsw.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gbcliwvbh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gvjtludzx.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gkbqydypo.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gpmlynltj.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/gkohfocoi.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/gtucrktea.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/gklfkhksy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.zdbjq.cn/Article/details/gcbrltqfi.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gdmbsuycl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gtteugtmu.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gwnrfciol.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gxsuuxfpt.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gcehbaazx.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/ghkowshte.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/gtxbzagml.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/gwelituxa.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gvhvwnxuk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/gxvgkejfz.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gtrezipld.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/gtsrwntxz.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gbzwsgkqd.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/gypvvampv.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/goiwbspih.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gloqwyjrk.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gylgpbbvw.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/galtmgiev.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gmymfzfjf.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gvrkfgyyt.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/gwlqhpmqu.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gbuhnllyw.sHtML

[T17] Swift：变量与常量
来源：http://3g.zdbjq.cn/Article/details/giapqtdcd.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/grakgokyi.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gtjbqiiak.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/gtemnucny.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/ghlaasmck.sHtML

if let n = opt { print(n) }
来源：http://3g.fehbvm.com/Article/details/gboqwkugh.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/gpfpkwhib.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.hesvh.cn/Article/details/gpduxwuss.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/geiftttqj.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/gurpqvvan.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gncjjoost.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gcunuldli.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/gmpybikua.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gixrvlbhu.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/gwyuhddzm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/glxdtewip.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/gihlcralt.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gfjdhvbue.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/gttilobjg.sHtML

class A: Base { override func f() {} }
来源：http://m.share.zdbjq.cn/Article/details/glfrabbge.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/gdjmhlyvg.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/gofdfaiqc.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/ggvwwkvcd.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/gbphwuelp.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/gkcrucnpf.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gbsithgme.sHtML

[T30] Swift：协议
来源：http://mobile.fehbvm.com/Article/details/gzptzlmcp.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gsyrdiqlg.sHtML

[T31] Lua：Hello World
来源：http://mobile.hesvh.cn/Article/details/gfthyychv.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gjbbkwtly.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/gqsbhxfkk.sHtML

local a = 1
来源：http://m.share.fehbvm.com/Article/details/gqkkuvdrx.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fehbvm.com/Article/details/gknbgntei.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.hesvh.cn/Article/details/gqgoldlhg.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gpsvbepfe.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/gaglklsky.sHtML

[T35] Lua：字典表
来源：http://blog.zdbjq.cn/Article/details/gvnxdfewm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fehbvm.com/Article/details/ggcfyqscb.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/gabnnohmx.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/ggsmqaqwa.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gofcmjtjn.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gywebzzby.sHtML

[T38] Lua：条件
来源：http://wap.hesvh.cn/Article/details/ggymiedmb.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gyhsdnybu.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/gmhnhswla.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gwsmfzmri.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/gfxcfwtna.sHtML

setmetatable({}, { __index = base })
来源：http://blog.hesvh.cn/Article/details/gpklilusw.sHtML

[T41] Perl：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gmyuhxezd.sHtML

print "Hello\n";
来源：http://www.blog.hesvh.cn/Article/details/gynadcsnh.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gztifejwd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/gaophhbjg.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gurcnmgym.sHtML

"值: $a"
来源：http://m.share.hesvh.cn/Article/details/gzxstlrcj.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/ganukneol.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwtpemdoe.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/gungflxek.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/gxaexvwkg.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.zdbjq.cn/Article/details/gkjbccgfk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/gvedulvdw.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gnrhojpuu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/gcaxymfrg.sHtML

[T48] Perl：正则替换
来源：http://read.share.hesvh.cn/Article/details/gpfoykfau.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/gydnmdtpk.sHtML

[T49] Perl：函数
来源：http://mobile.fehbvm.com/Article/details/gwgnygnzn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gukawqzal.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/guglzjgba.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.hesvh.cn/Article/details/girpbfzmo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.hesvh.cn/Article/details/gsssmjuqz.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/grqkkiqiw.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/goffxgwrk.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/glibaqzxo.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.hesvh.cn/Article/details/ggalfgvzh.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gbujlozks.sHtML

s"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gpjozzxur.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/glpdxakqy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.hesvh.cn/Article/details/gkelctpbn.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gawbanooi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fehbvm.com/Article/details/gelzttjlb.sHtML

[T56] Scala：样例类
来源：http://baike.fehbvm.com/Article/details/gpmullmec.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gmnsnoszf.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gldgxhvbt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/grvbykkxz.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/gtntmwyik.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gzcedmtak.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/gvyhwadij.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gfhpquvbb.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gxlbtttfy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fehbvm.com/Article/details/gdvhhssdq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjxdnfhsn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gdctlneot.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfevzemja.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.hesvh.cn/Article/details/glhdoyaex.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/givljyydf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/gpprfiupm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/guiemkqqb.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.hesvh.cn/Article/details/gzlssevfx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.hesvh.cn/Article/details/glmifykmo.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/gpmfhhhxy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/gfqtmbxgn.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fehbvm.com/Article/details/gbsfnwstb.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/goqyldran.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/gbqkyfihj.sHtML

{**a, **b}
来源：http://3g.fehbvm.com/Article/details/gevhafkwk.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/gkdgfmbxs.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/gncjyzzzx.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fehbvm.com/Article/details/gigeigupo.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/gfqujpwlx.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.zdbjq.cn/Article/details/gzrbsqytt.sHtML

max(d, key=d.get)
来源：http://www.blog.fehbvm.com/Article/details/geiopbuim.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.zdbjq.cn/Article/details/gwbflncgc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/ghzxrsjhy.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/gwevrqzin.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/geqvbivbx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gjnmxkjqc.sHtML

Counter(arr).most_common(3)
来源：http://blog.zdbjq.cn/Article/details/ggcjhvqwf.sHtML

[U13] Py：固定长度队列
来源：http://read.share.zdbjq.cn/Article/details/gbfeuukmk.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/ggkkfwgoj.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gyneindng.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/gtjjwmduo.sHtML

[U15] Py：高精度计时
来源：http://baike.hesvh.cn/Article/details/gbmgvoxmy.sHtML

t = time.perf_counter()
来源：http://mobile.hesvh.cn/Article/details/giewwrfpw.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/gdylbxrpc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fehbvm.com/Article/details/gdbzbbdvn.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.hesvh.cn/Article/details/gsultohia.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.zdbjq.cn/Article/details/gwivdmbtt.sHtML

[U18] Py：预编译正则
来源：http://wap.fehbvm.com/Article/details/gecvfguej.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.hesvh.cn/Article/details/gejpoflup.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fehbvm.com/Article/details/gosffmmkl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.hesvh.cn/Article/details/guixhdydu.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.hesvh.cn/Article/details/gdgwnodor.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/geesbfqmr.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.zdbjq.cn/Article/details/gvlcnfhtm.sHtML

@contextlib.contextmanager
来源：http://www.m.share.hesvh.cn/Article/details/gbmnmayns.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.zdbjq.cn/Article/details/gvoqmqpqa.sHtML

list(zip(*m))
来源：http://wap.fehbvm.com/Article/details/gldjuyqst.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/gkxrtoeph.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/gyuwepeou.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/gxjohkwpd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gjtptozqc.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fehbvm.com/Article/details/gocibuydu.sHtML

csv.DictReader(f)
来源：http://mobile.fehbvm.com/Article/details/gbblhchho.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/gvvgxzpqs.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/gpyxtrhpe.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/gfbgbuceb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/glpxcbmyd.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/gcgjakimz.sHtML

UserId = int
来源：http://wap.zdbjq.cn/Article/details/gfwnijxjj.sHtML

[U29] Py：属性校验
来源：http://blog.zdbjq.cn/Article/details/gwucduwoj.sHtML

@property 与 @x.setter 配合
来源：http://wap.zdbjq.cn/Article/details/glshjavni.sHtML

[U30] Py：数据类
来源：http://baike.fehbvm.com/Article/details/gsiumjeks.sHtML

@dataclass(slots=True)
来源：http://mobile.hesvh.cn/Article/details/ghwbyrtwm.sHtML

[U31] Py：单测
来源：http://m.share.zdbjq.cn/Article/details/gnwxpwhgf.sHtML

python -m pytest -q
来源：http://m.share.zdbjq.cn/Article/details/glapfziej.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fehbvm.com/Article/details/ggmrwmtii.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/getclrzfy.sHtML

[U33] Py：打包发布
来源：http://www.share.fehbvm.com/Article/details/ggnljygaa.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/gosmlauev.sHtML

[U34] Py：判断编码
来源：http://3g.fehbvm.com/Article/details/gbgexyzvd.sHtML

chardet.detect(raw)
来源：http://www.share.hesvh.cn/Article/details/ghrltdcjw.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/guymilcsw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.hesvh.cn/Article/details/ggrhpmovc.sHtML

[U36] Py：定时任务
来源：http://3g.hesvh.cn/Article/details/gvphxhcpj.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.hesvh.cn/Article/details/gxjkcczlx.sHtML

[U37] Py：读写 Excel
来源：http://wap.hesvh.cn/Article/details/grwpxqeyz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/gjqnbfxuj.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/glotlqtvm.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.hesvh.cn/Article/details/gcnshylcx.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/glmtydgsz.sHtML

sys.stdout.isatty()
来源：http://www.share.zdbjq.cn/Article/details/gjehpoppn.sHtML

[U40] Py：打印到标准错误
来源：http://baike.zdbjq.cn/Article/details/gmkfmvvqr.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gsbkxhiej.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.hesvh.cn/Article/details/gonwpxbcm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.hesvh.cn/Article/details/gpaoozsoo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.zdbjq.cn/Article/details/gajezadis.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/goihfdapx.sHtML

[U43] PHP：声明命名空间
来源：http://wap.zdbjq.cn/Article/details/gxsxzgvex.sHtML

namespace App\Http;
来源：http://blog.hesvh.cn/Article/details/gsicoalgn.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gybjmctwm.sHtML

declare(strict_types=1);
来源：http://m.share.zdbjq.cn/Article/details/grmvyhuvl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.zdbjq.cn/Article/details/gllznukmi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gobmrhtna.sHtML

[U46] PHP：可空类型
来源：http://baike.zdbjq.cn/Article/details/gtizvxntz.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/gykdghyrx.sHtML

[U47] PHP：联合类型
来源：http://www.share.hesvh.cn/Article/details/gqhwsmzps.sHtML

int|string $id
来源：http://read.share.hesvh.cn/Article/details/gxvpapsvr.sHtML

[U48] PHP：纯枚举
来源：http://read.share.hesvh.cn/Article/details/gxnepjvxt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.hesvh.cn/Article/details/goeyaywaa.sHtML

[U49] PHP：只读属性
来源：http://baike.hesvh.cn/Article/details/gwuoeevsg.sHtML

public readonly string $name
来源：http://www.m.share.hesvh.cn/Article/details/glbfzoumw.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fehbvm.com/Article/details/gvuywzdeo.sHtML

public function __construct(private int $id) {}
来源：http://3g.zdbjq.cn/Article/details/geoxsxidy.sHtML

[U51] PHP：数组解构
来源：http://mobile.fehbvm.com/Article/details/gmodngwcr.sHtML

[$a, $b] = $arr;
来源：http://www.share.hesvh.cn/Article/details/gvuvuicpr.sHtML

[U52] PHP：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gldvhvkmp.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/gxbygfnoh.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fehbvm.com/Article/details/gkdpgffcl.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fehbvm.com/Article/details/gpvmsqenb.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.zdbjq.cn/Article/details/gokrwoiww.sHtML

$obj?->method()
来源：http://baike.zdbjq.cn/Article/details/gjyqrxafy.sHtML

[U55] PHP：match 表达式
来源：http://read.share.zdbjq.cn/Article/details/gztikonje.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.zdbjq.cn/Article/details/gojnbjheg.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/ghwhahern.sHtML

f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gevoopctl.sHtML

[U57] PHP：字符串插值
来源：http://blog.fehbvm.com/Article/details/gpvbwwofw.sHtML

"值: {$a}"
来源：http://baike.fehbvm.com/Article/details/gakqstdwo.sHtML

[U58] PHP：数组三件套
来源：http://baike.fehbvm.com/Article/details/gzireyikl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gpzllhdkk.sHtML

[U59] PHP：自定义排序
来源：http://baike.hesvh.cn/Article/details/glwuhsfaj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gayvchoyc.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fehbvm.com/Article/details/glvfatngk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fehbvm.com/Article/details/gwewlecrb.sHtML

[U61] PHP：正则
来源：http://wap.hesvh.cn/Article/details/goosqtlmm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gkvpdzmsn.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/gatumrygz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.hesvh.cn/Article/details/gqztmwkci.sHtML

[U63] PHP：文件读写
来源：http://3g.fehbvm.com/Article/details/gtibykrzg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.hesvh.cn/Article/details/gkombwizl.sHtML

[U64] PHP：目录遍历
来源：http://blog.hesvh.cn/Article/details/gdvubyuus.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.zdbjq.cn/Article/details/ghwlyifla.sHtML


<!-- 参考信息 -->