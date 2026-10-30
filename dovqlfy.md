代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gihnopitw.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gnzprlilb.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gegergnwm.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/grpwkkuim.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkkqahebi.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gyewrmkmd.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gpdlndwuk.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gdbnccpzu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gwelbbxol.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjorbfpo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvsmbmjz.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gwauerwyn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gveekepkv.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnzqhbbu.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpvswcgc.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gretuaita.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpvgmywh.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwkitize.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuagwdem.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnfaqgdk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gwqftlaoz.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/glhxsfaez.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gvlsbhpvs.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrxchkty.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gsyacujnq.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gstyksrmj.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gmryponsp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtddhfmfr.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/ggewiqxkq.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcuyscjy.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxprftmr.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrrcsixe.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtglrtxdz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjvugmie.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gnetkmvfl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/grbbcuhkw.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/greoblvvd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsurweeeb.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gejbtxykr.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gwknokkcm.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gcbohgujv.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/geduewbjt.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpmyolob.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/gkquuomnf.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/ghopzwrrf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkumpmxib.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfnjsotc.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfstnyrul.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gbidkjauv.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gbkwovhxu.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glheznlgh.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrwcoeuz.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gycayqtqr.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdcosjbm.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsotbfrhx.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gbpgoxnqo.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gpthgtnpq.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gshcuwdni.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gwumhsbnq.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/gbzhahavc.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnuxugyx.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwohfjje.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxnfbtfg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gnsneidlv.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/glfweflzq.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gahihhbie.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkptrvje.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgmgliiv.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gqxzaevum.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/glyioflyu.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjionmin.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gojnexvel.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/gvnipiisa.sHtML

struct P { var x: Int }
来源：http://baike.fanxiaobao.xyz/Article/details/guwadgnhj.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gtojxqkhx.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/gqhpjcuyh.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gebqtyvsf.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/ggaxmvzic.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gtuzhwggc.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gslxrjsby.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/ghskujtqw.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdamugdpe.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsysuffm.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyctuazzd.sHtML

[T31] Lua：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxibrvcr.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gtdaktqct.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gepkkvici.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gzzpnbmas.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhtplpni.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/gggcffzyy.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/goqfvgwxd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnweqjyg.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/goodikofi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gydhlacnz.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gufkvxbet.sHtML

function add(a, b) return a + b end
来源：http://baike.fanxiaobao.xyz/Article/details/gxltcoaqp.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gvgupndqm.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrgeymaf.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdngfrcut.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmrrkexc.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/ggllcevkn.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gkuhzozba.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gregohskb.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/gtijvzstn.sHtML

[T41] Perl：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gbzqvlgzb.sHtML

print "Hello\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gfdxpouoo.sHtML

[T42] Perl：变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gudjibetg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/ghpdokyni.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbnnvkqh.sHtML

"值: $a"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihoosfdg.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gmmjenvcp.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdqqzctp.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/guoiafqvb.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkoyltksc.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtdjnwat.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpovtjmmv.sHtML

[T47] Perl：正则捕获
来源：http://baike.fanxiaobao.xyz/Article/details/giitckxuh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwnnmisi.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/ggglmqfyg.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/genjnrnnk.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gepixkxdl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvcheucb.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasbkmfal.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpydsyzs.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvhcajlce.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqoimjeyg.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/goynxtzim.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gocriusdu.sHtML

val a = 1;  var b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/goqqdwlnl.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdpfgmgj.sHtML

s"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpwsuvee.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gahbcrbit.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gvanrdbvn.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gzoaubimr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefrxzcry.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/gixchwpdw.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/glwmfhlbh.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhxomnkq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwtznjln.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/gpzeesnea.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gofxxuhdh.sHtML

[T59] Scala：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/goohjzvfe.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gtnfyxxzp.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/gllezelhu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/gndvomjuq.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gfeharhge.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfadvheae.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gjobhtpfs.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fanxiaobao.xyz/Article/details/gjnjjmesf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbnkiuep.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjvbokwg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/grvnupgcp.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fanxiaobao.xyz/Article/details/gwntsvcgp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/gefpguxhu.sHtML

