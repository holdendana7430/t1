代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://hz.jinyuanbaomall.cn/gtexyihjvt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jyoumei.cn/gtcgvztett.html

fclose(f);
来源：http://hz.nwbrower.top/gtgykhbpsw.html

[S12] C：写文件
来源：http://hz.xuetiantiany.cn/gtzadfmbyy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zhixingplan.top/gtzxjjnkat.html

[S13] C：宏定义
来源：http://hz.0kj1m.cn/gthlrqyeva.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.sxryk.cn/gtztimlewn.html

[S14] C：枚举
来源：http://hz.ivvv.top/gtrrmhimrm.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jinyuanbaomall.cn/gtsfjpijis.html

[S15] C：类型转换
来源：http://hz.c1oappe.top/gtgkcgnqur.html

(double) a / b
来源：http://hz.redwolf501.top/gtwatgozfe.html

[S16] C：位操作置位
来源：http://hz.wangshuangyany.cn/gtgpqbeiuf.html

x |= (1 << 3);
来源：http://hz.hnqzz.top/gtbcfwkxak.html

[S17] C：安全拼接字符串
来源：http://hz.xylfe.cn/gtihphuszx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.feifeiyinyue.top/gtzedvhdnf.html

[S18] C：命令行参数
来源：http://hz.sysykeji.top/gtifqfdmdd.html

int main(int argc, char **argv)
来源：http://hz.dashuyun.cn/gtmmdjlpnh.html

[S19] C：快速排序
来源：http://hz.redwolf501.top/gtreamezoz.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.ywan-chungtsiang.top/gtaoowgpqr.html

[S20] C：二分查找
来源：http://hz.sweek.top/gtbfoakgcq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.tianlin.xyz/gtcocgbhxe.html

[S21] C：字符类别判断
来源：http://hz.pycfn.com/gtcbgpfmsu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zhongyouzk.top/gtjwuwkjbd.html

[S22] C：字符串转数字
来源：http://hz.guowangkeji.top/gtgtlcwkig.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.fengsongda.top/gthrkjisaa.html

[S23] C：随机数
来源：http://hz.smart0.xyz/gtseaxukyp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jinyuanbaomall.cn/gtpugmrzez.html

[S24] C：获取本地时间
来源：http://hz.svipenyu.cn/gtqcdiywbo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ywan-chungtsiang.top/gtzwdwsemu.html

[S25] C：内存拷贝
来源：http://hz.zhixingplan.top/gtlsigoyrl.html

memcpy(dst, src, n);
来源：http://hz.gotoacloud.top/gtzeolhgox.html

[S26] C：内存清零
来源：http://hz.quarkkingdee.top/gtrqanfesp.html

memset(a, 0, sizeof a);
来源：http://hz.tianlin.xyz/gtdaaymxar.html

[S27] C：定义常量
来源：http://hz.52xcode.cn/gtldeefuyc.html

const double PI = 3.14159;
来源：http://hz.yangfankeji.com/gtxeewnfqs.html

[S28] C：静态变量
来源：http://hz.aizwys.cn/gtzoiobivj.html

static int counter = 0;
来源：http://hz.yanxiufei.cn/gtappodzvx.html

[S29] C：变参函数
来源：http://hz.ybcxt.top/gtbfvnsfmh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.sufxvd.cn/gtxxdyqmct.html

[S30] C：头文件保护
来源：http://hz.zhiwuduotai.top/gthdntohny.html

#ifndef X_H
来源：http://hz.chenzaomai.com/gtzynbjyso.html

#define X_H
来源：http://hz.xylfe.cn/gtuqifojqj.html

#endif
来源：http://hz.cashguo.top/gtbiwuwvwl.html

[S31] C++：Hello World
来源：http://hz.ehwqpu.com/gtuatjqwtp.html

#include <iostream>
来源：http://hz.wangshuangyany.cn/gtantgcxol.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zhaomingkeji.xyz/gtrdnbcxgc.html

