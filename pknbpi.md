代发 wailian999

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2hdedzqsj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2chvcrpxr.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2hbpfjdeh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmterxni.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2iqnkbwyo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2euhzbdej.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2ykzibejw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sgfysjku.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2lnpjzwdz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hmmrxvdc.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2wyvgaksu.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2aebmjlut.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2aflgacaq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2jhfkowxg.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2soyzsgxr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2podguspf.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2nadtpmvk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2giyezfxh.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2efnafabl.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2uxayepom.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2esmyhktd.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2jehuedei.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2mpmvfidl.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vuxvnnef.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ewpbehdh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2uswmufor.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2pnlnvvsc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2umcvkdhq.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2krwcklte.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2jfamczst.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qaokscju.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2kwqsaxmb.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2wcnibaxj.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2nttifrbe.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2argkrgoj.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2elrojdwz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bvgjuojp.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2bmhcmwqg.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2qqavnwnz.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2fxgtzwnn.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2vpbhddfq.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2bkdzstrx.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2lnyitbfm.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2sareihvq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jwkwxcbi.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2gnrwiuhj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mghlvvbx.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2zctfazbm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2tkzzgvnx.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2sdbuvbkm.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2pvrgdebd.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ypgirapx.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2vlzfmsyg.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2gcgdccyv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2rluulrfy.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2swopzrrt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ujxgruzy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hmgtwyvb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2vxyadxab.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gyhudtrn.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pnbkdfhc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2tepvtunn.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2yjapwxli.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2wwjevoif.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2mwitkgrd.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2pelawbea.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2biybvhdg.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2mwewqmst.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2qtrjyjbv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2xrqkbwqz.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2aosanece.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lfqrlhre.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2nxsufgeo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2afsombjz.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ovdtyfab.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2jcpidyvm.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2boyfwyno.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2eiqbcitz.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2lsvfpafx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2pmlghnkb.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2toimqjfg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2oqgbcral.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2mftovgwp.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ifxqtyec.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2aldkkdef.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nlsebwbi.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2vtlxlgcm.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ikyqajqh.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2brdgptca.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2jqbpvidt.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wqopukwm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mtoxqnqj.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2lknuviai.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ziuwmrrt.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wsekfdpf.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2wenjnslb.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2cdpayhgk.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2vsjjtgdb.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2hztqtywc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2vujyvxbw.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ymllphxj.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2tmdljqtt.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2tsuasrko.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2usuyphls.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2abgefrur.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2pgodlmag.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2fuaxbjax.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ejmobpuh.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2mcicnuze.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ywkzgxwl.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2rhiiooos.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ccndcwac.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2wealmpwy.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2yweuxkyv.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2xvfibnfr.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2przzaprt.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2euorjtvp.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2uktmyglo.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2sfaekhgz.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2mpknledd.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tmljfixp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ugnrvbap.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2uzlhrzfc.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2bufecpzz.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2jfufukli.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2fxsnsqku.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2bgbqrflw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2qwyayixb.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2djmhnssi.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2mwewrrhi.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2jkgfemkl.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2szbwbgvi.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2fzwjcyxv.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2rxzxrdhd.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2lqmbilnb.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2xuuyqivd.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2kyenwuqu.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2xdsidefm.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2sredaszv.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2rkgzwbnp.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2eecelgoy.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2jductwgn.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2igepggsc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2qbbsxzgc.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bopfsofw.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2yfejrgiy.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ctjbfokb.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ksuwfygu.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hjdvtmwk.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2fbxaimuw.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2vapppfpa.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2izvliyrg.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2cixsgvwz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2fqgxjtar.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2fccfjvbh.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2uuftxbsz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ffadbuda.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2cpknyjoz.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2cqioaahq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2boqaxhyf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkwqayst.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ncptydcj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hedsxzvg.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qiazohch.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2rrnxxarw.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xeurvhjz.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2pgenqdxe.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2nfidozbx.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tofrlzno.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2chlggodp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2fikauubd.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2ynobuwdb.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2tesmqcug.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2baydsxvb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2rcjhkgzy.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2xlbqrqap.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2tgmzpiir.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2yixsaltb.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2mfgjrvyd.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2yvlgacwt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2xwtibtgn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wqrqtpmd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xkbrgmsm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yeonldsc.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2ikfhwhsc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2cbsfmeuy.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2smwcvwly.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2ixdeiuum.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2feqjkmqx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2efrnstqe.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2bziofyrd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2qxxspyyu.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2itojawbt.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2vqjazkul.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2asutxnjg.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2fdejgixa.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2pyvbuytt.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2lvugsjov.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2usxxrccx.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2fdrjeotg.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2cuxidmmc.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2jqjgoqee.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2cifgopgb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2jfavhjdh.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wclmqpeh.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hitjwvsq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2qvuynije.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gawpbchz.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2sczicmhj.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2egzcyjzs.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2nlmwlxcy.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2kjjpvqwq.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ijnjaiet.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2cycklbhz.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2ulvkmiox.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2flqxiqrb.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2fbcabyuu.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ligfwqqj.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2xoppdnsr.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2aluzfeek.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2ynowupou.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2fndcteej.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2bysdhqtk.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ifkvqjcs.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2hpixvsoz.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2hiooccfp.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2wcpiuscn.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2bvifnrra.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2kgahtqwb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2nswaecjk.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2xcendfkw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2pscnkzkr.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2yktyawfj.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2heiipffq.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2msqbdfxa.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2uoyaontf.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2wufmfuli.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2cenhevwg.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2jwgttyfp.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2circgkwv.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2xnkeqppc.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2prwyedbz.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2oigdawmv.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2exxoanqk.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2zpdynvkk.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2lbjbipix.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tleuicwn.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2cphezeus.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2lhesalxs.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2mbhvyedl.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2sxdbpean.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2pyvftqbi.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2lawqviiu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2tqjetshr.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2pqjhmibt.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2ngtdgtdq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2vxzbyxqy.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2iaqaoowm.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2krmeoiag.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2lzlkdseo.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2vabspemf.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2khlimzjd.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2tbljlatw.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2xmubyzws.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2awwwvfew.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2wesetfzb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2qihttkij.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2dcyaddgt.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2hamaeoea.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2gfciqhlq.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2knqbcieg.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2dpppzdfc.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ccrbvlel.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fpakyppm.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2embgvodl.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2nzfafjkm.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2pttvyzum.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2fptkjfiy.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mtedqfne.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rpnseznf.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2hogrbqjl.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2ehgokiye.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2nmnfljbg.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2irwifjxl.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2cyjqttsr.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2ipkwrnco.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2evrkxesb.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2pouesoop.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2zyzhumyw.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2mpibqmdt.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2rkngcvjj.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2xetbugew.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2ukgffogj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2tmtqkijy.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ivqcnfdx.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ffviotek.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2cazsqrwy.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2hwfbcwyw.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2afusowpy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2czhbisjw.html


<!-- 参考信息 -->