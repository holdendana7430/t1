代发 wailian999

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3lxbmtcre.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kndkajza.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3aznrodre.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ppzckqmf.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3bgtrfwbf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ahdpfssa.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3wtszfflu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rqnfckvv.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3mtzwfuxr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ppltompf.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3kxsfhldy.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3fnbdfdxu.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3wbbbxvad.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3kwzafsmd.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3sdivnijw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3drusoytg.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ergcurgf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3zjdgwruo.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3glapckxa.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3nsjiwkxp.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3omhixudn.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ozatdufe.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3qabmlexy.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3uikvaepx.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3codatnvl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3mcxnveaq.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3xrfufqbo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwfincue.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3bjilhrwt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3wsrqcsea.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hpgfnofy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3zqglyiff.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3bwgvdkxo.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3fhdeezcj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3zrtdkitd.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3pkutpjjb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wpdxjikw.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3wfqflwhk.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3klungpll.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3cibllhil.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3afqqwdrc.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3fpwtkomy.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3grdzzlvy.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3glwdrmxf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3sifavhni.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3qdoymxrz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3jzuyrvjk.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3otaviqci.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3iahcdykw.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3chohffax.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3exeufmes.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ldfzbfyg.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jonimylt.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3ugazjifu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3duaywbki.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3uyontluf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3mvhbpgnc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hzlnfvdk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3useyumnz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xhbmocvh.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gmnuvvmb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wjxbplci.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3eplnmbrc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ubdsbgxv.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3cbhipnlk.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3uqskjvnd.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3lovckgpi.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3msnaiiui.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3esdhlnba.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3unzmyyrf.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ajorvzvp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3afixhpsm.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3njctlwog.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3hrqjdwez.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3cellkxis.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rrtwkfda.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3qjohjdre.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3bexxuhpa.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3yjqxqzhn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3ybjporaz.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3mzqueitu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3xfkivzsf.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3tjyrjgdi.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ihbabuup.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3moxmrnhn.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3udjgrrxw.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3ilstsdyb.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3pzcxfbpe.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3blzrtckp.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3akkrzpym.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3miogngqx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zmvlzhcq.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3zgbyobqo.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3jqkykhwn.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3irlmvvwb.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3qrbuwggi.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3yohupyxi.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3qqquzlfs.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3rwvqqaja.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3brmrmxfc.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3xznutpyc.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3utyhucil.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3fysjgbqg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jounumsd.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3kxzazkep.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jvudyjly.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3adorhisa.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kpykuzdj.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3gmmsazmt.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3bjvutbjh.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3zbcollii.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3gozkoclr.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3jbivusam.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3gppcipnb.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fwrzwmwk.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3xhrhyand.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ekyipppp.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3siamfpli.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3mmwgjpkn.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3ggshoijo.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3diykwyhy.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rcchbibw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3kkhdwuoa.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3thtalbzk.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3qiktzucq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3dsfteqbl.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3uesyelyh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3wrnuzvhu.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ilsfrahr.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3meixvijy.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3qjgctknw.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3dxifowli.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3shkxkhir.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3xsieupzn.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3zostjimu.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3aojdladf.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ckgpglpy.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3etadeopq.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3iwidxrlf.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3smfuocpu.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ypblucmx.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3fsspmvzq.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3bevoawhw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3oxumvagq.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3sbrgcaym.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3yktbeisr.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3lcpychml.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhnolnxj.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mlklfuhr.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilkyvzbh.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3dzlrxnbo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxptnjjz.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3yeowkqaa.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujfrmhrn.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3eydcutxn.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3peikevgo.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3rqoidchw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yqorleav.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rhzpbgvc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3gdibwqqf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3efkrxfdr.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vwpdczcd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qazpfcum.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3pqlqqwih.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hqiugmlx.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pkhcbdfw.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3vhpczcys.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vlnxkzsg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3caeraabv.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3uuhtypgq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sgtoerfs.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3knbowftg.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3prpecjkz.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3whnjneoi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3tjsxtfeq.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3uqrmvwze.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3trnbkxnh.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3iykonakr.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3sissobbg.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3huchsstz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3wjhfwook.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pbsfzcyq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3xjomihpt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ftvqxvnk.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3wcwjuqlv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3pcuxksjn.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3jpdwebsl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vemshvbs.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3srcltxmp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3lrcspyro.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3jprzxuar.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3nowxbcvk.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3gukrdsft.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wimhxumg.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3dhdddgmt.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3phafozhg.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3emvpmtjx.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3cmsvtmlq.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3hvekzjwf.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3tfgfbczq.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3wgiwfsfj.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3tapycbjr.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3gbtfgben.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3rukqytas.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3afmzrpey.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pibswoes.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3kaoyfmsr.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3nlqjylvo.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3zjwecnhz.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3oyehrguc.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3dcrreqbz.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ajzqptbl.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3dyvpppto.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3bkjzghyj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3sdkqmuhj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3znujzgty.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3psakacug.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3orbzyorw.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3utwheapr.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qmwxdboz.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3akbvseuy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3neowogck.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3wbjwikvy.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3foozdqxg.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3itftoeqi.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3piwijwqg.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3wudqwggc.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3zzcfihxk.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3ihjbmafh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3otxqslod.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3jmcrkltg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mxutdgow.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3nohrgvtv.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3qsfgclhl.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3ncvytljz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3uetgoqqo.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3iakksxdk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3atflapfu.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3metqowjs.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3auwiibwu.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3cruwhgjh.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3pczqmwhd.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3dpjdhsyj.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ihxxskkl.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3zezqkqmw.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3qwifmkpz.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3zympktdl.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3dmejtbdd.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3tsldwkvx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3sosddiwv.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3hadvyviq.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3ivtbfgcc.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3lccdkvzt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3xmqnjloc.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3smgocfok.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3dqyiumir.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3gtgwkroi.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3mqbkwznm.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3cqdwjket.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3gjxxwien.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3xkaslabt.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3aquobukb.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3bkrsgsxh.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ipnqcjzi.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3hwpypdpt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3ulynjgch.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3ljftnnho.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3ookweeuc.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3oxwmzlzp.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3giodatgz.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3vlwbrxjp.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3unickues.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3jpymbbqg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3djmgfkuw.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3bggdhxqk.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3vdbrpgik.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3zioorvnp.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3rqlueatf.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3orhvpcan.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjctafzn.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3qamcplfr.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3pvhgfcyw.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ygioeaed.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fdvhrbof.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3ejzmbfch.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ragdsgbi.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3qkzjzzem.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3hxjubyvd.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3zadcehww.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3myuamyyh.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3eeinbjvt.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3agxqvvaa.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3lpmqbugf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3zooiyqvu.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3zabrcquu.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yakyzgga.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xpvdiuap.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3hmahqxoi.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3anjfloal.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3albfijeg.html


<!-- 参考信息 -->