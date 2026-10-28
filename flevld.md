代发 wailian999

x |= (1 << 3);
来源：http://hz.kuanghao11.cn/gttmkxzpog.html

[S17] C：安全拼接字符串
来源：http://hz.shuidangran.top/gtijpgrxti.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.haohaochexian.top/gtmttvdbzx.html

[S18] C：命令行参数
来源：http://hz.feifeiyinyue.top/gtlxdvfqpj.html

int main(int argc, char **argv)
来源：http://hz.yonumen.top/gtcggugxdt.html

[S19] C：快速排序
来源：http://hz.yonumen.top/gtisdvonnu.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.xziqi.cn/gtafbahvrp.html

[S20] C：二分查找
来源：http://hz.yj20258888.top/gtgwlvswsi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hysaishi.cn/gtlsrnkoyb.html

[S21] C：字符类别判断
来源：http://hz.jinghuilouyu.cn/gtgywlibjd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.shanyushiyangtech.top/gttwzwmjhs.html

[S22] C：字符串转数字
来源：http://hz.shzxlz.cn/gtninydtcx.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.birdmap.top/gtgfynovce.html

[S23] C：随机数
来源：http://hz.shzxlz.cn/gtjrgefstz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.gzhubu.top/gtzcafvyhj.html

[S24] C：获取本地时间
来源：http://hz.yanxiufei.cn/gtozxnekdv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.havefunace.top/gtsociohtw.html

[S25] C：内存拷贝
来源：http://hz.hnxiangtu.top/gttvebqtwr.html

memcpy(dst, src, n);
来源：http://hz.quarkkingdee.top/gtotfasjmz.html

[S26] C：内存清零
来源：http://hz.ydjk.org.cn/gtfzrxftze.html

memset(a, 0, sizeof a);
来源：http://hz.aibaodan.cn/gtkhthgzla.html

[S27] C：定义常量
来源：http://hz.tianlin.xyz/gtiqnltckc.html

const double PI = 3.14159;
来源：http://hz.ywan-chungtsiang.top/gtnanwgghj.html

[S28] C：静态变量
来源：http://hz.shanyushiyangkeji.top/gtqunujhpq.html

static int counter = 0;
来源：http://hz.gaohongyu789.top/gtwdmqfney.html

[S29] C：变参函数
来源：http://hz.jqgufenzy.top/gtxohswnlh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.wangdashe.top/gtwgwbbiwt.html

[S30] C：头文件保护
来源：http://hz.gzhubu.top/gtuvkfmozc.html

#ifndef X_H
来源：http://hz.tian-w.cn/gtqgaonvzj.html

#define X_H
来源：http://hz.shanyushiyangkeji.top/gtiohnuugw.html

#endif
来源：http://hz.jinqigfzy.top/gtwpsqrngw.html

[S31] C++：Hello World
来源：http://hz.chenzaomai.com/gtgebfpcbd.html

#include <iostream>
来源：http://hz.cqqwz.cn/gtwwxwmafk.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.feifeiyinyue.top/gtubageszx.html

[S32] C++：字符串
来源：http://hz.c1oappe.top/gtiyzpaxxp.html

std::string s = "hi";  s += "!";
来源：http://hz.0kj1m.cn/gtvlkjlbkd.html

[S33] C++：vector 增删
来源：http://hz.vqdsnc.cn/gtofbascaa.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shzxlz.cn/gtqsjpwlmx.html

[S34] C++：遍历 vector
来源：http://hz.redwolf501.top/gtqoewsike.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.sxryk.cn/gtgivdpzay.html

[S35] C++：map
来源：http://hz.sweek.top/gthcgndzdu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tianlin.xyz/gteqyktwbd.html

[S36] C++：unordered_map
来源：http://hz.jyoumei.cn/gtggslahza.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cheryme.top/gtorslafaa.html

[S37] C++：set
来源：http://hz.fengsongda.top/gttcjwronu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yanxiufei.cn/gttimimkwv.html