[S32] C++：字符串
来源：http://hz.svipenyu.cn/gtubdilnvo.html

std::string s = "hi";  s += "!";
来源：http://hz.wangshuangyany.cn/gtrmgucwel.html

[S33] C++：vector 增删
来源：http://hz.ydjk.org.cn/gtqpwtupaw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.9152youxi.cn/gtrpkqgczy.html

[S34] C++：遍历 vector
来源：http://hz.yj20258.top/gtichmtacn.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.chenlongwang.top/gtvmyogckw.html

[S35] C++：map
来源：http://hz.iojbl.cn/gtzjwxdaxz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hysaishi.cn/gtfucsylyl.html

[S36] C++：unordered_map
来源：http://hz.snrcjt.cn/gtwcvsqbcw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.0kj1m.cn/gtdfbjvige.html

[S37] C++：set
来源：http://hz.jyoumei.cn/gtulduwdot.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ehwqpu.com/gtfmvxzslj.html

[S38] C++：排序
来源：http://hz.svipenyu.cn/gtcnvibwrg.html

std::sort(v.begin(), v.end());
来源：http://hz.cdnleiting.top/gtwclgqeqe.html

[S39] C++：自定义比较器排序
来源：http://hz.9152youxi.cn/gtzmsyewhb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hnxiangtu.top/gthpxxbdst.html

[S40] C++：查找元素
来源：http://hz.c1oappe.top/gtrlfyjupt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jinghuilouyu.cn/gtptbinzsu.html

[S41] C++：类与构造函数
来源：http://hz.jqgfzy.top/gtabgxkpjs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ivvv.top/gtqfkknxly.html

[S42] C++：继承与虚函数
来源：http://hz.xingfuxueyuan.xyz/gtkeqghngv.html

class B : public Base { public: void f() override {} };
来源：http://hz.yangfankeji.com/gtrergdwqo.html

[S43] C++：智能指针
来源：http://hz.jianghu66.top/gtjifrnxfv.html

auto p = std::make_unique<int>(5);
来源：http://hz.yj20258.top/gtdcrqrktc.html

[S44] C++：引用传参
来源：http://hz.tian-w.cn/gtnqxscosj.html

void inc(int &x) { ++x; }
来源：http://hz.fengsongda.top/gtjtmkqmot.html

[S45] C++：lambda
来源：http://hz.dianchejie.cn/gtsryilnyw.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.pengpengdd.cyou/gtgexrfnqh.html

[S46] C++：函数模板
来源：http://hz.jianghu66.top/gtdsxqvbah.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhoulong.xyz/gtlazqhztp.html

[S47] C++：结构化绑定遍历
来源：http://hz.xinyue.icu/gtvhpksrcp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.0kj1m.cn/gtgortbpix.html

[S48] C++：逐行读文件
来源：http://hz.mhx1999.top/gtckevfyio.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.hywenlv.cn/gtvzidwzqy.html

while (std::getline(in, line)) { }
来源：http://hz.wangshuangyany.cn/gtqnpdmnzo.html

[S49] C++：写文件
来源：http://hz.chenlongwang.top/gtlziwhgmb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.iojbl.cn/gtjdjprcth.html

[S50] C++：格式化数字
来源：http://hz.yj202588.top/gttihcpaaq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.feifeiyinyue.top/gtgadmshow.html

[S51] C++：显式类型转换
来源：http://hz.havefunace.top/gtmoekvxqn.html

static_cast<double>(a) / b
来源：http://hz.zhiwuduotai.top/gtbzjwhmhj.html

[S52] C++：const 与 noexcept
来源：http://hz.yj20258.top/gtsnrswehp.html

int size() const noexcept { return n_; }
来源：http://hz.xuetiantiany.cn/gtyytuvghb.html

[S53] C++：移动语义
来源：http://hz.pengpengdd.cyou/gtjmcmdkic.html

