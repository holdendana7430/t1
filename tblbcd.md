代发 wailian999

x |= (1 << 3);
来源：http://hz.iojbl.cn/gtbcvtppjp.html

[S17] C：安全拼接字符串
来源：http://hz.cqqwz.cn/gtmuogjozi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ppjwa.cn/gtackisqli.html

[S18] C：命令行参数
来源：http://hz.kuanghao11.cn/gthhihvcnu.html

int main(int argc, char **argv)
来源：http://hz.gotoacloud.top/gtmupkykaq.html

[S19] C：快速排序
来源：http://hz.aizwys.cn/gttfyksupz.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.snrcjt.cn/gttljqirab.html

[S20] C：二分查找
来源：http://hz.shangyingyoupin.top/gtnofpwmrz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yj20258888.top/gttjtgjfcx.html

[S21] C：字符类别判断
来源：http://hz.mhx1999.top/gtawndmlem.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ydzc1.top/gteeouzfbw.html

[S22] C：字符串转数字
来源：http://hz.ivvv.top/gtoupmxlfk.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.shzxlz.cn/gtqcaashgi.html

[S23] C：随机数
来源：http://hz.yuxming.cn/gtcncjwbxa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xziqi.cn/gttkwruuxm.html

[S24] C：获取本地时间
来源：http://hz.ydjk.org.cn/gtkofdudpd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.shzxlz.cn/gtgzqhtdsm.html

[S25] C：内存拷贝
来源：http://hz.chenjidiqi.icu/gtfrnnyeqs.html

memcpy(dst, src, n);
来源：http://hz.yuanzhike.top/gtjgyxcsvx.html

[S26] C：内存清零
来源：http://hz.ydzc1.top/gtfqnxnres.html

memset(a, 0, sizeof a);
来源：http://hz.tian-w.cn/gtmogthxwf.html

[S27] C：定义常量
来源：http://hz.9152youxi.cn/gtfvzncqpq.html

const double PI = 3.14159;
来源：http://hz.zhengqikj.top/gtlzpehazj.html

[S28] C：静态变量
来源：http://hz.daxiang520.top/gtibfnsovj.html

static int counter = 0;
来源：http://hz.yvedp.cn/gtnhrbeqzu.html

[S29] C：变参函数
来源：http://hz.chenjidiqi.icu/gtzklrfyax.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hnqzz.top/gthnrlmeet.html

[S30] C：头文件保护
来源：http://hz.aibaodan.cn/gtrjcvsdhi.html

#ifndef X_H
来源：http://hz.hnqzz.top/gtmdhifjxa.html

#define X_H
来源：http://hz.birdmap.top/gtlyebeedn.html

#endif
来源：http://hz.jianghu66.top/gtjwcbvnjq.html

[S31] C++：Hello World
来源：http://hz.shzxlz.cn/gthqlzbfaz.html

#include <iostream>
来源：http://hz.ydzc1.top/gtmovowlzk.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.sxryk.cn/gtrcadrvfb.html

[S32] C++：字符串
来源：http://hz.guowangkeji.top/gtopuuzolh.html

std::string s = "hi";  s += "!";
来源：http://hz.hfpthk.cn/gtlecrhfas.html

[S33] C++：vector 增删
来源：http://hz.fengsongda.top/gtvnjoyers.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.daxiang520.top/gtunykaeir.html

[S34] C++：遍历 vector
来源：http://hz.svipenyu.cn/gtrlzevcki.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.wangdashe.top/gtfahhykcq.html

[S35] C++：map
来源：http://hz.wangdashe.top/gtvmwgwmak.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.pycfn.com/gtymekubnv.html

[S36] C++：unordered_map
来源：http://hz.0kj1m.cn/gttxtqgsts.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yanxiufei.cn/gtldfhhxfj.html

[S37] C++：set
来源：http://hz.gzhubu.top/gtkhgivpxw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.guannengcc.top/gtpliivjkf.html