[S38] C++：排序
来源：http://hz.cheryme.top/gtesscstdz.html

std::sort(v.begin(), v.end());
来源：http://hz.zhaomingkeji.xyz/gtqfvdpouf.html

[S39] C++：自定义比较器排序
来源：http://hz.cqqwz.cn/gtackspgcv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jqgfzy.top/gtmfmzpdez.html

[S40] C++：查找元素
来源：http://hz.52xcode.cn/gtnydaajzx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hammf.cn/gtejusfebk.html

[S41] C++：类与构造函数
来源：http://hz.fengsongda.top/gteuigeuno.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yanxiufei.cn/gtvnmaafvb.html

[S42] C++：继承与虚函数
来源：http://hz.yongpay.top/gtkhgwtguh.html

class B : public Base { public: void f() override {} };
来源：http://hz.ywan-chungtsiang.top/gtzehzjjqn.html

[S43] C++：智能指针
来源：http://hz.chenjidiqi.icu/gtebvnddpg.html

auto p = std::make_unique<int>(5);
来源：http://hz.cdnleiting.top/gthhkahzfb.html

[S44] C++：引用传参
来源：http://hz.zhongyouzk.top/gttcfimvsx.html

void inc(int &x) { ++x; }
来源：http://hz.wangdashe.top/gtwkulhanc.html

[S45] C++：lambda
来源：http://hz.sweek.top/gtyebolqxf.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yuxming.cn/gtdmefbxcd.html

[S46] C++：函数模板
来源：http://hz.shanyushiyangkeji.top/gtfzmohfel.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shanyushiyangtech.top/gtlhxlptkv.html

[S47] C++：结构化绑定遍历
来源：http://hz.jqgfzy.top/gtmwtsyxio.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jqgfzy.top/gtqrcgkmby.html

[S48] C++：逐行读文件
来源：http://hz.wangdashe.top/gtlvcmhozz.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.xuanzx.com/gtaduhxjtp.html

while (std::getline(in, line)) { }
来源：http://hz.dashuyun.cn/gtquxrmbtj.html

[S49] C++：写文件
来源：http://hz.smart0.xyz/gtsmjwriro.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.iojbl.cn/gtdjhhtlwf.html

[S50] C++：格式化数字
来源：http://hz.cqqwz.cn/gtbtubxufh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.ybcxt.top/gtknotrbcm.html

[S51] C++：显式类型转换
来源：http://hz.andypj.xyz/gtfceeeglm.html

static_cast<double>(a) / b
来源：http://hz.shuidangran.top/gteuaqucki.html

[S52] C++：const 与 noexcept
来源：http://hz.0kj1m.cn/gtanbfyerk.html

int size() const noexcept { return n_; }
来源：http://hz.jinghuilouyu.cn/gtstlccegy.html

[S53] C++：移动语义
来源：http://hz.0kj1m.cn/gtixkwuxeo.html

std::vector<int> w = std::move(v);
来源：http://hz.feifeiyinyue.top/gtrwfpbxwd.html

[S54] C++：异常处理
来源：http://hz.yvedp.cn/gthnmceglu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.haohaochexian.top/gtaqnsrnlq.html

[S55] C++：结构化绑定
来源：http://hz.jinqigufen.top/gtsakfolci.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.wangdashe.top/gtrrqfhnym.html

[S56] C++：optional
来源：http://hz.chenzaomai.com/gtykkssxzb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.dianchejie.cn/gtwcdqvcnf.html

[S57] C++：编译期常量
来源：http://hz.shanyushiyangtech.top/gtxonkvyiq.html

constexpr int N = 10;
来源：http://hz.guannengcc.top/gtchrynlmv.html

[S58] C++：命名空间
来源：http://hz.yj20258.top/gtpelceakd.html

namespace ns { int f() { return 1; } }
来源：http://hz.zycfv.cn/gttvezulul.html

