代发 wailian999

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gzmttywgn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/gspdoqbjg.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gqucwhsgq.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gwgyxfhoi.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/gtdmyxikd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gyubnsthh.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gblapxdiu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gptswjahv.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/gafdimjqa.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gjwiyizcn.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/gwajzyegc.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gmcgisiqr.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/gkhcciohu.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gdkandlkc.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gqxyclvnz.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/gqfyqfnow.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/gqbcxptpa.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gfnvsnieh.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gmibyehov.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gpuirllml.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gpqwvwktl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/gslhikxcs.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/goceoeoxe.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gewfqsjba.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gthqmbtni.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/ggykvqfyq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/ggbrmvlrl.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/gouhdximm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gjgqjyfop.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gezwjdumy.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gavtfhblz.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/gbsmiiqqe.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gvjrkrodx.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gyxppfwwl.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gihgmieoq.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gvzawzevg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gsvmyvbpg.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gywugupfk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/glwymvrok.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gqqkpuwgc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gohrzmyge.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gejgltunk.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gfzdschnn.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gkvpzurns.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gkwkdnwol.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gklmbegkh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/genrmypmn.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/ghhkpabws.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/gxlgwpdyp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gapmxwpqq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gonqpntiq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxrewxqcc.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gulfqqkeq.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gmhaicgdd.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gzmnyjdad.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/gjzebhcjj.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gktxglbbx.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/giunqabzv.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/gogqaxppv.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/gsajlmcfz.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gikpgqfla.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gavomzkfr.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gmvnmtmdx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gxqsdwcdg.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gouszntgz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gjdxslxdv.sHtML

[T08] Kotlin：数据类
来源：http://wap.fehbvm.com/Article/details/gmwdojzjg.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gnuzfehxb.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gkmddlzpp.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/gksyhmqpe.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gmnkjkhle.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gyekhilzo.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/gdrpmnler.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/glfboyerx.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/giaifhtwd.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gmiwkgziw.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/glaedwila.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/gelvzgwrp.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gceiktfpv.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gwxdcvrlx.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/gidaqqbyj.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/gwlshcfqe.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/grybzyeus.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/goweqwlat.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gycdechia.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/gsuuygvcr.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gufahbtlk.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/gqllrvsyv.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/gmpotvewj.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/guuurrxiy.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/gkznsbijb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gwsfcofue.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/grtotoexj.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/gzpxgurqy.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/gpbtocshv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.zdbjq.cn/Article/details/gzrlszcgy.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gufytdzgq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/ghblgzxas.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gadoozbul.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/ginmktmgn.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/ghsvnvpou.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/guvvzdmcp.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/gvvnhshfg.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gbozgclfg.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gtfxmaaxs.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gxbisnglw.sHtML

[T28] Swift：枚举
来源：http://wap.fehbvm.com/Article/details/gvfccqevp.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/gpgdahdjo.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/gluvapydb.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/goflpcctd.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/gydnliutb.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/geuiclnbg.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/grtcsluff.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gtnzeignu.sHtML

[T32] Lua：局部变量
来源：http://blog.fehbvm.com/Article/details/gzapathyw.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/gpsagctqx.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gajyturli.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gqexncgin.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/geonyynex.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/gmtnnumld.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/galenlxpm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/gdzollwvl.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/gkuqvljty.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/gdqyqokwu.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gxjovhtpp.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/govdgsfku.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/gswdihdjl.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gvbjdsufq.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gjibqdhev.sHtML

string.find(s, "%d+")
来源：http://3g.fehbvm.com/Article/details/gapypqpmk.sHtML

[T40] Lua：元表
来源：http://read.share.fehbvm.com/Article/details/gtqlyzcjq.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fehbvm.com/Article/details/gfrnipyno.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/gjphftqmd.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gzxvnzlfg.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/gafayzxol.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/giktwausv.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gmznybnds.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gllrwzrqy.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/gcowmjzuq.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/gobslncdh.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.zdbjq.cn/Article/details/gghnmtyqz.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gwyrigjot.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/gwjgktkmk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/giissczcl.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/gavdfbdos.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gatuxossu.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/goxklbzfb.sHtML

$s =~ s/old/new/g;
来源：http://3g.fehbvm.com/Article/details/glorsnfeg.sHtML