[S38] C++：排序
来源：http://hz.fengsongda.top/gtlcmkjbos.html

std::sort(v.begin(), v.end());
来源：http://hz.yj20258.top/gtojeycmjs.html

[S39] C++：自定义比较器排序
来源：http://hz.nwbrower.top/gtpzmduwuu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.fzhhl.top/gtxrsnfair.html

[S40] C++：查找元素
来源：http://hz.daria6918.cn/gtejvjuqgv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hywenlv.cn/gthzovcveh.html

[S41] C++：类与构造函数
来源：http://hz.hongshengwenyu.top/gtaafoscvs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xuetiantiany.cn/gtqrelyckm.html

[S42] C++：继承与虚函数
来源：http://hz.yj202588.top/gtxwyltfxr.html

class B : public Base { public: void f() override {} };
来源：http://hz.hnxiangtu.top/gtxrjsfvzl.html

[S43] C++：智能指针
来源：http://hz.zhaomingkeji.xyz/gtefolhdus.html

auto p = std::make_unique<int>(5);
来源：http://hz.hywenlv.cn/gtxebnaxeq.html

[S44] C++：引用传参
来源：http://hz.xingfuxueyuan.xyz/gtahhzopaa.html

void inc(int &x) { ++x; }
来源：http://hz.jqgufenzy.top/gtqfbuasav.html

[S45] C++：lambda
来源：http://hz.hongshengwenyu.top/gtoqczkdcz.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yuanzhike.top/gtnpietucp.html

[S46] C++：函数模板
来源：http://hz.yangfankeji.com/gtbtcxdowp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.hnxiangtu.top/gttpmnmcvb.html

[S47] C++：结构化绑定遍历
来源：http://hz.yonumen.top/gtkesodukc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.sysykeji.top/gtdmjpqnsq.html

[S48] C++：逐行读文件
来源：http://hz.zhengqikj.top/gtinzivwnm.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.sysykeji.top/gtjfonmtnf.html

while (std::getline(in, line)) { }
来源：http://hz.zhoulong.xyz/gtsougqzww.html

[S49] C++：写文件
来源：http://hz.yuxming.cn/gtrbiduovk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ydzc1.top/gtivyendsr.html

[S50] C++：格式化数字
来源：http://hz.gzhubu.top/gtgptasnaf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.0kj1m.cn/gtcntsccxh.html

[S51] C++：显式类型转换
来源：http://hz.bjfxy.top/gtdpnyadcr.html

static_cast<double>(a) / b
来源：http://hz.cqqwz.cn/gteekynnkb.html

[S52] C++：const 与 noexcept
来源：http://hz.zhoulong.xyz/gtlkbjzlae.html

int size() const noexcept { return n_; }
来源：http://hz.zycfv.cn/gtatgdvyio.html

[S53] C++：移动语义
来源：http://hz.cashguo.top/gtfxvkwnmr.html

std::vector<int> w = std::move(v);
来源：http://hz.ppjwa.cn/gtywjnrufu.html

[S54] C++：异常处理
来源：http://hz.zhongyouzk.top/gtqtudrljz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ybcxt.top/gtgzknemhi.html

[S55] C++：结构化绑定
来源：http://hz.yuxming.cn/gtzsolejkr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yvedp.cn/gtjlymqens.html

[S56] C++：optional
来源：http://hz.aibaodan.cn/gtlszjhiac.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhijiandao.cn/gtigeqlpgj.html

[S57] C++：编译期常量
来源：http://hz.zhongyouzk.top/gttmjcwigr.html

constexpr int N = 10;
来源：http://hz.zhongyouzk.top/gtffmjkoqc.html

[S58] C++：命名空间
来源：http://hz.zycfv.cn/gtmjmihppa.html

namespace ns { int f() { return 1; } }
来源：http://hz.yongpay.top/gtafmfjeks.html