[S59] C++：静态断言
来源：http://hz.ydjk.org.cn/gtphukcciv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jianghu66.top/gtrlppjwax.html

[S60] C++：遍历并删除元素
来源：http://hz.zhixingplan.top/gtbxhyvlie.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.dashuyun.cn/gtuvdayaks.html

================================================================================
来源：http://hz.xylfe.cn/gtcyixsehc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xuetiantiany.cn/gtzvxctfrv.html

================================================================================
来源：http://hz.zhengqikj.top/gtwqafrgmu.html

[T01] Kotlin：Hello World
来源：http://hz.hywenlv.cn/gthazahuas.html

println("Hello")
来源：http://hz.xinyue.icu/gtibeetyrc.html

[T02] Kotlin：变量
来源：http://hz.zhaomingkeji.xyz/gtrnkichrw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.guowangkeji.top/gtdaeeblfu.html

[T03] Kotlin：字符串模板
来源：http://hz.yj20258.top/gtueplttug.html

"值: $b"
来源：http://hz.andypj.xyz/gtxckqlytc.html

[T04] Kotlin：空安全
来源：http://hz.hammf.cn/gtnxtktiuh.html

val n: String? = null;  n?.length
来源：http://hz.gzhubu.top/gtmzytqjmn.html

[T05] Kotlin：when 表达式
来源：http://hz.hnxiangtu.top/gtlsdzczmr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.9152youxi.cn/gtejtgwlqr.html

[T06] Kotlin：集合映射
来源：http://hz.andypj.xyz/gtydbrcpdp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yj202588.top/gtazcluydj.html

[T07] Kotlin：集合过滤
来源：http://hz.sufxvd.cn/gtgbdathqt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zycfv.cn/gtveasfyhb.html

[T08] Kotlin：数据类
来源：http://hz.cdnleiting.top/gtgxvxhwfl.html

data class User(val name: String, val age: Int)
来源：http://hz.zhijiandao.cn/gtbdzxhzae.html

[T09] Kotlin：扩展函数
来源：http://hz.daxiang520.top/gthbioezan.html

fun String.exclaim() = this + "!"
来源：http://hz.zhiwuduotai.top/gtdhcqlmuf.html

[T10] Kotlin：默认参数
来源：http://hz.zhaomingkeji.xyz/gtiklcqucv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yuanzhike.top/gtxgtwiaqf.html

[T11] Kotlin：协程
来源：http://hz.cashguo.top/gtdqpdczig.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.cqqwz.cn/gtxiedtmow.html

[T12] Kotlin：解构声明
来源：http://hz.zhaomingkeji.xyz/gtbmkaqobl.html

val (a, b) = Pair(1, 2)
来源：http://hz.gaohongyu789.top/gtdasfztac.html

[T13] Kotlin：只读 Map
来源：http://hz.pycfn.com/gtekselvqn.html

val m = mapOf("a" to 1)
来源：http://hz.kuanghao11.cn/gtxkolmfon.html

[T14] Kotlin：循环
来源：http://hz.9152youxi.cn/gtoyxnpiuk.html

for (i in 1..10) println(i)
来源：http://hz.tian-w.cn/gteqlfyetq.html

[T15] Kotlin：接口
来源：http://hz.fengsongda.top/gtzcwaurcx.html

interface Shape { fun area(): Double }
来源：http://hz.xylfe.cn/gtxuiopigo.html

[T16] Swift：Hello World
来源：http://hz.hywenlv.cn/gtwcaihwmr.html

print("Hello")
来源：http://hz.svipenyu.cn/gtlzyxjdfq.html

[T17] Swift：变量与常量
来源：http://hz.xuetiantiany.cn/gtmytowhht.html

var a = 1;  let b = 2
来源：http://hz.aizwys.cn/gtgarrrfqb.html

[T18] Swift：字符串插值
来源：http://hz.havefunace.top/gtljnpxgtp.html

