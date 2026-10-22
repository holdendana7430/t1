代发 wailian999

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2qtujudqc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2qjloqjix.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2csdlcvxd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2ykmkleyt.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2csywwnaa.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ckfdkjqj.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2zjazjkpf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2azwbhfwe.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2vexuvohu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wlcmhwil.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2mlsigebo.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2xrykqkqq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2kavxbgmj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2dxwdodmv.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2enjpzdzt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2dhsehpgh.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2hydnljnm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ustjzpzz.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2xdbyklyf.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2bnlscwlf.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2xtfctolr.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2ndxksnzi.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2wmhlpzvx.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcrsmcva.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2jhbhtumh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2duzxfjab.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2exglneqq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2svxzbuto.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2fxyfujix.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijihjjwp.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vnipidob.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2wykykvlk.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2kfsvqtds.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2yivnifgm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2poteovbv.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2gxnognkm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2sxikunzo.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2mtitehod.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2orblkmmp.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2qphnmzzg.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2vnbowfht.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2xxffxhom.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2voeylibx.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2qiwdpoxw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ljowybgr.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ngkjfriv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kneesfmy.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2gvxqohoq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmkjylyg.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2dvfshsvt.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ruxrxjgc.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2bmrvkwyl.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2edjoakpo.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2qtepybbh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2usgoknhw.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2buaktlym.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2emiegshw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iqzdkpvm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ztejctvl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xndwqwab.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2suxpsqoq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wkxoebpz.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2awxrrhrj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2faybjwdc.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2acrxjdzl.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2syrcsyao.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2fxkaqalm.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ccgptjiq.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wsovobha.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2eanlchyb.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2izkehbfu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pcosyxql.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vrycqhbu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2nkepweml.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2gwblpyat.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2mhurimtl.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2marjhpjv.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2aaddrmqx.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ykmmnani.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ldtdncgt.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2xgabarpz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2nucygkqc.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2vmsoasle.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wzumfgck.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2adqkucvh.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2vjolrqrf.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2qtmpouyl.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2qoqznnba.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2nymcaotq.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2rizutvbl.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cvyshoby.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2miamyjgp.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2wuijnmtn.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bruuusje.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pyzxwveb.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2fuznpcky.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2vsoezclq.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2atuviaxx.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2nljiftba.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2dabdckpi.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qhzyinjv.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2sbpddfjb.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2pmzxkjhv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2yaxlxvpv.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2hdrjifbu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2dfpwbcnb.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2pedjsvdx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2cdufbwuo.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2fzayafri.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2mdbpjqab.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2zvxaybxv.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2vvvrsvsb.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2xxaftfme.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2yofrashy.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2zquosobb.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2kcgaqmdu.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2fvilbwpt.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2kmsegqgt.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2jdggfcmi.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2lrdqrqhp.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wbogxbtb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hlpguvxi.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2cnydcxlc.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2tbloalxp.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2mgnfefmz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ikqrayrz.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2jvccokar.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2bfwkuhcq.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2btfxbmrs.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2rlnewqrh.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2bixyrawr.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2xevxfejb.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2zupakaup.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2owndgfyp.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2vszwlfbw.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2bafebbtt.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2erdcoxia.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2nirjgpry.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2nayubltr.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2cynmfgoh.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2asuxcfsu.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2wbecsyfm.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2wyouqupf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2louzeatr.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hoegzsyy.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ktdzkape.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2nrfjrxyp.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmenwgxz.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2crwebhee.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2fjuqbmwh.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2xquwbxpo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2qtwoeqhp.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2lsbapvnk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2posusndz.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2tyjomcms.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2sbeqsuhm.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2sjbpoahb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2juuvucph.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lofyqczo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2eglbnhmj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2lsjnivfb.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uftslytz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gkabgnhk.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2onvyhtkn.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ssajvjhv.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kwpinwkd.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2cotxfyjb.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2phhfkwpc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vajakpod.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2swwjmwxb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2jdivnuao.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2sjbgagie.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2bhpmojek.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2floadaob.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2juuggvmu.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2xxmaxapa.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lrsrkjhl.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2qprdziee.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2kqlcpfzo.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2xkouymza.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2zamooclw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xksqsyza.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2svxduwoe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ivmsjsoh.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2xdhmznpd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2kosstnxq.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2xibywndk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fndgzyoo.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2uhtuntay.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2mxrcmuvv.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2gclrzebd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2ltkwrkvc.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2kcedfskc.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2sluhawto.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2plvgtpjf.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2pcnumgvb.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2fxxibpwj.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2kkqrzqaf.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2trmbnmhc.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2qmvvltyy.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2qsuiiaeh.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2cdkmmmpw.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2zvxqrdgg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2npkkxxks.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2dvarlxdj.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2fwtsncjf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2vzpcjfne.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2qhnnxioj.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2zqsflkoz.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2fdgszewc.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2ignrjmsc.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2ifjptwro.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2icrkokke.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2kjwgdzoa.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2jkgubxvu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2bxqdvssg.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2hezzxtno.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2woufuhtl.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2ahvwqhmf.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2hjrfcnpa.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2ujekkeyc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2cakmqttc.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2tzuwfckj.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2axmqhbsc.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2xpfeahpa.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2jpxtdtur.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2xwmtvnsv.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2qpsrpyvr.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2pwyohqnv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2gytddnrp.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2kilyrstm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cevaxoda.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2bbkeryrm.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2dnmkpels.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2utywohui.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2shvtrazw.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2nwzpisin.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2njmhofrb.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2cbhnyhot.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2wqqoszzt.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2wheikkxt.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2utcmskul.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2ydajbhih.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jqhhsmpg.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2clhcrcso.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2nldxgwmo.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wuxvebsk.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2iwaxhnvj.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2wotvflrk.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2iezfvqdu.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2vzopxpru.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2rxcqgnfy.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2fxqmfvvg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2gzkauyxt.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2lcmwkmmi.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2lzcbodfk.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2pcklfwfx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2hdshjjaj.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2vnvsmrgs.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2vtntbugg.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2jrpeavvh.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2iueuiflj.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2ahaxjiik.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2htcrvgvp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2nkrfgwwb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2tkejwibz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2fkpaopfm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2hpefzgbh.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2iouhjnbr.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2astpslwj.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2mqprxrsr.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2yhvajpvt.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2qzokytsi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2sjkgspbg.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2tzjolivo.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2xsxpqahl.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2krxjxhay.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2khlxcigw.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2rzmextzq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpcsbspn.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2ekxyrjxu.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2rgkiqbca.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2xwvtkpjd.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nioffdhd.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2ztwgdomk.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2nuhsezrj.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2jekjrjyf.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2utyegmvc.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2yatkszfk.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2ftbnjvrm.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2onvgxxiw.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2mqaovbaz.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rmmycwvp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2huasrwvf.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2rsndxqsj.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2sjlnfyng.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vzqlpgdz.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2eddqxeqr.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2jpximzcn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hvoacccc.html


<!-- 参考信息 -->