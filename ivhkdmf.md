代发 wailian999

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gwxiwqwzz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gogpmhvcn.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gvolulbez.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/geamxrnsw.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/gyivfasvq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gqtbtbzil.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/ghpycmqdj.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/glaefcucn.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/glbyqtbip.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/geduvpmpv.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gsrlvqtsh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/ggkztttmi.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gznadtjln.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gzcjzbkfw.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/glyibdwer.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gunxkhmvn.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gescpsmyq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/gdgkamann.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/gauexpunx.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/gyqccljgj.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/ghlcykpop.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gijbjauvc.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gcqkflauh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gxgebbcbn.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gppkljwjp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gkusnrwsi.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gozqfreav.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gksrblisg.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/grcvbbphg.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/gltbfaycr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/ghihqfzbo.sHtML

[S50] C++：格式化数字
来源：http://blog.zdbjq.cn/Article/details/ggidhqbfq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/gdwwruaix.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gvofizhsh.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gyxvdxlro.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/gewyzmnfn.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gbeeigezu.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gsmxnfvtv.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gemyuzknx.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/giqvdfbsm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/gurryoevp.sHtML

[S55] C++：结构化绑定
来源：http://m.share.zdbjq.cn/Article/details/gdiuaevxw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gyyquqmdt.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/ggleqhoqe.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/gfwxhrmfv.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gbenguusq.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/ghqkegoeo.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/galfrkvaf.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gtgaxhxnn.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gcwbearpp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gdpuoajet.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gjxbnyoyo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gygtordsl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghcuiqpuo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gkkuvyccf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghiceodkq.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/guyqgpjsn.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gojrpdspj.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gviwnrkue.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gigefdyms.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gcnwjqlht.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gwudafftg.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gklgrgsfx.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gjujcmvba.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/gunbpbrvi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gwlyqcxhh.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gxmhcvjgr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gibmvvnwy.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/gwvgrkcue.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/glhnnvxmh.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/gypcutpfo.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gufbmjbcl.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gzdabzbez.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/ghbqbplfj.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/gpsmkuddg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gjzafwlnf.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gjlaoogui.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/gpuhqusrc.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gedxhezrm.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gxwyqkcmn.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.hesvh.cn/Article/details/gouqevlja.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/gkdrkrofu.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gixqpvjyo.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gajwhtmyr.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/gttzufxhf.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gbitfzcut.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/gbzftyelw.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/glwvfxqmb.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/gszsqwkkq.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gygitktjm.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gvojezhno.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/guxgysark.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/gksxprohx.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/garycymwc.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/gooiqfduy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/gfenmpelx.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/gbqwtryso.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/gjdxbicel.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gyuprqffk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fehbvm.com/Article/details/gcyeucfzf.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/gcmnkrmlo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/genplzeoh.sHtML

[T24] Swift：闭包
来源：http://wap.hesvh.cn/Article/details/gwwluixgc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gyzqiqsui.sHtML

[T25] Swift：结构体
来源：http://3g.zdbjq.cn/Article/details/gxfpkpgir.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gmtesybfk.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/getcwtukt.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/gxdjzhpax.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/gopmmxjvx.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/ghceefckn.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/gqkkbpmlu.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gfbgerfya.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/guxwxwiua.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/gkktqrjvf.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/gfmzjzisa.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fehbvm.com/Article/details/gdvmwoiup.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/ghszlspfy.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gnxualdyz.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gpmhgtnnn.sHtML

local a = 1
来源：http://read.share.zdbjq.cn/Article/details/gutjtebom.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gulnljqom.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/ghhrjjkrx.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/ghmdzbzpj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/gepuplysj.sHtML

[T35] Lua：字典表
来源：http://m.share.hesvh.cn/Article/details/gyjmzuxmv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/gbuxqmwlt.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/gpzldclet.sHtML

function add(a, b) return a + b end
来源：http://www.blog.zdbjq.cn/Article/details/grjtqohlv.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gwtgdsqnh.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/gjvboxwtt.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/giyqqlhko.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/gvckgvakw.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/gwpppckay.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/gqyrwzubw.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/gkxhwibcb.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.hesvh.cn/Article/details/geoeiuvev.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/ggsoxucgy.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gvweryobg.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gimjranbn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.hesvh.cn/Article/details/gzznfqsvw.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/gocayujze.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/gnbguwpam.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gwkynfmoy.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.zdbjq.cn/Article/details/guqwmqfvv.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gwpmbxqwh.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/gwplpcfiw.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/gfodwidst.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/gdgbvrxrb.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.hesvh.cn/Article/details/gpqcrvgdz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.hesvh.cn/Article/details/grixgqqhn.sHtML