"值: \(b)"
来源：http://hz.yongpay.top/gtgrolceyv.html

[T19] Swift：可选绑定
来源：http://hz.zycfv.cn/gtavwxkant.html

if let n = opt { print(n) }
来源：http://hz.daxiang520.top/gtnbwnbdtf.html

[T20] Swift：数组操作
来源：http://hz.smart0.xyz/gtuojztvex.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jiagoushi.top/gthekbfkgi.html

[T21] Swift：遍历
来源：http://hz.xingfuxueyuan.xyz/gthdlwceat.html

for x in a { print(x) }
来源：http://hz.vqdsnc.cn/gtuoifqdrk.html

[T22] Swift：字典
来源：http://hz.zdqjudy.top/gtcespiubl.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.shanyushiyangkeji.top/gtrslmpgnn.html

[T23] Swift：函数
来源：http://hz.9152youxi.cn/gtuwuxjbem.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.hongshengwenyu.top/gtkouyniei.html

[T24] Swift：闭包
来源：http://hz.yonumen.top/gthnhaionr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.shangyingyoupin.top/gtdrmcafmt.html

[T25] Swift：结构体
来源：http://hz.hongshengwenyu.top/gttnolfnwk.html

struct P { var x: Int }
来源：http://hz.svipenyu.cn/gtrgchkyup.html

[T26] Swift：类与重写
来源：http://hz.yvedp.cn/gtheqlsmky.html

class A: Base { override func f() {} }
来源：http://hz.fengsongda.top/gtsvgzsvno.html

[T27] Swift：错误处理
来源：http://hz.xziqi.cn/gtrmgikfji.html

do { try f() } catch { print(error) }
来源：http://hz.zhoulong.xyz/gtqipbcnry.html

[T28] Swift：枚举
来源：http://hz.0kj1m.cn/gtqzaouqjs.html

enum Color { case red, green }
来源：http://hz.yuanzhike.top/gtdwtyywfv.html

[T29] Swift：guard 提前返回
来源：http://hz.quarkkingdee.top/gtygwzqlxw.html

guard let x = opt else { return }
来源：http://hz.meibo888.top/gtqmwcctyn.html

[T30] Swift：协议
来源：http://hz.jyoumei.cn/gtlhfgdwre.html

protocol Shape { func area() -> Double }
来源：http://hz.jqgfzy.top/gtbzpiwyah.html

[T31] Lua：Hello World
来源：http://hz.hywenlv.cn/gtcntxdjbj.html

print("Hello")
来源：http://hz.chenzaomai.com/gtiubvagnr.html

[T32] Lua：局部变量
来源：http://hz.yj20258888.top/gtqyrfxndp.html

local a = 1
来源：http://hz.andypj.xyz/gtoymnlarx.html

[T33] Lua：表（数组）
来源：http://hz.xuetiantiany.cn/gtsrwqjcbv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.gzhubu.top/gtaponcqfg.html

[T34] Lua：遍历表
来源：http://hz.hfpthk.cn/gtjpityvwa.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.hysaishi.cn/gtqlhxhbcv.html

[T35] Lua：字典表
来源：http://hz.sxryk.cn/gtboplgwpd.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jqgufenzy.top/gtigbgwsgf.html

[T36] Lua：函数
来源：http://hz.quarkkingdee.top/gtqrztopqf.html

function add(a, b) return a + b end
来源：http://hz.andypj.xyz/gtfehhtzgg.html

[T37] Lua：字符串拼接
来源：http://hz.wangdashe.top/gtbesdtyon.html

"a" .. "b"
来源：http://hz.zhoulong.xyz/gtlmyrethc.html

[T38] Lua：条件
来源：http://hz.sysykeji.top/gtpphnhojw.html

if x > 0 then print("正") end
来源：http://hz.chenjidiqi.icu/gtixzwtzic.html

[T39] Lua：模式匹配
来源：http://hz.aizwys.cn/gtupstbcia.html