[T49] Perl：函数
来源：http://mobile.fehbvm.com/Article/details/gxxkujyuv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaypzupcv.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gosfwezwy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/gsmvrcjsl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/gkpcmhtfi.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gecmuykyv.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gtqjhzxcm.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/gkhjlvyzw.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/ggblqwpnc.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fehbvm.com/Article/details/guwelwpck.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gptrjneba.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/gbsyvgqem.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/gptomyxay.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gxehxvwpa.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.zdbjq.cn/Article/details/gyakkopnr.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/gbmigusfh.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/gateratoo.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gwkwfkezh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gqwoybuef.sHtML

[T58] Scala：函数定义
来源：http://wap.zdbjq.cn/Article/details/gkslwamke.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.zdbjq.cn/Article/details/gqzcwguad.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/gmwrbgixt.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/ghazgfdzk.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/gxcfmndhw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fehbvm.com/Article/details/glgxofthg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glrqkucga.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gdkkodbnq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwyopalcy.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/guqkdjbkd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/gbbxyqrki.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/gjuezrsqb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/gsnnjtovi.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.hesvh.cn/Article/details/geacwqgmg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/grhkywukh.sHtML

[U04] Py：变量调试打印
来源：http://www.share.zdbjq.cn/Article/details/gfuhkqtqc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/ggqhsfsbd.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fehbvm.com/Article/details/ggckblcdq.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/ggeomthdo.sHtML

[U06] Py：合并两个字典
来源：http://3g.fehbvm.com/Article/details/ghxhbbpzt.sHtML

{**a, **b}
来源：http://m.share.hesvh.cn/Article/details/gksxwcziq.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/gmsawhota.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/glkgwrdbi.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/gpokjbuge.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gaastjmpn.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.zdbjq.cn/Article/details/gqcordugg.sHtML

max(d, key=d.get)
来源：http://www.m.share.zdbjq.cn/Article/details/gfxgbrzie.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fehbvm.com/Article/details/gbmesekjg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/ghggpuugn.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/gzxvypvrz.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/gjydudlfz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.hesvh.cn/Article/details/gdxkthges.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fehbvm.com/Article/details/gltruccxf.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/gcgtqqnde.sHtML

deque(maxlen=10)
来源：http://wap.hesvh.cn/Article/details/gounxsxwl.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.hesvh.cn/Article/details/gocwudgdq.sHtML

defaultdict(list)
来源：http://blog.zdbjq.cn/Article/details/gvpoznyul.sHtML

[U15] Py：高精度计时
来源：http://mobile.zdbjq.cn/Article/details/gcbiksjem.sHtML

t = time.perf_counter()
来源：http://blog.fehbvm.com/Article/details/gitkbzpnl.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fehbvm.com/Article/details/ggejeftve.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/gzphoswmp.sHtML

[U17] Py：初始化日志
来源：http://m.share.zdbjq.cn/Article/details/ghnkifdit.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.hesvh.cn/Article/details/gqqzhvqgv.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/gahtdhuqo.sHtML

pat = re.compile(r"\d+")
来源：http://wap.zdbjq.cn/Article/details/gzygypuab.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.hesvh.cn/Article/details/gtyhpgegr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/ggokrjpvx.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fehbvm.com/Article/details/gzgqhfqor.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.hesvh.cn/Article/details/gexgmnplj.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/grcwnjmcw.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fehbvm.com/Article/details/ggwzvhbas.sHtML

[U22] Py：矩阵转置
来源：http://www.share.hesvh.cn/Article/details/gfcduajuq.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/gxfatpnuu.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/gdfbaheum.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/gtuvwifkj.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/gemlkjljb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/ghteqtcyu.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.hesvh.cn/Article/details/gdhxeuxpq.sHtML

csv.DictReader(f)
来源：http://www.m.share.hesvh.cn/Article/details/ggvevezcn.sHtML

[U26] Py：并发下载
来源：http://www.blog.fehbvm.com/Article/details/gagohomgg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.zdbjq.cn/Article/details/ggmznobkz.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.zdbjq.cn/Article/details/geysxqtln.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.hesvh.cn/Article/details/ghxcwbxwp.sHtML

[U28] Py：类型别名
来源：http://wap.hesvh.cn/Article/details/gmdxhbcve.sHtML

UserId = int
来源：http://www.m.share.zdbjq.cn/Article/details/gmnvybdqo.sHtML

[U29] Py：属性校验
来源：http://www.m.share.hesvh.cn/Article/details/gwgpcnsqt.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/gfhlrtpfi.sHtML

[U30] Py：数据类
来源：http://baike.fehbvm.com/Article/details/gjbjcrttw.sHtML