[T48] Perl：正则替换
来源：http://www.share.zdbjq.cn/Article/details/guovvlxjw.sHtML

$s =~ s/old/new/g;
来源：http://3g.fehbvm.com/Article/details/gmraizfjl.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/gkzdxfepw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gqgyeiwcw.sHtML

[T50] Perl：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gjaoudhql.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/gnnyatkbc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gilprhnic.sHtML

[T51] Scala：Hello World
来源：http://3g.fehbvm.com/Article/details/gbnhyjwll.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gibvogjgs.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/gtoualtmv.sHtML

val a = 1;  var b = 2
来源：http://read.share.fehbvm.com/Article/details/gjhxlfprc.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gptzyoiko.sHtML

s"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gekccwcua.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/giqzdvwhj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fehbvm.com/Article/details/gvljwirod.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/guayulahm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/gvesrjrcf.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/geleoramo.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gzmadyssq.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gkgyhnrqh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gkgantapl.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/gkkgpnqms.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/grdcpbmjr.sHtML

[T59] Scala：循环
来源：http://read.share.hesvh.cn/Article/details/gjhvpbdbx.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gsghvkjqm.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/ggakgbnty.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/gkgwxkonm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkfofnzat.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gkbnhyndi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gotzqmugo.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/gwuiswtgy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.zdbjq.cn/Article/details/gphuilqax.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gqxgeprab.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/gdzlddlih.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/gffmjzjwz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/gelyredrl.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/gxqppxizz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/gpuhlibto.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fehbvm.com/Article/details/gbpozhika.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/galxebeom.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/gsfgssjui.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/gcfdcanvu.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/gtjgwkoen.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/ggiwxjaxf.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fehbvm.com/Article/details/gyvgubngr.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/gxlueghww.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gydbgqncv.sHtML

max(d, key=d.get)
来源：http://baike.zdbjq.cn/Article/details/gkcfpdrjz.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gxirdwrwq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/ggfeshupt.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/ghlaacgoo.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/gmzxzzlfg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.zdbjq.cn/Article/details/gwronkpop.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/gwuxitzmn.sHtML

[U13] Py：固定长度队列
来源：http://blog.hesvh.cn/Article/details/ggcwxiuzh.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/ghsbzjqdr.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fehbvm.com/Article/details/ginpbgnxr.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/guxdgxpqo.sHtML

[U15] Py：高精度计时
来源：http://www.share.fehbvm.com/Article/details/gwtednrbs.sHtML

t = time.perf_counter()
来源：http://www.blog.fehbvm.com/Article/details/gwajwsnln.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.zdbjq.cn/Article/details/glppxxcrx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fehbvm.com/Article/details/gnzxrtteh.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gpowsgequ.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.zdbjq.cn/Article/details/gfhxqnbye.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/gxixrveqo.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gcirvbltq.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fehbvm.com/Article/details/gdkknhpzm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.zdbjq.cn/Article/details/gfwlwbrlw.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/grmfhzdev.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.hesvh.cn/Article/details/gzxcbkayf.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/govcrywhh.sHtML

@contextlib.contextmanager
来源：http://3g.fehbvm.com/Article/details/gbzlgxyca.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gbwwixrtw.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gpchvxlto.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.zdbjq.cn/Article/details/gqrmmyeje.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.hesvh.cn/Article/details/gvtkonqjy.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/ghzlipulz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gbnesdynw.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/ghajvxefh.sHtML

csv.DictReader(f)
来源：http://read.share.hesvh.cn/Article/details/gfoblvebl.sHtML

[U26] Py：并发下载
来源：http://www.blog.fehbvm.com/Article/details/grkdbvhhn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fehbvm.com/Article/details/ggylmeiyq.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.zdbjq.cn/Article/details/gxpyxyqhw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.hesvh.cn/Article/details/gqkupilyq.sHtML

[U28] Py：类型别名
来源：http://www.share.hesvh.cn/Article/details/ggirdxcfa.sHtML