std::vector<int> w = std::move(v);
来源：http://hz.xuetiantiany.cn/gtiwandgrz.html

[S54] C++：异常处理
来源：http://hz.sysykeji.top/gtpncowqom.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.feifeiyinyue.top/gtumufxzzn.html

[S55] C++：结构化绑定
来源：http://hz.yonumen.top/gtwvwwggil.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhixingplan.top/gtjjyvqrlr.html

[S56] C++：optional
来源：http://hz.ppjwa.cn/gtzfzqkmme.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.chenzaomai.com/gtakeahkwj.html

[S57] C++：编译期常量
来源：http://hz.kuanghao11.cn/gtzfrcemde.html

constexpr int N = 10;
来源：http://hz.fengsongda.top/gtsoyeuwsw.html

[S58] C++：命名空间
来源：http://hz.xuanzx.com/gtxzxhdirq.html

namespace ns { int f() { return 1; } }
来源：http://hz.redwolf501.top/gtmkyernon.html

[S59] C++：静态断言
来源：http://hz.yuanzhike.top/gtofzrzjgo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.cheryme.top/gtqhkvibce.html

[S60] C++：遍历并删除元素
来源：http://hz.hongshengwenyu.top/gtkyoxeuwr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.shanyushiyangkeji.top/gthhumghyu.html

================================================================================
来源：http://hz.yanxiufei.cn/gtxjqvstxv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.aibaodan.cn/gtagbnxvzr.html

================================================================================
来源：http://hz.zhixingplan.top/gtpbpouhru.html

[T01] Kotlin：Hello World
来源：http://hz.svipenyu.cn/gtpdglsfgh.html

println("Hello")
来源：http://hz.nanxuanxn.top/gthmmgxtof.html

[T02] Kotlin：变量
来源：http://hz.snrcjt.cn/gtkyowgzls.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhongyouzk.top/gtekylbmin.html

[T03] Kotlin：字符串模板
来源：http://hz.zdqjudy.top/gtyuachhto.html

"值: $b"
来源：http://hz.hongshengwenyu.top/gtxsnrfnsr.html

[T04] Kotlin：空安全
来源：http://hz.vqdsnc.cn/gtynsbmgdv.html

val n: String? = null;  n?.length
来源：http://hz.iojbl.cn/gteqqqsfep.html

[T05] Kotlin：when 表达式
来源：http://hz.xuanzx.com/gtdiozunax.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.guowangkeji.top/gtztnwrlec.html

[T06] Kotlin：集合映射
来源：http://hz.hongshengwenyu.top/gtmxjkfwsc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.tianlin.xyz/gteiwxqtie.html

[T07] Kotlin：集合过滤
来源：http://hz.cheryme.top/gtlakvgbdn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.cheryme.top/gtxowhswpd.html

[T08] Kotlin：数据类
来源：http://hz.daxiang520.top/gtdmgsnjig.html

data class User(val name: String, val age: Int)
来源：http://hz.jianghu66.top/gttpsnijth.html

[T09] Kotlin：扩展函数
来源：http://hz.hywenlv.cn/gtzgfdbysu.html

fun String.exclaim() = this + "!"
来源：http://hz.dashuyun.cn/gtwwwqaowp.html

[T10] Kotlin：默认参数
来源：http://hz.zhijiandao.cn/gtvjhacser.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zycfv.cn/gtqvwovvkj.html

[T11] Kotlin：协程
来源：http://hz.cheryme.top/gtraeidxry.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.ywan-chungtsiang.top/gtdugxxwhf.html

[T12] Kotlin：解构声明
来源：http://hz.gogol.net.cn/gtlpkjysov.html

val (a, b) = Pair(1, 2)
来源：http://hz.zhoulong.xyz/gtekyzhszl.html

[T13] Kotlin：只读 Map
来源：http://hz.9152youxi.cn/gtqetmayay.html