[U04] Py：变量调试打印
来源：http://blog.fanxiaobao.xyz/Article/details/govydbspk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fanxiaobao.xyz/Article/details/gpcaqkggf.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fanxiaobao.xyz/Article/details/gypihaemn.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gnqohcjrm.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrhywsbj.sHtML

{**a, **b}
来源：http://wap.fanxiaobao.xyz/Article/details/gaqmqogbc.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbhurvcb.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/gppaglrir.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzbicibn.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/glkrdfbig.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwxmrioq.sHtML

max(d, key=d.get)
来源：http://blog.fanxiaobao.xyz/Article/details/gsiwilddg.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/glucxxyoz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpoezaoj.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhvdfzys.sHtML

(x * 2 for x in arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmlyyuxd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fanxiaobao.xyz/Article/details/gprkcrvrt.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gssuhiymu.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipvtvslb.sHtML

deque(maxlen=10)
来源：http://3g.fanxiaobao.xyz/Article/details/gwgshvlrb.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxrnyrcf.sHtML

defaultdict(list)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxnwqfrc.sHtML

[U15] Py：高精度计时
来源：http://3g.fanxiaobao.xyz/Article/details/givqxvyfe.sHtML

t = time.perf_counter()
来源：http://wap.fanxiaobao.xyz/Article/details/gysbqqusq.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gyejbpwme.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmppjcfpt.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gqulxfedy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fanxiaobao.xyz/Article/details/gigiztkah.sHtML

[U18] Py：预编译正则
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqkrbcgt.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyftvtld.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fanxiaobao.xyz/Article/details/gqknzscgk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gotvnpupo.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/grjlrgxkc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fanxiaobao.xyz/Article/details/guobgivee.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdkcnqkk.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnqbabqh.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxdjfpxu.sHtML

list(zip(*m))
来源：http://blog.fanxiaobao.xyz/Article/details/gsxqxqpcz.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnonidjle.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fanxiaobao.xyz/Article/details/gybmpknqu.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gzcixnpec.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gpdyqqwlt.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyaajaox.sHtML

csv.DictReader(f)
来源：http://3g.fanxiaobao.xyz/Article/details/gbqyumsxe.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwcsqhlc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fanxiaobao.xyz/Article/details/ggsclcbdu.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fanxiaobao.xyz/Article/details/gwloqlzse.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fanxiaobao.xyz/Article/details/gqaucaphl.sHtML

[U28] Py：类型别名
来源：http://m.share.fanxiaobao.xyz/Article/details/gmooxvisu.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/gnaceohvs.sHtML

[U29] Py：属性校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsvbyjgx.sHtML

@property 与 @x.setter 配合
来源：http://blog.fanxiaobao.xyz/Article/details/gvfdbfred.sHtML

[U30] Py：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gfeumlpfo.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbggwzmmp.sHtML

[U31] Py：单测
来源：http://3g.fanxiaobao.xyz/Article/details/gfrhizlgx.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/gtqjuhrup.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpnbxopm.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fanxiaobao.xyz/Article/details/grejasagf.sHtML

[U33] Py：打包发布
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuiwesdw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fanxiaobao.xyz/Article/details/gysxmengh.sHtML

[U34] Py：判断编码
来源：http://wap.fanxiaobao.xyz/Article/details/glystorqg.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/gmujzurgw.sHtML

[U35] Py：发送邮件
来源：http://3g.fanxiaobao.xyz/Article/details/gnrlnehji.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjomyfeza.sHtML

[U36] Py：定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdedmhmb.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhoyvhum.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsdnxsxz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fanxiaobao.xyz/Article/details/ggykozyor.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fanxiaobao.xyz/Article/details/gzfcehgpp.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fanxiaobao.xyz/Article/details/gwopfielx.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fanxiaobao.xyz/Article/details/gpxzaeyaq.sHtML

sys.stdout.isatty()
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvlycysy.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdzdketo.sHtML

print("err", file=sys.stderr)
来源：http://blog.fanxiaobao.xyz/Article/details/gzjkhlaxk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvphxzfog.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fanxiaobao.xyz/Article/details/ggulwloft.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/gehxrveog.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fanxiaobao.xyz/Article/details/gckltkthq.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gmquzxwga.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/ghwkfbmyb.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fanxiaobao.xyz/Article/details/gljpopvlb.sHtML

declare(strict_types=1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvdjrnnh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhjlmkxs.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunrswoiw.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazzyuyae.sHtML

?string $name = null
来源：http://read.share.fanxiaobao.xyz/Article/details/gbthwgsdm.sHtML

[U47] PHP：联合类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjunrnas.sHtML

int|string $id
来源：http://blog.fanxiaobao.xyz/Article/details/gkfprpumy.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gvazmloev.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdbturcos.sHtML

[U49] PHP：只读属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkimjsla.sHtML

public readonly string $name
来源：http://baike.fanxiaobao.xyz/Article/details/gcwkjeuae.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/gvowrujhb.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbzuacds.sHtML

[U51] PHP：数组解构
来源：http://mobile.fanxiaobao.xyz/Article/details/ghymnaezs.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakscnzxt.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlabbrqc.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gkwklfhqg.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fanxiaobao.xyz/Article/details/gymenpbav.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fanxiaobao.xyz/Article/details/gxhacuayw.sHtML

[U54] PHP：空安全调用
来源：http://baike.fanxiaobao.xyz/Article/details/gvkllzzhc.sHtML

$obj?->method()
来源：http://wap.fanxiaobao.xyz/Article/details/gjlhqzjvq.sHtML

[U55] PHP：match 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gqxuvjlpl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fanxiaobao.xyz/Article/details/giornapmu.sHtML

[U56] PHP：命名参数
来源：http://m.share.fanxiaobao.xyz/Article/details/grgybmghf.sHtML

f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbthspyr.sHtML

[U57] PHP：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gxswfopqc.sHtML

"值: {$a}"
来源：http://read.share.fanxiaobao.xyz/Article/details/giqkprjbr.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqtqvbne.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/guepnwdbt.sHtML

[U59] PHP：自定义排序
来源：http://baike.fanxiaobao.xyz/Article/details/gyhfqobig.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gogifzaww.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fanxiaobao.xyz/Article/details/gncpmskbd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvugakpbc.sHtML

[U61] PHP：正则
来源：http://3g.fanxiaobao.xyz/Article/details/gxzpbvuwd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gbprhfbth.sHtML

[U62] PHP：日期对象
来源：http://baike.fanxiaobao.xyz/Article/details/gqegxprnd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fanxiaobao.xyz/Article/details/gbamyxmgn.sHtML

[U63] PHP：文件读写
来源：http://wap.fanxiaobao.xyz/Article/details/gttvybgqz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fanxiaobao.xyz/Article/details/glbjummaj.sHtML

[U64] PHP：目录遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gmpubynfy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkvxpelh.sHtML

[U65] PHP：会话
来源：http://blog.fanxiaobao.xyz/Article/details/gdmtodcst.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/glbvdrbpp.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxsadzon.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gslglycul.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fanxiaobao.xyz/Article/details/giwxeffrz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrhreror.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fanxiaobao.xyz/Article/details/gewtctbuu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fanxiaobao.xyz/Article/details/gtwcudvqh.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsfpiiym.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyukoiod.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fanxiaobao.xyz/Article/details/guowkemlv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fanxiaobao.xyz/Article/details/gpwldalfr.sHtML

[U71] PHP：抛出异常
来源：http://baike.fanxiaobao.xyz/Article/details/gvaxbnpyk.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxpuqkvt.sHtML

[U72] PHP：写错误日志
来源：http://wap.fanxiaobao.xyz/Article/details/gejysxthn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbftoqbo.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyewzdsm.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjwclzmf.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gfqyohrzb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fanxiaobao.xyz/Article/details/gclqvbzbl.sHtML

[U75] PHP：依赖注入
来源：http://wap.fanxiaobao.xyz/Article/details/geznevtji.sHtML

composer require psr/container
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguxknunk.sHtML

[U76] PHP：简单路由
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhofrdzy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fanxiaobao.xyz/Article/details/gfofqiifl.sHtML


<!-- 参考信息 -->