[S59] C++：静态断言
来源：http://hz.mhx1999.top/gtpwabpocp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xinyue.icu/gtkodhluyl.html

[S60] C++：遍历并删除元素
来源：http://hz.gogol.net.cn/gtxtiflpml.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.snrcjt.cn/gtcyhbyrjd.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtkqntiwbb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yuxming.cn/gtauhxhwcs.html

================================================================================
来源：http://hz.cqqwz.cn/gtgfvczsqw.html

[T01] Kotlin：Hello World
来源：http://hz.chenjidiqi.icu/gtwftltbyh.html

println("Hello")
来源：http://hz.ydzc1.top/gttxxdkxnz.html

[T02] Kotlin：变量
来源：http://hz.jiagoushi.top/gttqlpgmxg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.52xcode.cn/gtqmzhhktd.html

[T03] Kotlin：字符串模板
来源：http://hz.haohaochexian.top/gtyicxvwdk.html

"值: $b"
来源：http://hz.yuanzhike.top/gtkharrnbp.html

[T04] Kotlin：空安全
来源：http://hz.shuidangran.top/gtbwkefyrn.html

val n: String? = null;  n?.length
来源：http://hz.nwbrower.top/gtsrzlamwd.html

[T05] Kotlin：when 表达式
来源：http://hz.yj20258.top/gtnfbwuhkk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.dashuyun.cn/gttcrqbvor.html

[T06] Kotlin：集合映射
来源：http://hz.wangshuangyany.cn/gtlkuquwlo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.gzhubu.top/gtjfwshxpr.html

[T07] Kotlin：集合过滤
来源：http://hz.xingfuxueyuan.xyz/gtblfzzzhf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.shanyushiyangkeji.top/gtoigtekyq.html

[T08] Kotlin：数据类
来源：http://hz.nwbrower.top/gtwcuhuncu.html

data class User(val name: String, val age: Int)
来源：http://hz.316326.xyz/gtimoqbbmp.html

[T09] Kotlin：扩展函数
来源：http://hz.jiagoushi.top/gthxsalpxr.html

fun String.exclaim() = this + "!"
来源：http://hz.dianchejie.cn/gtpypbrlhd.html

[T10] Kotlin：默认参数
来源：http://hz.tianlin.xyz/gtagwlcylx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zhongyouzk.top/gtchlhfhpk.html

[T11] Kotlin：协程
来源：http://hz.daria6918.cn/gteqloscyi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.0kj1m.cn/gtgyjdprww.html

[T12] Kotlin：解构声明
来源：http://hz.yangfankeji.com/gtfhzwtyui.html

val (a, b) = Pair(1, 2)
来源：http://hz.shanyushiyangkeji.top/gtkfakaqjo.html

[T13] Kotlin：只读 Map
来源：http://hz.wangshuangyany.cn/gtomimophy.html

val m = mapOf("a" to 1)
来源：http://hz.smart0.xyz/gtyxnocpis.html

[T14] Kotlin：循环
来源：http://hz.wangdashe.top/gtrkmpyxqq.html

for (i in 1..10) println(i)
来源：http://hz.zhoulong.xyz/gtnqjirutp.html

[T15] Kotlin：接口
来源：http://hz.meibo888.top/gtyvdeayep.html

interface Shape { fun area(): Double }
来源：http://hz.feifeiyinyue.top/gtohfmlgal.html

[T16] Swift：Hello World
来源：http://hz.smart0.xyz/gtkwpneoeq.html

print("Hello")
来源：http://hz.pycfn.com/gtgtuncuzd.html

[T17] Swift：变量与常量
来源：http://hz.hysaishi.cn/gtyyefmcbx.html

var a = 1;  let b = 2
来源：http://hz.cdnleiting.top/gtjlqvrocd.html

[T18] Swift：字符串插值
来源：http://hz.smart0.xyz/gtpjwhgzkc.html