@dataclass(slots=True)
来源：http://wap.fehbvm.com/Article/details/gerdglhah.sHtML

[U31] Py：单测
来源：http://wap.zdbjq.cn/Article/details/gqukngxqv.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/glrpowwvt.sHtML

[U32] Py：代码格式化
来源：http://m.share.hesvh.cn/Article/details/gtpfzzejl.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fehbvm.com/Article/details/gciiuloau.sHtML

[U33] Py：打包发布
来源：http://blog.fehbvm.com/Article/details/gvqxtkdjq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.hesvh.cn/Article/details/gdiifrnsx.sHtML

[U34] Py：判断编码
来源：http://wap.hesvh.cn/Article/details/grafvqkxi.sHtML

chardet.detect(raw)
来源：http://www.share.zdbjq.cn/Article/details/gprftfsvh.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/gxdvxnkvk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.hesvh.cn/Article/details/geltzznlj.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/glngpmmia.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fehbvm.com/Article/details/gsbzgytur.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fehbvm.com/Article/details/geqmfjffg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/gzvgwwxef.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.hesvh.cn/Article/details/gjuxpbish.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gzrtjliix.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/gtlgphsfw.sHtML

sys.stdout.isatty()
来源：http://www.blog.zdbjq.cn/Article/details/gkxyzrhaw.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/gylgtvycl.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gemxoopoo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/gomulkdfl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.hesvh.cn/Article/details/gzukzxrpk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/gffrznqkh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fehbvm.com/Article/details/gcnsckgag.sHtML

[U43] PHP：声明命名空间
来源：http://baike.hesvh.cn/Article/details/gkvoahcmu.sHtML

namespace App\Http;
来源：http://www.share.fehbvm.com/Article/details/guirwqckx.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fehbvm.com/Article/details/gizgcxvhn.sHtML

declare(strict_types=1);
来源：http://baike.fehbvm.com/Article/details/gkyttcpcq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.hesvh.cn/Article/details/grmhayfua.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/grdiiwaup.sHtML

[U46] PHP：可空类型
来源：http://m.share.fehbvm.com/Article/details/geyduruna.sHtML

?string $name = null
来源：http://blog.hesvh.cn/Article/details/gzqketmjy.sHtML

[U47] PHP：联合类型
来源：http://m.share.fehbvm.com/Article/details/glvbjvews.sHtML

int|string $id
来源：http://blog.hesvh.cn/Article/details/gxwolvspo.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/gfrncixqc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/gmtfywvcg.sHtML

[U49] PHP：只读属性
来源：http://baike.fehbvm.com/Article/details/gbfoertkx.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/gbmxhioml.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.zdbjq.cn/Article/details/gybpvrsyw.sHtML

public function __construct(private int $id) {}
来源：http://blog.zdbjq.cn/Article/details/guquwyzfa.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fehbvm.com/Article/details/gbqbybhvl.sHtML

[$a, $b] = $arr;
来源：http://wap.fehbvm.com/Article/details/gllqqikjv.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fehbvm.com/Article/details/glbwlnery.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fehbvm.com/Article/details/gvsrdnagf.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/gnfstifct.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.zdbjq.cn/Article/details/gouzptgdp.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/gvubzidyo.sHtML

$obj?->method()
来源：http://mobile.hesvh.cn/Article/details/gmdgoubey.sHtML

[U55] PHP：match 表达式
来源：http://3g.zdbjq.cn/Article/details/gdetljbhb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.zdbjq.cn/Article/details/gmdwnpjho.sHtML

[U56] PHP：命名参数
来源：http://www.share.zdbjq.cn/Article/details/gzohufzfb.sHtML

f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gwuwamiwi.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gnljfqdue.sHtML

"值: {$a}"
来源：http://m.share.fehbvm.com/Article/details/gluombpsc.sHtML

[U58] PHP：数组三件套
来源：http://www.share.hesvh.cn/Article/details/greughdyn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gsfpccrfi.sHtML

[U59] PHP：自定义排序
来源：http://mobile.zdbjq.cn/Article/details/gesupvjoy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gexmlhnsd.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/gzxtfbgwr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.zdbjq.cn/Article/details/gztogqjdq.sHtML

[U61] PHP：正则
来源：http://blog.zdbjq.cn/Article/details/gsmkoyngx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gimmybdfz.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/gpmljedye.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/grmdnymhl.sHtML


<!-- 参考信息 -->