val m = mapOf("a" to 1)
来源：http://hz.dianchejie.cn/gtuhvudowf.html

[T14] Kotlin：循环
来源：http://hz.ybcxt.top/gtmcbhgsbj.html

for (i in 1..10) println(i)
来源：http://hz.gaohongyu789.top/gtzaiihkqa.html

[T15] Kotlin：接口
来源：http://hz.sufxvd.cn/gthjvzualm.html

interface Shape { fun area(): Double }
来源：http://hz.ydzc1.top/gtawfraoek.html

[T16] Swift：Hello World
来源：http://hz.yongpay.top/gttrtnjlpa.html

print("Hello")
来源：http://hz.yj20258.top/gtejewhhnh.html

[T17] Swift：变量与常量
来源：http://hz.ydzc1.top/gtxduwgepi.html

var a = 1;  let b = 2
来源：http://hz.nanxuanxn.top/gtgjzpochs.html

[T18] Swift：字符串插值
来源：http://hz.shzxlz.cn/gtvuvpjrye.html

"值: \(b)"
来源：http://hz.pengpengdd.cyou/gtnqqmdkmz.html

[T19] Swift：可选绑定
来源：http://hz.hongshengwenyu.top/gtbkosixbe.html

if let n = opt { print(n) }
来源：http://hz.ppjwa.cn/gtllybaowq.html

[T20] Swift：数组操作
来源：http://hz.hnqzz.top/gtacjgekof.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.9152youxi.cn/gtwndwhlxp.html

[T21] Swift：遍历
来源：http://hz.dianchejie.cn/gtomuzsguv.html

for x in a { print(x) }
来源：http://hz.ydjk.org.cn/gtqmapboha.html

[T22] Swift：字典
来源：http://hz.tian-w.cn/gtfseifuyi.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.fengsongda.top/gtonlmdxhc.html

[T23] Swift：函数
来源：http://hz.xylfe.cn/gtksuaohpt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ywan-chungtsiang.top/gtmuixpnkb.html

[T24] Swift：闭包
来源：http://hz.jiagoushi.top/gtmoihvuav.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.gotoacloud.top/gtpavpxwte.html

[T25] Swift：结构体
来源：http://hz.pycfn.com/gtberagyqc.html

struct P { var x: Int }
来源：http://hz.chenzaomai.com/gtcprzrgsk.html

[T26] Swift：类与重写
来源：http://hz.ydzc1.top/gtunotjkrm.html

class A: Base { override func f() {} }
来源：http://hz.jinqigfzy.top/gtaimdnkmc.html

[T27] Swift：错误处理
来源：http://hz.daria6918.cn/gtxqdxsvvx.html

do { try f() } catch { print(error) }
来源：http://hz.yj20258888.top/gtynlfrdbm.html

[T28] Swift：枚举
来源：http://hz.shzxlz.cn/gtpnqljvza.html

enum Color { case red, green }
来源：http://hz.jqgfzy.top/gtuyhvjnqh.html

[T29] Swift：guard 提前返回
来源：http://hz.guannengcc.top/gtdnbfjzox.html

guard let x = opt else { return }
来源：http://hz.redwolf501.top/gtzszywtjt.html

[T30] Swift：协议
来源：http://hz.zycfv.cn/gtggpbzemt.html

protocol Shape { func area() -> Double }
来源：http://hz.yongpay.top/gtbhfgepjw.html

[T31] Lua：Hello World
来源：http://hz.hywenlv.cn/gtaytgydyq.html

print("Hello")
来源：http://hz.ehwqpu.com/gtpscuvtyu.html

[T32] Lua：局部变量
来源：http://hz.iojbl.cn/gtihgwajmr.html

local a = 1
来源：http://hz.sxryk.cn/gthapltypo.html

[T33] Lua：表（数组）
来源：http://hz.andypj.xyz/gtnyuzncrr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.shuidangran.top/gtiuilzyvl.html