"值: \(b)"
来源：http://hz.nanxuanxn.top/gtldmwqyqd.html

[T19] Swift：可选绑定
来源：http://hz.daria6918.cn/gtkmwlcaed.html

if let n = opt { print(n) }
来源：http://hz.gogol.net.cn/gtnswllaxq.html

[T20] Swift：数组操作
来源：http://hz.haohaochexian.top/gtjpaowmrq.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.9152youxi.cn/gteospsqzk.html

[T21] Swift：遍历
来源：http://hz.c1oappe.top/gtvwvogyac.html

for x in a { print(x) }
来源：http://hz.xylfe.cn/gtdojwtook.html

[T22] Swift：字典
来源：http://hz.zhixingplan.top/gtmclxargp.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.gogol.net.cn/gtbzmuwhem.html

[T23] Swift：函数
来源：http://hz.zhijiandao.cn/gtbnbunlon.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.guowangkeji.top/gtofrpfrik.html

[T24] Swift：闭包
来源：http://hz.hammf.cn/gtkcvaclca.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.sysykeji.top/gtospgvgwf.html

[T25] Swift：结构体
来源：http://hz.hnqzz.top/gtrycsmdjj.html

struct P { var x: Int }
来源：http://hz.jyoumei.cn/gtctxpnqna.html

[T26] Swift：类与重写
来源：http://hz.sweek.top/gtydldynin.html

class A: Base { override func f() {} }
来源：http://hz.aizwys.cn/gtvqsnwyhl.html

[T27] Swift：错误处理
来源：http://hz.ydjk.org.cn/gtthwnhfrq.html

do { try f() } catch { print(error) }
来源：http://hz.jqgfzy.top/gtksfochgm.html

[T28] Swift：枚举
来源：http://hz.fzhhl.top/gtgdwwvbra.html

enum Color { case red, green }
来源：http://hz.hysaishi.cn/gthlshiwzo.html

[T29] Swift：guard 提前返回
来源：http://hz.dashuyun.cn/gtsasluztz.html

guard let x = opt else { return }
来源：http://hz.ehwqpu.com/gtcqtclxad.html

[T30] Swift：协议
来源：http://hz.yj20258888.top/gthpjynwbv.html

protocol Shape { func area() -> Double }
来源：http://hz.tian-w.cn/gtkjlmnfai.html

[T31] Lua：Hello World
来源：http://hz.jinqigufen.top/gtcbvqsnxb.html

print("Hello")
来源：http://hz.pengpengdd.cyou/gtqbnfqjfk.html

[T32] Lua：局部变量
来源：http://hz.nwbrower.top/gtocwiodfd.html

local a = 1
来源：http://hz.yanxiufei.cn/gtumtplors.html

[T33] Lua：表（数组）
来源：http://hz.jqgfzy.top/gtwbnqgxdx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jianghu66.top/gthzrefkas.html

[T34] Lua：遍历表
来源：http://hz.zhaomingkeji.xyz/gtjinpauxl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.hammf.cn/gtizcprkgg.html

[T35] Lua：字典表
来源：http://hz.ybcxt.top/gtcnyrqosf.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jinyuanbaomall.cn/gtpzaiqutn.html

[T36] Lua：函数
来源：http://hz.yongpay.top/gteykqhkxx.html

function add(a, b) return a + b end
来源：http://hz.hfpthk.cn/gtflquvmyp.html

[T37] Lua：字符串拼接
来源：http://hz.jlsjyb.cn/gtykssmrwy.html

"a" .. "b"
来源：http://hz.daxiang520.top/gtuixpeqks.html

[T38] Lua：条件
来源：http://hz.svipenyu.cn/gtggsmhnri.html

if x > 0 then print("正") end
来源：http://hz.haohaochexian.top/gttozegmfn.html

[T39] Lua：模式匹配
来源：http://hz.tianlin.xyz/gtsyyhxmnl.html

