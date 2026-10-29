代发 wailian999

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/ghnbbeztl.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gbdhewcqs.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/gpukubmpj.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gdtbjjofp.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/gyyfmzrof.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/glrsxkaol.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/grlxvvcgl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gciwicgwl.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gzabklaof.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gcnqratxn.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gjpwmtcmj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/glniuaxcz.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/gfyafujso.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/guvpurrgw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gfxesgxot.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gfotjopal.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gdcvzkfys.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/girpmnosu.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/glbeuohoh.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gconztmgx.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gqpbduuvr.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/gyfkgdszc.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gkimjnthz.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/gonvxyhlb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/gwnvjtqec.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gkbxxisjs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/glxnpichi.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gpjfcbbtd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/guzsyzzcl.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/gsmgbwczy.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/gyxgapysh.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/goelogiru.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gapdpwldo.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gvarzmxxj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/gubrjzelr.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/guqmgosjl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gvvrplxnm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gntwhbwpb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gxwrovyca.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzylcnwgz.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/govhxdkxn.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gyfwfhprs.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gytnvowuf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/girshakjl.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/gkdttqlyx.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/glxflgpum.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/geejnsked.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/gfroinjei.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gtnatohne.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gntkxzngo.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gkuzezchd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gvtowajrb.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/gawrgpjav.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/gcfpdwjky.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/glpbhfuvc.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gamjhjowb.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/guhvgwaew.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/grulhkrae.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gjwelqppg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/gvhafigkm.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/gjfgnvkjq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/gxkuwjept.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gyzeslzmo.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gjqualtwx.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gdwkipxsl.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/gyblkdmxi.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/ggfeugchf.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/gjjhncpsi.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/glnqenmnv.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/grahifngd.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/guithqtqy.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gzhiwmdar.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/gnhpliscd.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/grwemgvdo.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/ggftuoate.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/glyeyretp.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gdqapihpr.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/geqcutqtu.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/gmktqdxur.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gyhqspbee.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/guszbxeew.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/gpxpykbxh.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/guyvnuhmn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gqjstskez.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gxzqvzjqi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gwxtigtan.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gsenjhqge.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gajljokho.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/ggkjacubm.sHtML

struct P { var x: Int }
来源：http://www.m.share.zdbjq.cn/Article/details/gwdywqrjj.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/gdlzchhhw.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gczqoyviv.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gddnkruzu.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.hesvh.cn/Article/details/gdidokygh.sHtML

[T28] Swift：枚举
来源：http://www.blog.fehbvm.com/Article/details/gbqjoluod.sHtML

enum Color { case red, green }
来源：http://www.share.fehbvm.com/Article/details/gnencjyaj.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/gguiulghf.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/gxfthgzgj.sHtML

[T30] Swift：协议
来源：http://m.share.fehbvm.com/Article/details/gmwapdqnn.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/gwnzvjeme.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gwdjiuabd.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/ghyxmfcgx.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/gryiauptz.sHtML

local a = 1
来源：http://baike.zdbjq.cn/Article/details/gutimqmue.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/grgulfsuz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gwwfmpptx.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/gpjytpcqw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/gicxlwxwj.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gzjolqmfx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gevcpuuea.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/gqtzgytlt.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/gfbqsbkzs.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gyzwiwjjk.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/gleyebfvn.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/gvyccbvvv.sHtML

if x > 0 then print("正") end
来源：http://m.share.zdbjq.cn/Article/details/gnomlmera.sHtML

[T39] Lua：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gvwqimpax.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/gwgpqwqrk.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/gzpeorhru.sHtML

setmetatable({}, { __index = base })
来源：http://wap.zdbjq.cn/Article/details/grehbldpa.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/guebkmnbv.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/gjsktfhah.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gjugtzblj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.zdbjq.cn/Article/details/gqyqmmuyf.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gwjwxzybj.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/gblfbdlhy.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/glkrbhcym.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fehbvm.com/Article/details/gkmamzxux.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gbdxhtkkg.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.hesvh.cn/Article/details/gbhukshol.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fehbvm.com/Article/details/gjbrjctlb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gnvsbcbqg.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gnbccdacj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/gcteblecz.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/gpeuywfys.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/gewtfdzlm.sHtML

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/gslmfltbw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gpagmabvt.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gcbbspwuo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.hesvh.cn/Article/details/gtteiuqct.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gaebtlazi.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gkjdtyzob.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gdiezdcdc.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gyhsovjhu.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gnqryikbv.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fehbvm.com/Article/details/glogbcnvt.sHtML