string.find(s, "%d+")
来源：http://hz.feifeiyinyue.top/gtfkvjjojv.html

[T40] Lua：元表
来源：http://hz.jinyuanbaomall.cn/gtsyiwaqbn.html

setmetatable({}, { __index = base })
来源：http://hz.smart0.xyz/gtcrkgayqr.html

[T41] Perl：Hello World
来源：http://hz.jianghu66.top/gtpffslplk.html

print "Hello\n";
来源：http://hz.tianlin.xyz/gttfpfpobk.html

[T42] Perl：变量类型
来源：http://hz.jlsjyb.cn/gtueioulmx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yangfankeji.com/gtifpnbogp.html

[T43] Perl：字符串插值
来源：http://hz.zdqjudy.top/gtbaxovrqt.html

"值: $a"
来源：http://hz.shanyushiyangtech.top/gtrszmkadt.html

[T44] Perl：条件
来源：http://hz.dianchejie.cn/gtaqgifeuj.html

if ($a > 0) { print "正"; }
来源：http://hz.haohaochexian.top/gtriirbfri.html

[T45] Perl：数组遍历
来源：http://hz.zhongyouzk.top/gtqffmrwsm.html

for my $x (@arr) { print $x; }
来源：http://hz.nanxuanxn.top/gtgckdpmpe.html

[T46] Perl：哈希操作
来源：http://hz.yuxming.cn/gtbpiabmjy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.hnxiangtu.top/gtwozavcrw.html

[T47] Perl：正则捕获
来源：http://hz.jinqigfzy.top/gtvahfaiwo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.ppjwa.cn/gtqexfpisa.html

[T48] Perl：正则替换
来源：http://hz.ydjk.org.cn/gtdicqxarf.html

$s =~ s/old/new/g;
来源：http://hz.nanxuanxn.top/gtkqghxvas.html

[T49] Perl：函数
来源：http://hz.yj202588.top/gtgkbzzssr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.daxiang520.top/gtoggxjjku.html

[T50] Perl：逐行读文件
来源：http://hz.yongpay.top/gtxhsnaypg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.ehwqpu.com/gtdpeupzbv.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yvedp.cn/gtkjinlkiz.html

[T51] Scala：Hello World
来源：http://hz.sxryk.cn/gtrlkfmgck.html

println("Hello")
来源：http://hz.kuanghao11.cn/gtblyqjtxx.html

[T52] Scala：变量
来源：http://hz.wangdashe.top/gtpkhgsfyi.html

val a = 1;  var b = 2
来源：http://hz.xuetiantiany.cn/gtrcfaxscq.html

[T53] Scala：字符串插值
来源：http://hz.shzxlz.cn/gtwjytuvfd.html

s"值: $b"
来源：http://hz.xinyue.icu/gtyrtxovso.html

[T54] Scala：集合映射
来源：http://hz.nanxuanxn.top/gtappuylos.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.mhx1999.top/gtvlkwssqm.html

[T55] Scala：集合过滤
来源：http://hz.shanyushiyangtech.top/gtssgvxkzn.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.hywenlv.cn/gteiqncelk.html

[T56] Scala：样例类
来源：http://hz.pengpengdd.cyou/gtoldiqsbj.html

case class User(name: String, age: Int)
来源：http://hz.zhengqikj.top/gtiatwrhmi.html

[T57] Scala：模式匹配
来源：http://hz.tianlin.xyz/gtdzasegml.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.ybcxt.top/gtaluijigi.html

[T58] Scala：函数定义
来源：http://hz.aibaodan.cn/gtavjcqlgc.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.ydzc1.top/gtoclddbrv.html

[T59] Scala：循环
来源：http://hz.dianchejie.cn/gthkytjgbo.html

for (i <- 1 to 10) println(i)
来源：http://hz.yuanzhike.top/gtvxtjppim.html