string.find(s, "%d+")
来源：http://hz.hnqzz.top/gtbtcoqzut.html

[T40] Lua：元表
来源：http://hz.svipenyu.cn/gtyyicpdne.html

setmetatable({}, { __index = base })
来源：http://hz.shangyingyoupin.top/gtvuazpaqd.html

[T41] Perl：Hello World
来源：http://hz.yj202588.top/gtvyvdaqka.html

print "Hello\n";
来源：http://hz.jianghu66.top/gtdptngxhh.html

[T42] Perl：变量类型
来源：http://hz.jinqigfzy.top/gtuxmpelrh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.nanxuanxn.top/gtvckxdbqy.html

[T43] Perl：字符串插值
来源：http://hz.havefunace.top/gtjjogbwij.html

"值: $a"
来源：http://hz.nwbrower.top/gtnmjgufnm.html

[T44] Perl：条件
来源：http://hz.chenjidiqi.icu/gtskpyvwax.html

if ($a > 0) { print "正"; }
来源：http://hz.yonumen.top/gtifkfplhb.html

[T45] Perl：数组遍历
来源：http://hz.jqgufenzy.top/gthxxwsmyf.html

for my $x (@arr) { print $x; }
来源：http://hz.xziqi.cn/gtrxjtaxla.html

[T46] Perl：哈希操作
来源：http://hz.ivvv.top/gtzwquioao.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.hammf.cn/gtnutlixnj.html

[T47] Perl：正则捕获
来源：http://hz.pycfn.com/gtprsprezy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.zhengqikj.top/gtxlaomibm.html

[T48] Perl：正则替换
来源：http://hz.jiagoushi.top/gtqdlwdjnt.html

$s =~ s/old/new/g;
来源：http://hz.cashguo.top/gtxaacjbzk.html

[T49] Perl：函数
来源：http://hz.zhixingplan.top/gtuzjgvbav.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jinqigfzy.top/gtpdlittkw.html

[T50] Perl：逐行读文件
来源：http://hz.hammf.cn/gtpszwvlwb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.ybcxt.top/gtyrfzflro.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.cashguo.top/gtcauzuuro.html

[T51] Scala：Hello World
来源：http://hz.cashguo.top/gtizwtbiev.html

println("Hello")
来源：http://hz.ydzc1.top/gtnchuzqma.html

[T52] Scala：变量
来源：http://hz.hnqzz.top/gtanajvjnf.html

val a = 1;  var b = 2
来源：http://hz.cdnleiting.top/gtvdkgqmqr.html

[T53] Scala：字符串插值
来源：http://hz.jyoumei.cn/gthwjszhsb.html

s"值: $b"
来源：http://hz.sxryk.cn/gtcfywzuwf.html

[T54] Scala：集合映射
来源：http://hz.daxiang520.top/gtrvehujzn.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.hfpthk.cn/gtdrzhnclw.html

[T55] Scala：集合过滤
来源：http://hz.ehwqpu.com/gtdrxrpjax.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jinqigufen.top/gtvxtjmaam.html

[T56] Scala：样例类
来源：http://hz.gogol.net.cn/gtxlexuufr.html

case class User(name: String, age: Int)
来源：http://hz.c1oappe.top/gtkmpnhlta.html

[T57] Scala：模式匹配
来源：http://hz.meibo888.top/gtltzayyvt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.jianghu66.top/gthkftnqkz.html

[T58] Scala：函数定义
来源：http://hz.vqdsnc.cn/gtkbqguwhx.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zycfv.cn/gtatgufqbg.html

[T59] Scala：循环
来源：http://hz.xuetiantiany.cn/gtzjcdbfbo.html

for (i <- 1 to 10) println(i)
来源：http://hz.svipenyu.cn/gtscrtndqq.html

[T60] Scala：折叠
来源：http://hz.ybcxt.top/gtyskcjmpi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.ydzc1.top/gtudbhjmmy.html