s"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gktnxvzwm.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/ggdvmrxjp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/gyfhcrrnz.sHtML

[T55] Scala：集合过滤
来源：http://3g.fehbvm.com/Article/details/gbdntllne.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/gcjnhrdjv.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/gqeufowco.sHtML

case class User(name: String, age: Int)
来源：http://www.share.hesvh.cn/Article/details/gczjqfueu.sHtML

[T57] Scala：模式匹配
来源：http://baike.zdbjq.cn/Article/details/glskszehw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/gxrzvkhbx.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/gzcbnkpnk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fehbvm.com/Article/details/gwvehlfjz.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/gprswvajs.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/gybrodimn.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/geuzrijrf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.zdbjq.cn/Article/details/gcbjpqusf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqxomsgxu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gwljxajwb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggjvmpqtq.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/gzkehbozp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/giqmobety.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/gllwzaieb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/ghyeoxpch.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fehbvm.com/Article/details/guygbopaj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/gagomdejb.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/gnsciuoiu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/glrrzimoy.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.zdbjq.cn/Article/details/gswtrqcvg.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gjzpyxplr.sHtML

[U06] Py：合并两个字典
来源：http://baike.hesvh.cn/Article/details/gbmzgzrla.sHtML

{**a, **b}
来源：http://baike.zdbjq.cn/Article/details/gqzhpqebc.sHtML

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/ggheltsdn.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/gznyswogx.sHtML

[U08] Py：展平二维列表
来源：http://wap.zdbjq.cn/Article/details/ggormjtik.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/grypxbmrk.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/gbytrkiay.sHtML

max(d, key=d.get)
来源：http://3g.zdbjq.cn/Article/details/gkbamdnrg.sHtML

[U10] Py：按值排序字典
来源：http://www.share.hesvh.cn/Article/details/ggktoarbd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.hesvh.cn/Article/details/gidfwjbua.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/gssypdejw.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/galehsipy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/gqgdfgjif.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/gsxalxwfh.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gkkbjxhdd.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/gjbfypcdk.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.hesvh.cn/Article/details/gbihorgna.sHtML

defaultdict(list)
来源：http://3g.zdbjq.cn/Article/details/glrugczpb.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gemofvuag.sHtML

t = time.perf_counter()
来源：http://mobile.fehbvm.com/Article/details/guwmsrhrx.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/gkjqfyknz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/ggfwoygnl.sHtML

[U17] Py：初始化日志
来源：http://m.share.zdbjq.cn/Article/details/gvizptemz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.hesvh.cn/Article/details/geelptdpl.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/gaatjuvbp.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gkeklpuwh.sHtML

[U19] Py：正则替换带回调
来源：http://blog.zdbjq.cn/Article/details/golneozcx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.hesvh.cn/Article/details/gunbjtqsy.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fehbvm.com/Article/details/gmqividot.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fehbvm.com/Article/details/gksiolvgl.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/gulhfdjuc.sHtML

@contextlib.contextmanager
来源：http://www.blog.zdbjq.cn/Article/details/ghdygjayt.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.zdbjq.cn/Article/details/gbqpokizj.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gxfukmpqe.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gsqmnynbq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/gaozucant.sHtML

[U24] Py：路径操作
来源：http://www.blog.fehbvm.com/Article/details/gakbgipze.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gphctvsax.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gfpcvkcbh.sHtML

csv.DictReader(f)
来源：http://blog.hesvh.cn/Article/details/gropgtdrq.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/grmjbymqf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.zdbjq.cn/Article/details/gyuacclos.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gsydprxgd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/gunvvwyks.sHtML

[U28] Py：类型别名
来源：http://read.share.fehbvm.com/Article/details/gbtmfaizi.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/gbkbxuxut.sHtML

[U29] Py：属性校验
来源：http://mobile.hesvh.cn/Article/details/gtaaxxihv.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.zdbjq.cn/Article/details/gpemgptwp.sHtML

[U30] Py：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gevgnrwag.sHtML

@dataclass(slots=True)
来源：http://wap.hesvh.cn/Article/details/geedurdtc.sHtML

[U31] Py：单测
来源：http://www.share.hesvh.cn/Article/details/gikdwtplf.sHtML

python -m pytest -q
来源：http://3g.zdbjq.cn/Article/details/gocixzdvh.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fehbvm.com/Article/details/groajaiei.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fehbvm.com/Article/details/gswoqpqng.sHtML