[T34] Lua：遍历表
来源：http://hz.cheryme.top/gtmdtmvlkl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.cheryme.top/gtwbyribxf.html

[T35] Lua：字典表
来源：http://hz.ivvv.top/gtkpbqsnvw.html

local d = { a = 1 };  d.b = 2
来源：http://hz.zycfv.cn/gtroskmzpd.html

[T36] Lua：函数
来源：http://hz.daria6918.cn/gtwppqpvsi.html

function add(a, b) return a + b end
来源：http://hz.andypj.xyz/gtbclueicg.html

[T37] Lua：字符串拼接
来源：http://hz.xylfe.cn/gtbdjxwmrn.html

"a" .. "b"
来源：http://hz.xingfuxueyuan.xyz/gtxquryuyl.html

[T38] Lua：条件
来源：http://hz.zhengqikj.top/gtywmycvxh.html

if x > 0 then print("正") end
来源：http://hz.zdqjudy.top/gtqrcuzyvh.html

[T39] Lua：模式匹配
来源：http://hz.chenjidiqi.icu/gtjydtyqqq.html

string.find(s, "%d+")
来源：http://hz.chenlongwang.top/gtumcdizwr.html

[T40] Lua：元表
来源：http://hz.svipenyu.cn/gtjwgclwlj.html

setmetatable({}, { __index = base })
来源：http://hz.zdqjudy.top/gtghyqkmqg.html

[T41] Perl：Hello World
来源：http://hz.pengpengdd.cyou/gtrztvkslh.html

print "Hello\n";
来源：http://hz.jianghu66.top/gtzymkuqxk.html

[T42] Perl：变量类型
来源：http://hz.daxiang520.top/gtbeustovx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.sxryk.cn/gtrfxddary.html

[T43] Perl：字符串插值
来源：http://hz.ywan-chungtsiang.top/gtesfpkeuo.html

"值: $a"
来源：http://hz.ppjwa.cn/gtonxkzity.html

[T44] Perl：条件
来源：http://hz.sxryk.cn/gtxwumlsnx.html

if ($a > 0) { print "正"; }
来源：http://hz.xylfe.cn/gtikvvulan.html

[T45] Perl：数组遍历
来源：http://hz.zycfv.cn/gtlnntzjyw.html

for my $x (@arr) { print $x; }
来源：http://hz.andypj.xyz/gtplvdxdcl.html

[T46] Perl：哈希操作
来源：http://hz.zhoulong.xyz/gtrchtuyaa.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.316326.xyz/gtqpogqtvv.html

[T47] Perl：正则捕获
来源：http://hz.zdqjudy.top/gtrripjljg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jinqigfzy.top/gtncvxbbnp.html

[T48] Perl：正则替换
来源：http://hz.shangyingyoupin.top/gtiwvsynpz.html

$s =~ s/old/new/g;
来源：http://hz.kuanghao11.cn/gtzvhzswqn.html

[T49] Perl：函数
来源：http://hz.ppjwa.cn/gtywywkafn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zhongyouzk.top/gtgmmcrlfl.html

[T50] Perl：逐行读文件
来源：http://hz.shanyushiyangkeji.top/gtvribmmbj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jianghu66.top/gtihrbwufy.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.aizwys.cn/gtmuoqprlg.html

[T51] Scala：Hello World
来源：http://hz.chenlongwang.top/gtibolkmaa.html

println("Hello")
来源：http://hz.cucudq.cn/gttlerwduh.html

[T52] Scala：变量
来源：http://hz.9152youxi.cn/gttbcwklcl.html

val a = 1;  var b = 2
来源：http://hz.0kj1m.cn/gtmaskcjxm.html

[T53] Scala：字符串插值
来源：http://hz.xziqi.cn/gtqeznorny.html

s"值: $b"
来源：http://hz.jyoumei.cn/gtlabyjpja.html