================================================================================
来源：http://hz.nanxuanxn.top/gtgmasbujl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jqgufenzy.top/gtleocujhx.html

================================================================================
来源：http://hz.sufxvd.cn/gtfahjokyj.html

[U01] Py：创建虚拟环境
来源：http://hz.feifeiyinyue.top/gtfuyiyzjj.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.shanyushiyangtech.top/gtpckfhkwl.html

[U02] Py：导出 / 安装依赖
来源：http://hz.havefunace.top/gtfouhdgss.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.pycfn.com/gttqjpcepc.html

[U03] Py：加载 .env 配置
来源：http://hz.wangshuangyany.cn/gtcdevwten.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.quarkkingdee.top/gtkewyoqad.html

[U04] Py：变量调试打印
来源：http://hz.ywan-chungtsiang.top/gtgwitzfvx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.gzhubu.top/gtoonmfoyp.html

[U05] Py：列表去重且保序
来源：http://hz.shanyushiyangtech.top/gthexqklqg.html

list(dict.fromkeys(arr))
来源：http://hz.redwolf501.top/gtyxxmsqez.html

[U06] Py：合并两个字典
来源：http://hz.xylfe.cn/gtacqoylxp.html

{**a, **b}
来源：http://hz.jinghuilouyu.cn/gtvducdafz.html

[U07] Py：反转字典键值
来源：http://hz.shanyushiyangtech.top/gtefromrpl.html

{v: k for k, v in d.items()}
来源：http://hz.jyoumei.cn/gtyzdmoakl.html

[U08] Py：展平二维列表
来源：http://hz.cheryme.top/gtskswnbwn.html

[y for x in nested for y in x]
来源：http://hz.ybcxt.top/gtzufugbtz.html

[U09] Py：字典取最大值的键
来源：http://hz.9152youxi.cn/gtlspawniy.html

max(d, key=d.get)
来源：http://hz.yj202588.top/gtnknqkhca.html

[U10] Py：按值排序字典
来源：http://hz.yj20258.top/gtahiiqvjs.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.shangyingyoupin.top/gtvfuveelr.html

[U11] Py：生成器表达式
来源：http://hz.zhixingplan.top/gtzfihfrjw.html

(x * 2 for x in arr)
来源：http://hz.hywenlv.cn/gtqthrkyqi.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.chenzaomai.com/gtlkqcjwyp.html

Counter(arr).most_common(3)
来源：http://hz.chenlongwang.top/gttawmidcy.html

[U13] Py：固定长度队列
来源：http://hz.yonumen.top/gtpchwshji.html

deque(maxlen=10)
来源：http://hz.yanxiufei.cn/gtspshsmqh.html

[U14] Py：分组收集到列表
来源：http://hz.9152youxi.cn/gthgfphooe.html

defaultdict(list)
来源：http://hz.guannengcc.top/gtxhcxdiir.html

[U15] Py：高精度计时
来源：http://hz.zhoulong.xyz/gtkbljozit.html

t = time.perf_counter()
来源：http://hz.havefunace.top/gtletlrrja.html

[U16] Py：命令行参数解析
来源：http://hz.gogol.net.cn/gttnnhdjal.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.cqqwz.cn/gtqidqqyuo.html

[U17] Py：初始化日志
来源：http://hz.daxiang520.top/gtxhjrryst.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yj20258888.top/gtditzzfla.html

[U18] Py：预编译正则
来源：http://hz.jlsjyb.cn/gtqikyvdob.html

pat = re.compile(r"\d+")
来源：http://hz.guowangkeji.top/gttmxucwxp.html

[U19] Py：正则替换带回调
来源：http://hz.shzxlz.cn/gtebawivze.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.zhoulong.xyz/gtxmxtnxtp.html

[U20] Py：缓存函数结果
来源：http://hz.gogol.net.cn/gtywfgictq.html