[U33] Py：打包发布
来源：http://3g.zdbjq.cn/Article/details/grafcuekc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/geroywocj.sHtML

[U34] Py：判断编码
来源：http://baike.zdbjq.cn/Article/details/gumdkuhgt.sHtML

chardet.detect(raw)
来源：http://wap.fehbvm.com/Article/details/gvnqpigdf.sHtML

[U35] Py：发送邮件
来源：http://read.share.zdbjq.cn/Article/details/gmxyynzsy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fehbvm.com/Article/details/gkdwgrvgq.sHtML

[U36] Py：定时任务
来源：http://wap.fehbvm.com/Article/details/gltwseqlf.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/gijgptmyj.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fehbvm.com/Article/details/gqagkfuxx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fehbvm.com/Article/details/gjdcitckg.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.zdbjq.cn/Article/details/gthrwkhnb.sHtML

Path(__file__).resolve().parent
来源：http://wap.zdbjq.cn/Article/details/gvcyzyfec.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/gpbeuuhbg.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/gwixijast.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.hesvh.cn/Article/details/gvfpwndjn.sHtML

print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gpmirgemy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/goavnbpeg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/gkxwnzwgb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.hesvh.cn/Article/details/gtjffzojy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fehbvm.com/Article/details/gkemelffh.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/guzqctwsc.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/gdsgkgsnf.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.hesvh.cn/Article/details/galjbfzac.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/gdwwbeopw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fehbvm.com/Article/details/gqzbkhvgq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gejkpdpvy.sHtML

[U46] PHP：可空类型
来源：http://www.blog.hesvh.cn/Article/details/goyozdjsj.sHtML

?string $name = null
来源：http://wap.fehbvm.com/Article/details/gxzasvbkx.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/grpfadiyf.sHtML

int|string $id
来源：http://baike.hesvh.cn/Article/details/gnbpdczqv.sHtML

[U48] PHP：纯枚举
来源：http://mobile.zdbjq.cn/Article/details/gvdgpvvta.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.hesvh.cn/Article/details/gbnryihxl.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/gqvfndjzi.sHtML

public readonly string $name
来源：http://www.m.share.zdbjq.cn/Article/details/gnhkmuetj.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.zdbjq.cn/Article/details/gbktvrmiz.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fehbvm.com/Article/details/grblvhlzx.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/gznfqjewb.sHtML

[$a, $b] = $arr;
来源：http://www.share.hesvh.cn/Article/details/gengurxyl.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/gquleokcz.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.hesvh.cn/Article/details/gkwtxcmhd.sHtML

[U53] PHP：空合并运算符
来源：http://3g.zdbjq.cn/Article/details/gwqrwpnrq.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.zdbjq.cn/Article/details/gkpiariiz.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/gzmjgvqnb.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gwrgsqvtm.sHtML

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/gxycragyj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.zdbjq.cn/Article/details/glghacais.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/gkszqibfz.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gtfbtrigg.sHtML

[U57] PHP：字符串插值
来源：http://blog.fehbvm.com/Article/details/gytcnmkkb.sHtML

"值: {$a}"
来源：http://3g.zdbjq.cn/Article/details/gppjasgjy.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fehbvm.com/Article/details/ghhxmixex.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/grxftaqdp.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/gpvdmsobj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/geiveqgbk.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.zdbjq.cn/Article/details/gammpjeat.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fehbvm.com/Article/details/gmphxbnyh.sHtML

[U61] PHP：正则
来源：http://blog.hesvh.cn/Article/details/gynelepqq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/gseydviqt.sHtML

[U62] PHP：日期对象
来源：http://blog.hesvh.cn/Article/details/gvpklcvxj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.zdbjq.cn/Article/details/gkmogakaz.sHtML

[U63] PHP：文件读写
来源：http://read.share.hesvh.cn/Article/details/gdnmufsxz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/glpjmudwx.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fehbvm.com/Article/details/gqzsisozj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.zdbjq.cn/Article/details/gjioknqjy.sHtML

[U65] PHP：会话
来源：http://m.share.fehbvm.com/Article/details/gsqnemvtg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.hesvh.cn/Article/details/ghrxohtnt.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fehbvm.com/Article/details/gmnqcdkcd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fehbvm.com/Article/details/gnrooizfv.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/gmuoeugza.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.zdbjq.cn/Article/details/giupjrqdb.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.zdbjq.cn/Article/details/geayiwmsc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.hesvh.cn/Article/details/garmclxab.sHtML


<!-- 参考信息 -->