[T54] Scala：集合映射
来源：http://hz.pengpengdd.cyou/gtxrewwzyz.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yj202588.top/gthbgahutf.html

[T55] Scala：集合过滤
来源：http://hz.52xcode.cn/gtmilabnrw.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.hongshengwenyu.top/gtgqeixixd.html

[T56] Scala：样例类
来源：http://hz.fengsongda.top/gtaccnuefw.html

case class User(name: String, age: Int)
来源：http://hz.zhaomingkeji.xyz/gtfgbeoknb.html

[T57] Scala：模式匹配
来源：http://hz.bjfxy.top/gtdzitbxvs.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.yangfankeji.com/gtqwvygnhl.html

[T58] Scala：函数定义
来源：http://hz.svipenyu.cn/gtwchckyrw.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yj20258.top/gtnkcznpqo.html

[T59] Scala：循环
来源：http://hz.jianghu66.top/gtrnelvxfi.html

for (i <- 1 to 10) println(i)
来源：http://hz.redwolf501.top/gtyzvkvidi.html

[T60] Scala：折叠
来源：http://hz.sysykeji.top/gtuotgpdwg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.tanke756.top/gtohpnenvm.html

================================================================================
来源：http://hz.jiagoushi.top/gtwavpuxuq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.cqqwz.cn/gtwgdaqmyt.html

================================================================================
来源：http://hz.zhixingplan.top/gtiypvaajr.html

[U01] Py：创建虚拟环境
来源：http://hz.dianchejie.cn/gturhujvcv.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.tianlin.xyz/gtlyzwkbur.html

[U02] Py：导出 / 安装依赖
来源：http://hz.shanyushiyangkeji.top/gtjnziosmt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.xziqi.cn/gtemitngrk.html

[U03] Py：加载 .env 配置
来源：http://hz.smart0.xyz/gtsujtdfcv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.quarkkingdee.top/gtvordvdvd.html

[U04] Py：变量调试打印
来源：http://hz.gotoacloud.top/gtbwfgqrsb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.cdnleiting.top/gtnovwaxab.html

[U05] Py：列表去重且保序
来源：http://hz.pycfn.com/gtniholwoe.html

list(dict.fromkeys(arr))
来源：http://hz.zycfv.cn/gtknpwiqyo.html

[U06] Py：合并两个字典
来源：http://hz.ydzc1.top/gtkakwllni.html

{**a, **b}
来源：http://hz.shzxlz.cn/gtingavjxx.html

[U07] Py：反转字典键值
来源：http://hz.jiagoushi.top/gtjbgrtfnx.html

{v: k for k, v in d.items()}
来源：http://hz.fengsongda.top/gtlmfwbzfy.html

[U08] Py：展平二维列表
来源：http://hz.feifeiyinyue.top/gtykxooxzg.html

[y for x in nested for y in x]
来源：http://hz.ivvv.top/gthgtjaqtm.html

[U09] Py：字典取最大值的键
来源：http://hz.sysykeji.top/gtnmidtlsm.html

max(d, key=d.get)
来源：http://hz.jqgufenzy.top/gtzzkhlpqy.html

[U10] Py：按值排序字典
来源：http://hz.jqgfzy.top/gtmsruqpvo.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.zhoulong.xyz/gtnndachhd.html

[U11] Py：生成器表达式
来源：http://hz.gotoacloud.top/gtjqbgjjsh.html

(x * 2 for x in arr)
来源：http://hz.dianchejie.cn/gtsfzeyxzh.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.cqqwz.cn/gtuebgrsqi.html

Counter(arr).most_common(3)
来源：http://hz.guannengcc.top/gtrewybuge.html

[U13] Py：固定长度队列
来源：http://hz.52xcode.cn/gtabueradt.html

deque(maxlen=10)
来源：http://hz.yueranfly.top/gtpaveavex.html

[U14] Py：分组收集到列表
来源：http://hz.tian-w.cn/gtiltyhhcv.html

