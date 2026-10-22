代发 wailian999

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2bqlzmpfq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2heolxnra.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2fdakdawy.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2mbauumnu.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2aqxsilat.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ipbtesum.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2gypkmncw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2olxuhsmd.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rauydgho.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ucytiqlf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2dhqhpiav.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2ttfvulhq.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2hwdnfbso.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2dgkxoomr.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2cmsqrzhy.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2dcqdjlak.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2hdzyfjoi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2varauamd.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2xafongal.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2yidmazwq.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2sxuruvhw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2gqbkrgla.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ukhhrhgk.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2qcliqyra.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2vvxmrzjt.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ipiafzns.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2cnwdykeh.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2jamvyzpo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ggtmfwzn.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ljejnxhk.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2agzkghjn.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2hdjlclpz.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2klgaitwq.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2pghdvvvb.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2ibtsnexe.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2burgtgul.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2lsxsabzr.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2shphcyye.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2cumkegxm.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2qewfvlkw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2zdpyhvso.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2ernkcyso.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tasdlekg.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ftdxgxqg.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2qmkhsbxa.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2buvcxbjj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2ukupuaks.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2szbzbpbk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ormvucht.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xjqqjkyn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2fzmvjnax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zdhivbgz.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2phjaqbpj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xvbhsndw.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2afyrikvb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2pgmabipz.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2cckrzxlh.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ekaedcqq.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2xglbimos.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2jhxcgscy.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2lurepsni.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2qqkfebch.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2iewabwxu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gicqdvni.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2pzqyuwfj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2eljggzyn.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2tfdepnrg.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2fsomylwl.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2vmtfzcos.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2xxpfzkye.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2owghuabf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2tqgptpwh.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2qsailuog.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2grlwifbo.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2yqszdjao.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mbenjvsp.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2eqfsjztz.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2obtloykg.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2zlltjsae.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2tusyfmxx.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2ruvowjlm.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2wgkalovp.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sssxdgha.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vecpulbr.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2bzieanxa.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2nabvkxcg.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bpbcrwuk.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2joybqnqx.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2dozqpdii.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ucbftsuj.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2aqewfxcs.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2xnprqsud.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sqgsyxbu.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2kgredjtb.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2cjbcbgpl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2zljyhmvk.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2icslycod.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hsjflhir.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2repckqhl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vvozjmsp.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2bfwngilk.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2fqluiorj.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2iiydjzns.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2yizosfpl.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2ovuqjkkv.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2szllvqrm.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2jypdomia.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2xzpbnyyy.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2wjtzbmzh.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2pvmvavcj.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2bhvoclza.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2pjmylfnq.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mqlrbpip.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2krptwjed.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2mjbuvltw.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2xrebmmkz.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ilbwfvbg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2frfrjirn.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2bhkdsirg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2ocihxhmc.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2extntotf.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2vajpjqnj.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2gmppgouc.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2gclrbymw.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xykpndkn.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2mumrwdli.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2pphqupaz.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2dimxnepg.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2rowiouwq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2nsvrkbue.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2xnjzhzlq.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2cbawbhcc.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2eieidipj.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2shmglhdp.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2jmhtxlzc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2tiupmsoy.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2dlghwadl.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2cqbuzreg.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2sntpyjoq.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2flwtkmvb.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2srclyyzq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwbvzjhz.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2omhinuco.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjzswsdh.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2qvfbnvcy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2fnstffzg.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2itagkkvq.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2buxvtpsy.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2zxtqahqy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qvyulyuh.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2pgkxqxkh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ggklvlsz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2fujumopv.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qivavzyz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dphyvdiz.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ghdzjrur.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2yjkafmao.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2lpicgvcn.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2obvtmzne.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ayqqvkcb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2olpaauqt.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2szefhzcz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nboezbwj.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2seocgbhf.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2azklhqsz.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rcvdsjgk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2imtpsvbn.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2jhtlycvw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2nraueiup.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2bcsgqvsz.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2wqcvzmji.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2xtnckefi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ksbswhhz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gaovhxfy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2kpxkvrdz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eukcmznb.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2frjtxldi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2ndqqxink.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2lpwxcypw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2qzhjydip.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2fvoalhdo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2aflfigwr.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2fzchkkgy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2onsrlwok.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2nbnkqctr.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2nblinuqc.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2addcbdax.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2lsooagwz.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2fjydniul.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2yvqrygnx.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2pvynxvrz.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2pbukgbwh.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ilmmpbmd.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2julytoty.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2imbqirlu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2jixlquzq.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dfqzlxhv.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2xbwemzjw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2jthdvaux.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2rbghmodk.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2okmdryxg.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2ofmhjjza.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2rspanatt.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2gwhzqpmk.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2lwuebnrm.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2nvoddmcw.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2asxejhwt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2gctrwlny.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2udnevomc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2nwqkjyqz.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2nbsfdtcz.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2lakfzxoi.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2issfewrs.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2uuqpwxfy.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2vpcpmxxp.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2mluawyxz.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2ngymoaia.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2vpdfkztl.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2xfiqwxna.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2rajxdnde.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2accaiahp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2dwqoqqyb.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2gwcyjthw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2irdhhmzi.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2jieejbgd.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2qbfbckqt.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2ypfbneer.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2xkspwrid.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2lpojpgja.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2lwravluz.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2wlvidccl.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2ktixylmu.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2tcyowqdp.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2fqqynlil.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ujkxzbsx.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2svvgpjus.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2tvemflny.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2herbnlua.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2eunojlpl.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2yhgajtfn.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2rluticwf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2jycjgxgl.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2bcaygdbi.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2ubicysnc.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2kktrdemy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2mzuvhydw.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2xoeqnfzr.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2pqtsklrb.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2vgeimnsj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2vedcgdur.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2imuuvgif.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2nkguyzow.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2wrvtoytj.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2tamdbggp.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2srusooyz.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2pcoyrvlb.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2xgdeklqg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2nwthreqq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2jvivzhli.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2fuaszogk.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2tlhcnpfq.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2lqrxhpwj.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2aybesdhr.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2ahedqzmk.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ekvgwnyc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2imggfreq.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2stfwaumq.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2hgqplhje.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2zudkjjwo.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2ydcbhcbj.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2kvljnswf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2explhrvj.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2jdzswpkx.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2pniapmgq.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2uwnjvocb.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wmvvtomy.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2rhtxkjcb.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2modrqbey.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2kdgjsouh.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2kkpwmrax.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2uhmubmgn.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2momrnhbv.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2vnuazqsj.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2jgbcsyqj.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mgnjcnjp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2hlspobuk.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2djxejamc.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yxgxwlla.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2cxvpmoyv.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2xfggjtsa.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2zzgzyeha.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2uxurvhgv.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2ewiffbbn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2hjkegqpp.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2nflrubfu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2porbyvqr.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2qfnqxbmv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2rclvocee.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ifvuwykj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2gmszbvyh.html


<!-- 参考信息 -->