@functools.lru_cache(maxsize=None)
来源：http://hz.meibo888.top/gtmltzchqp.html

[U21] Py：自定义上下文管理器
来源：http://hz.jinghuilouyu.cn/gtdqjecjyp.html

@contextlib.contextmanager
来源：http://hz.shangyingyoupin.top/gtptaizmeh.html

[U22] Py：矩阵转置
来源：http://hz.shanyushiyangkeji.top/gtxvrctqrb.html

list(zip(*m))
来源：http://hz.guannengcc.top/gtatjuhyaf.html

[U23] Py：分块读取大文件
来源：http://hz.guowangkeji.top/gthxcrtmxa.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.daxiang520.top/gtneqcxnoj.html

[U24] Py：路径操作
来源：http://hz.sufxvd.cn/gtvhucnxro.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.gzhubu.top/gtsayutktw.html

[U25] Py：CSV 按字典读
来源：http://hz.cdnleiting.top/gtogiusvha.html

csv.DictReader(f)
来源：http://hz.yueranfly.top/gthkzfxbic.html

[U26] Py：并发下载
来源：http://hz.chenjidiqi.icu/gtnmcwwbvj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.shangyingyoupin.top/gtykwyspqk.html

[U27] Py：异步 HTTP
来源：http://hz.daria6918.cn/gtyncofqnq.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.dianchejie.cn/gtfbozlkpj.html

[U28] Py：类型别名
来源：http://hz.jqgufenzy.top/gtnhflvcbd.html

UserId = int
来源：http://hz.hnxiangtu.top/gtlsprnodi.html

[U29] Py：属性校验
来源：http://hz.yonumen.top/gtimbgtnrl.html

@property 与 @x.setter 配合
来源：http://hz.gogol.net.cn/gthhdhwzwd.html

[U30] Py：数据类
来源：http://hz.yuanzhike.top/gtsxhacshl.html

@dataclass(slots=True)
来源：http://hz.sufxvd.cn/gtbsraxhhl.html

[U31] Py：单测
来源：http://hz.snrcjt.cn/gtxxgplici.html

python -m pytest -q
来源：http://hz.redwolf501.top/gtemqhzbed.html

[U32] Py：代码格式化
来源：http://hz.fzhhl.top/gtdhrdrouu.html

ruff format . && ruff check --fix .
来源：http://hz.iojbl.cn/gtheuqgcwf.html

[U33] Py：打包发布
来源：http://hz.316326.xyz/gtypmomtpj.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.guowangkeji.top/gtngozcrje.html

[U34] Py：判断编码
来源：http://hz.xinyue.icu/gtanboetqh.html

chardet.detect(raw)
来源：http://hz.chenjidiqi.icu/gtspihjggd.html

[U35] Py：发送邮件
来源：http://hz.fengsongda.top/gtefwtqbku.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.shanyushiyangtech.top/gtffktacvn.html

[U36] Py：定时任务
来源：http://hz.jinyuanbaomall.cn/gtdolmsroi.html

schedule.every(10).minutes.do(job)
来源：http://hz.yanxiufei.cn/gttfppzuhn.html

[U37] Py：读写 Excel
来源：http://hz.iojbl.cn/gtulzyoiso.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.shangyingyoupin.top/gtouuizyls.html

[U38] Py：获取脚本所在目录
来源：http://hz.hammf.cn/gtocwxwdvu.html

Path(__file__).resolve().parent
来源：http://hz.jyoumei.cn/gtdewpxkun.html

[U39] Py：判断是否在交互环境
来源：http://hz.fengsongda.top/gtovnnxlbc.html

sys.stdout.isatty()
来源：http://hz.meibo888.top/gtlreupllg.html

[U40] Py：打印到标准错误
来源：http://hz.cheryme.top/gtjadrtpml.html

print("err", file=sys.stderr)
来源：http://hz.jinghuilouyu.cn/gtdibomibh.html


<!-- 参考信息 -->