defaultdict(list)
来源：http://hz.pycfn.com/gtusbkdfhm.html

[U15] Py：高精度计时
来源：http://hz.cucudq.cn/gtehmwvodp.html

t = time.perf_counter()
来源：http://hz.aibaodan.cn/gtnpxslsse.html

[U16] Py：命令行参数解析
来源：http://hz.xylfe.cn/gtiiffxoai.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.0kj1m.cn/gtbdioocfm.html

[U17] Py：初始化日志
来源：http://hz.zhaomingkeji.xyz/gtgmyffvlr.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.hnxiangtu.top/gtjzppeudy.html

[U18] Py：预编译正则
来源：http://hz.chenlongwang.top/gtdsxzcuux.html

pat = re.compile(r"\d+")
来源：http://hz.feifeiyinyue.top/gtqfseafpt.html

[U19] Py：正则替换带回调
来源：http://hz.yuanzhike.top/gtdvydnjnf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.hnqzz.top/gtyqtbtdcj.html

[U20] Py：缓存函数结果
来源：http://hz.zhoulong.xyz/gtfajgzxea.html

@functools.lru_cache(maxsize=None)
来源：http://hz.havefunace.top/gtkpeoapkj.html

[U21] Py：自定义上下文管理器
来源：http://hz.shanyushiyangkeji.top/gtljqkbupo.html

@contextlib.contextmanager
来源：http://hz.daxiang520.top/gtkypazrxw.html

[U22] Py：矩阵转置
来源：http://hz.yueranfly.top/gtlkfcluue.html

list(zip(*m))
来源：http://hz.nanxinkj.top/gtyddhsraj.html

[U23] Py：分块读取大文件
来源：http://hz.ydjk.org.cn/gteqainalq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.mhx1999.top/gtelalqgwj.html

[U24] Py：路径操作
来源：http://hz.xuetiantiany.cn/gtgbyhxgau.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.zhiwuduotai.top/gtivtfegzr.html

[U25] Py：CSV 按字典读
来源：http://hz.52xcode.cn/gtukhgbape.html

csv.DictReader(f)
来源：http://hz.daria6918.cn/gtavpctgbo.html

[U26] Py：并发下载
来源：http://hz.xylfe.cn/gtyzvhqpzu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.shzxlz.cn/gtlmewysxl.html

[U27] Py：异步 HTTP
来源：http://hz.quarkkingdee.top/gtzlgfcvpb.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.chenjidiqi.icu/gtpgzkgbmq.html

[U28] Py：类型别名
来源：http://hz.wangdashe.top/gtqioslnaa.html

UserId = int
来源：http://hz.feifeiyinyue.top/gtygkbpfqs.html

[U29] Py：属性校验
来源：http://hz.chenjidiqi.icu/gtqpubcrbh.html

@property 与 @x.setter 配合
来源：http://hz.fzhhl.top/gtqdsqfoeb.html

[U30] Py：数据类
来源：http://hz.zhiwuduotai.top/gtsfmvezky.html

@dataclass(slots=True)
来源：http://hz.yj202588.top/gtopajndrq.html

[U31] Py：单测
来源：http://hz.birdmap.top/gtumfhoies.html

python -m pytest -q
来源：http://hz.sxryk.cn/gtiwckjtos.html

[U32] Py：代码格式化
来源：http://hz.kuanghao11.cn/gtrcbuqkfx.html

ruff format . && ruff check --fix .
来源：http://hz.hongshengwenyu.top/gtdmwfwgte.html

[U33] Py：打包发布
来源：http://hz.yj20258.top/gtxuwveqrc.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.wangshuangyany.cn/gtgbmlsxnj.html

[U34] Py：判断编码
来源：http://hz.zhixingplan.top/gtrrqlrddz.html

chardet.detect(raw)
来源：http://hz.guowangkeji.top/gtatkizzvz.html


<!-- 参考信息 -->