[T60] Scala：折叠
来源：http://hz.cashguo.top/gtrhiclhoh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.zhengqikj.top/gtbrdeiwsr.html

================================================================================
来源：http://hz.hysaishi.cn/gtvfxnwfdc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.snrcjt.cn/gtamubgqig.html

================================================================================
来源：http://hz.guowangkeji.top/gtrfpciani.html

[U01] Py：创建虚拟环境
来源：http://hz.zhixingplan.top/gtppyqhnym.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.hywenlv.cn/gtqllgomph.html

[U02] Py：导出 / 安装依赖
来源：http://hz.ivvv.top/gtqyynzwmv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yj20258888.top/gtfpavctro.html

[U03] Py：加载 .env 配置
来源：http://hz.yj20258888.top/gtgyowzwre.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.havefunace.top/gtvkltydzz.html

[U04] Py：变量调试打印
来源：http://hz.shzxlz.cn/gtludezusg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.dianchejie.cn/gtbawrcxlb.html

[U05] Py：列表去重且保序
来源：http://hz.aizwys.cn/gtlcqzfvxx.html

list(dict.fromkeys(arr))
来源：http://hz.svipenyu.cn/gttqudrbje.html

[U06] Py：合并两个字典
来源：http://hz.daxiang520.top/gtsnxrhgjp.html

{**a, **b}
来源：http://hz.hywenlv.cn/gtrkrxusmx.html

[U07] Py：反转字典键值
来源：http://hz.dashuyun.cn/gtrrzqmegc.html

{v: k for k, v in d.items()}
来源：http://hz.0kj1m.cn/gtcookldgq.html

[U08] Py：展平二维列表
来源：http://hz.jyoumei.cn/gtpecibpks.html

[y for x in nested for y in x]
来源：http://hz.jiagoushi.top/gthffxbyzq.html

[U09] Py：字典取最大值的键
来源：http://hz.cucudq.cn/gtmvlohjbl.html

max(d, key=d.get)
来源：http://hz.ydzc1.top/gtfsgaokgh.html

[U10] Py：按值排序字典
来源：http://hz.52xcode.cn/gtusxzroto.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.hammf.cn/gtzudqkxfp.html

[U11] Py：生成器表达式
来源：http://hz.yj20258.top/gtcfmeuszp.html

(x * 2 for x in arr)
来源：http://hz.xuetiantiany.cn/gtilnwdtuh.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.havefunace.top/gtwwylxjop.html

Counter(arr).most_common(3)
来源：http://hz.andypj.xyz/gtaqqhjdbo.html

[U13] Py：固定长度队列
来源：http://hz.gzhubu.top/gtnrhgqmmi.html

deque(maxlen=10)
来源：http://hz.yueranfly.top/gtkutbjdcb.html

[U14] Py：分组收集到列表
来源：http://hz.jlsjyb.cn/gtqjhzmgdh.html

defaultdict(list)
来源：http://hz.cdnleiting.top/gtdthzcftn.html

[U15] Py：高精度计时
来源：http://hz.havefunace.top/gtrhxfbmka.html

t = time.perf_counter()
来源：http://hz.andypj.xyz/gtpdordtwr.html

[U16] Py：命令行参数解析
来源：http://hz.pengpengdd.cyou/gtlljpgrsg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jianghu66.top/gthhcyxcuh.html

[U17] Py：初始化日志
来源：http://hz.redwolf501.top/gtnypowdip.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yj20258888.top/gtcrhzqbcu.html

[U18] Py：预编译正则
来源：http://hz.birdmap.top/gtmxpgodac.html

pat = re.compile(r"\d+")
来源：http://hz.shuidangran.top/gtcckmzkqh.html

[U19] Py：正则替换带回调
来源：http://hz.gotoacloud.top/gttkuqonfe.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.jinyuanbaomall.cn/gtfjefbrpo.html

[U20] Py：缓存函数结果
来源：http://hz.wangdashe.top/gticcatido.html