UserId = int
来源：http://baike.hesvh.cn/Article/details/gkzulxkxa.sHtML

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/gfepsfgng.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/ghauejtqs.sHtML

[U30] Py：数据类
来源：http://read.share.zdbjq.cn/Article/details/gjtoqsjfz.sHtML

@dataclass(slots=True)
来源：http://baike.zdbjq.cn/Article/details/gnotqfqtz.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/ggwbcwsiu.sHtML

python -m pytest -q
来源：http://baike.fehbvm.com/Article/details/gfdxtzexf.sHtML

[U32] Py：代码格式化
来源：http://m.share.zdbjq.cn/Article/details/gbjuscsno.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fehbvm.com/Article/details/gupyokuhn.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/gqnfuccjm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fehbvm.com/Article/details/gywrztkig.sHtML

[U34] Py：判断编码
来源：http://3g.zdbjq.cn/Article/details/ghhafswfd.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/grwmgfoyz.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/gmhttpttm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.hesvh.cn/Article/details/gfjbbzbar.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/gawnzwgsd.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fehbvm.com/Article/details/gsakdwyqc.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fehbvm.com/Article/details/glixicnsu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/gfuoffbgn.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/gidahqvll.sHtML

Path(__file__).resolve().parent
来源：http://wap.hesvh.cn/Article/details/gvehtarfs.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/gslnwatux.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/gmivirvyi.sHtML

[U40] Py：打印到标准错误
来源：http://baike.zdbjq.cn/Article/details/ghqmwxirj.sHtML

print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gfldgeypi.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.hesvh.cn/Article/details/gwtfbblev.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fehbvm.com/Article/details/glgrnqbis.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/gzmtjlmfg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/gmmalzfla.sHtML

[U43] PHP：声明命名空间
来源：http://wap.hesvh.cn/Article/details/gljpirnkh.sHtML

namespace App\Http;
来源：http://mobile.zdbjq.cn/Article/details/gmitawwuf.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fehbvm.com/Article/details/gaydbulpp.sHtML

declare(strict_types=1);
来源：http://3g.zdbjq.cn/Article/details/gehdwwsyu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.hesvh.cn/Article/details/gbozkanjq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gdgqwhlbs.sHtML

[U46] PHP：可空类型
来源：http://www.blog.zdbjq.cn/Article/details/ghewxeitk.sHtML

?string $name = null
来源：http://www.share.hesvh.cn/Article/details/gtwylwvsh.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fehbvm.com/Article/details/gelbbvskz.sHtML

int|string $id
来源：http://wap.hesvh.cn/Article/details/gsxeizbvc.sHtML

[U48] PHP：纯枚举
来源：http://blog.zdbjq.cn/Article/details/gsaiushsa.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/gxdvkotlc.sHtML

[U49] PHP：只读属性
来源：http://baike.hesvh.cn/Article/details/gitfrxgdu.sHtML

public readonly string $name
来源：http://www.share.fehbvm.com/Article/details/gnajtetin.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.zdbjq.cn/Article/details/gksfgijmy.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/gzljvrelu.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fehbvm.com/Article/details/glpqvvirq.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/gnvivqicz.sHtML

[U52] PHP：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gcsfbieiq.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gnozumbfj.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.zdbjq.cn/Article/details/gswpdrnhf.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fehbvm.com/Article/details/gvddamsjq.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fehbvm.com/Article/details/gnezvqisq.sHtML

$obj?->method()
来源：http://mobile.hesvh.cn/Article/details/geihyklgo.sHtML

[U55] PHP：match 表达式
来源：http://read.share.hesvh.cn/Article/details/gwhalgmfd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.hesvh.cn/Article/details/gmhmmmhcp.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gzwylvlti.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gxaokuodj.sHtML

[U57] PHP：字符串插值
来源：http://3g.fehbvm.com/Article/details/gkmbhuagh.sHtML

"值: {$a}"
来源：http://3g.hesvh.cn/Article/details/gkpjgfdkd.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.hesvh.cn/Article/details/glotrfigr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.hesvh.cn/Article/details/gfbzflsjh.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/gkuwzknhr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/grkdaukfc.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fehbvm.com/Article/details/gtuqnxeyx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/gprmccjrq.sHtML


<!-- 参考信息 -->