@functools.lru_cache(maxsize=None)
来源：http://hz.daria6918.cn/gtqijyaaff.html

[U21] Py：自定义上下文管理器
来源：http://hz.feifeiyinyue.top/gtofpkxcav.html

@contextlib.contextmanager
来源：http://hz.hysaishi.cn/gtlenkenek.html

[U22] Py：矩阵转置
来源：http://hz.quarkkingdee.top/gtnjherhje.html

list(zip(*m))
来源：http://hz.yj20258.top/gtdnfduhym.html

[U23] Py：分块读取大文件
来源：http://hz.sysykeji.top/gtdjeujuuf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.shzxlz.cn/gtempxzmio.html

[U24] Py：路径操作
来源：http://hz.xuanzx.com/gtfyghftgg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.chenzaomai.com/gtafkewccv.html

[U25] Py：CSV 按字典读
来源：http://hz.feifeiyinyue.top/gtqwiujusy.html

csv.DictReader(f)
来源：http://hz.cheryme.top/gtkoynxwgz.html

[U26] Py：并发下载
来源：http://hz.nwbrower.top/gtdswhoqmt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.xinyue.icu/gtznzczgxn.html

[U27] Py：异步 HTTP
来源：http://hz.gaohongyu789.top/gtjfodnjvo.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.ybcxt.top/gthrxyryhy.html

[U28] Py：类型别名
来源：http://hz.quarkkingdee.top/gtpwpblzht.html

UserId = int
来源：http://hz.ivvv.top/gtefxtlqar.html

[U29] Py：属性校验
来源：http://hz.xingfuxueyuan.xyz/gtniqliszq.html

@property 与 @x.setter 配合
来源：http://hz.jiagoushi.top/gtxdbexztd.html

[U30] Py：数据类
来源：http://hz.nanxinkj.top/gtpaeewlms.html

@dataclass(slots=True)
来源：http://hz.pycfn.com/gtfvzqaaqi.html

[U31] Py：单测
来源：http://hz.guowangkeji.top/gtpepfqpba.html

python -m pytest -q
来源：http://hz.gotoacloud.top/gtuoplufkv.html

[U32] Py：代码格式化
来源：http://hz.yanxiufei.cn/gtuuuyzrvs.html

ruff format . && ruff check --fix .
来源：http://hz.daxiang520.top/gttkkxixoy.html

[U33] Py：打包发布
来源：http://hz.gogol.net.cn/gtdnofhipr.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.hongshengwenyu.top/gtczvufsag.html

[U34] Py：判断编码
来源：http://hz.cashguo.top/gtxiugmzge.html

chardet.detect(raw)
来源：http://hz.dianchejie.cn/gtqjttqwit.html

[U35] Py：发送邮件
来源：http://hz.fzhhl.top/gtgynabezg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.meibo888.top/gtqydbmahx.html

[U36] Py：定时任务
来源：http://hz.nanxuanxn.top/gthrxflpgd.html

schedule.every(10).minutes.do(job)
来源：http://hz.nanxinkj.top/gteybrozjk.html

[U37] Py：读写 Excel
来源：http://hz.iojbl.cn/gtwmkjpzpy.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.meibo888.top/gtdawrxpbj.html

[U38] Py：获取脚本所在目录
来源：http://hz.cdnleiting.top/gtptgxyopc.html

Path(__file__).resolve().parent
来源：http://hz.yueranfly.top/gtqjoswlah.html

[U39] Py：判断是否在交互环境
来源：http://hz.zhongyouzk.top/gtlcfncdnn.html

sys.stdout.isatty()
来源：http://hz.jqgufenzy.top/gttzulzjus.html

[U40] Py：打印到标准错误
来源：http://hz.tanke756.top/gtzlgwoziu.html

print("err", file=sys.stderr)
来源：http://hz.ydjk.org.cn/gtinnnrzhp.html


<!-- 参考信息 -->