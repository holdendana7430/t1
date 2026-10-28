代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.bjfxy.top/gtdcaayfwq.html

[S08] C：动态内存分配与释放
来源：http://hz.nwbrower.top/gtwrajjhnn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jianghu66.top/gtxtmxgemn.html

[S09] C：结构体定义与初始化
来源：http://hz.c1oappe.top/gtrrbfettz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.birdmap.top/gtcmayijvu.html

[S10] C：指针与解引用
来源：http://hz.havefunace.top/gtfbyorzzk.html

int *p = &a;  *p = 5;
来源：http://hz.ppjwa.cn/gtrxewyyps.html

[S11] C：逐行读文件
来源：http://hz.birdmap.top/gtlpyrdfmz.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.guowangkeji.top/gttkllktnl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.chenzaomai.com/gtmtpuavap.html

fclose(f);
来源：http://hz.zhiwuduotai.top/gtldjfnnjl.html

[S12] C：写文件
来源：http://hz.vqdsnc.cn/gtvchghjki.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.nwbrower.top/gtjuyuxcwc.html

[S13] C：宏定义
来源：http://hz.jyoumei.cn/gtzqtcwvew.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ydzc1.top/gtsprlrcxk.html

[S14] C：枚举
来源：http://hz.gaohongyu789.top/gtdxyjokvp.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.meibo888.top/gtfiyqscab.html

[S15] C：类型转换
来源：http://hz.nwbrower.top/gtjxmksgxf.html

(double) a / b
来源：http://hz.yonumen.top/gtwihoafwt.html

[S16] C：位操作置位
来源：http://hz.aizwys.cn/gtrhslmuqk.html

x |= (1 << 3);
来源：http://hz.redwolf501.top/gtidegrldw.html

[S17] C：安全拼接字符串
来源：http://hz.gotoacloud.top/gtoreatful.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.tanke756.top/gtskkclbkg.html

[S18] C：命令行参数
来源：http://hz.yuxming.cn/gtzepriuox.html

int main(int argc, char **argv)
来源：http://hz.yj202588.top/gtchofyvst.html

[S19] C：快速排序
来源：http://hz.yj20258.top/gtdnlzemal.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.xinyue.icu/gtuzhmmlwp.html

[S20] C：二分查找
来源：http://hz.xuanzx.com/gtgztllcrb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.quarkkingdee.top/gtvrelrrnb.html

[S21] C：字符类别判断
来源：http://hz.wangdashe.top/gtsnpkomur.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ybcxt.top/gtyftmboun.html

[S22] C：字符串转数字
来源：http://hz.zhongyouzk.top/gtsiuovxoz.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jlsjyb.cn/gtlxtkxdtv.html

[S23] C：随机数
来源：http://hz.yj20258888.top/gtpeykcnzg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yj20258.top/gtdovbribw.html

[S24] C：获取本地时间
来源：http://hz.hongshengwenyu.top/gtaxupylqb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xinyue.icu/gtpkdmzkdv.html

[S25] C：内存拷贝
来源：http://hz.ivvv.top/gtqomkoqpf.html

memcpy(dst, src, n);
来源：http://hz.smart0.xyz/gtxhkswbrm.html

[S26] C：内存清零
来源：http://hz.aizwys.cn/gtikiyrplm.html

memset(a, 0, sizeof a);
来源：http://hz.0kj1m.cn/gtbnupqwvv.html

[S27] C：定义常量
来源：http://hz.zhoulong.xyz/gtyexyopzr.html

const double PI = 3.14159;
来源：http://hz.yj20258888.top/gtvwfnqapu.html

[S28] C：静态变量
来源：http://hz.ydzc1.top/gtjhlpbkry.html

static int counter = 0;
来源：http://hz.mhx1999.top/gtcjbwzuol.html

[S29] C：变参函数
来源：http://hz.tianlin.xyz/gtkutslavk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.gogol.net.cn/gtahmbaezg.html

[S30] C：头文件保护
来源：http://hz.316326.xyz/gtpwowajjr.html

#ifndef X_H
来源：http://hz.yuxming.cn/gtsjmhkeul.html

#define X_H
来源：http://hz.yj20258888.top/gtraobegbm.html

#endif
来源：http://hz.shuidangran.top/gtrkxjivoe.html

[S31] C++：Hello World
来源：http://hz.hongshengwenyu.top/gtdmmvjmdj.html

#include <iostream>
来源：http://hz.ivvv.top/gtvggvuvld.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yuxming.cn/gtukfvnpsu.html

[S32] C++：字符串
来源：http://hz.52xcode.cn/gtvytylqhq.html

std::string s = "hi";  s += "!";
来源：http://hz.jqgufenzy.top/gtaicwqebc.html

[S33] C++：vector 增删
来源：http://hz.haohaochexian.top/gtvuewvilk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.xuanzx.com/gtrmplnxqf.html

[S34] C++：遍历 vector
来源：http://hz.yuanzhike.top/gtcslbeitl.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yangfankeji.com/gtwvoehdap.html

[S35] C++：map
来源：http://hz.jianghu66.top/gterknbcir.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.kuanghao11.cn/gtbylggjkm.html

[S36] C++：unordered_map
来源：http://hz.jiagoushi.top/gtmtpeyaxb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.mhx1999.top/gtfwpttpcs.html

[S37] C++：set
来源：http://hz.jinghuilouyu.cn/gtyngbasfj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.gzhubu.top/gtectoknnl.html

[S38] C++：排序
来源：http://hz.shangyingyoupin.top/gtrwxjpamv.html

std::sort(v.begin(), v.end());
来源：http://hz.havefunace.top/gtgmqidqyp.html

[S39] C++：自定义比较器排序
来源：http://hz.sxryk.cn/gtwhvnapca.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jinqigfzy.top/gtbxtxozbj.html

[S40] C++：查找元素
来源：http://hz.guannengcc.top/gticnisils.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.quarkkingdee.top/gtiqqpmizz.html

[S41] C++：类与构造函数
来源：http://hz.redwolf501.top/gtonrbmavj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhijiandao.cn/gtizsugxwo.html

[S42] C++：继承与虚函数
来源：http://hz.chenzaomai.com/gtgkwrhxpv.html

class B : public Base { public: void f() override {} };
来源：http://hz.ivvv.top/gttrhrnxgw.html

[S43] C++：智能指针
来源：http://hz.zhiwuduotai.top/gtonxcmcls.html

auto p = std::make_unique<int>(5);
来源：http://hz.tianlin.xyz/gtmneiinii.html

[S44] C++：引用传参
来源：http://hz.hammf.cn/gtdisyykkw.html

void inc(int &x) { ++x; }
来源：http://hz.ehwqpu.com/gtwgrttydg.html

[S45] C++：lambda
来源：http://hz.yangfankeji.com/gtaksfwtco.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cdnleiting.top/gtziexpubh.html

[S46] C++：函数模板
来源：http://hz.zhijiandao.cn/gtklcxfhiv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shangyingyoupin.top/gtrnsvzcub.html

[S47] C++：结构化绑定遍历
来源：http://hz.xziqi.cn/gtjatmojyq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.tanke756.top/gtxmksrehu.html

[S48] C++：逐行读文件
来源：http://hz.52xcode.cn/gtmsbgnnaw.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yvedp.cn/gtzqzzzxii.html

while (std::getline(in, line)) { }
来源：http://hz.sysykeji.top/gtatcgwobz.html

[S49] C++：写文件
来源：http://hz.pycfn.com/gtqxziotyp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.iojbl.cn/gtdywgsugk.html

[S50] C++：格式化数字
来源：http://hz.chenzaomai.com/gtofujhlws.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.pycfn.com/gtinktudmw.html

[S51] C++：显式类型转换
来源：http://hz.shangyingyoupin.top/gtitqmldqn.html

static_cast<double>(a) / b
来源：http://hz.yongpay.top/gtvcegdjsw.html

[S52] C++：const 与 noexcept
来源：http://hz.ydjk.org.cn/gtmgouynol.html

int size() const noexcept { return n_; }
来源：http://hz.gzhubu.top/gtyxmtcyse.html

[S53] C++：移动语义
来源：http://hz.daria6918.cn/gtvwmwjdbw.html

std::vector<int> w = std::move(v);
来源：http://hz.ywan-chungtsiang.top/gtybuqhjym.html

[S54] C++：异常处理
来源：http://hz.shangyingyoupin.top/gtwvgnwtcb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.iojbl.cn/gtvdneflkl.html

[S55] C++：结构化绑定
来源：http://hz.zdqjudy.top/gtouwozlbg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.nwbrower.top/gtdcrnijsf.html

[S56] C++：optional
来源：http://hz.hnxiangtu.top/gtlqmammzr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.aizwys.cn/gtswbrcwpv.html

[S57] C++：编译期常量
来源：http://hz.cashguo.top/gtbalefhcx.html

constexpr int N = 10;
来源：http://hz.jinqigufen.top/gtbduwaawx.html

[S58] C++：命名空间
来源：http://hz.jiagoushi.top/gtcrshnpez.html

namespace ns { int f() { return 1; } }
来源：http://hz.guowangkeji.top/gtcxrgfgdc.html

[S59] C++：静态断言
来源：http://hz.zhixingplan.top/gtkdjsozhc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.sweek.top/gtltplylaw.html

[S60] C++：遍历并删除元素
来源：http://hz.daria6918.cn/gtvjuhhnhy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.xingfuxueyuan.xyz/gtrpknigfo.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtpfxaadny.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.kuanghao11.cn/gtsanfcqug.html

================================================================================
来源：http://hz.xinyue.icu/gtpdizducf.html

[T01] Kotlin：Hello World
来源：http://hz.kuanghao11.cn/gtshzobinw.html

println("Hello")
来源：http://hz.xuetiantiany.cn/gtcxnwldke.html

[T02] Kotlin：变量
来源：http://hz.haohaochexian.top/gtlvqevcma.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jyoumei.cn/gtqypfkafu.html

[T03] Kotlin：字符串模板
来源：http://hz.ydzc1.top/gtxjrsuiay.html

"值: $b"
来源：http://hz.shanyushiyangtech.top/gtcicdotmf.html

[T04] Kotlin：空安全
来源：http://hz.hongshengwenyu.top/gtlwprgoks.html

val n: String? = null;  n?.length
来源：http://hz.yonumen.top/gtwlozogft.html

[T05] Kotlin：when 表达式
来源：http://hz.meibo888.top/gtkmoxevtk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.xziqi.cn/gttomkkyux.html

[T06] Kotlin：集合映射
来源：http://hz.yj20258.top/gtsztccdgf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.gzhubu.top/gtywxwlnov.html

[T07] Kotlin：集合过滤
来源：http://hz.ybcxt.top/gtskkusayc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.gogol.net.cn/gtnjmncnzt.html

[T08] Kotlin：数据类
来源：http://hz.shuidangran.top/gtmypzdkos.html

data class User(val name: String, val age: Int)
来源：http://hz.zdqjudy.top/gtrhasbtmc.html

[T09] Kotlin：扩展函数
来源：http://hz.xinyue.icu/gtauarntwx.html

fun String.exclaim() = this + "!"
来源：http://hz.feifeiyinyue.top/gtgmynbyrg.html

[T10] Kotlin：默认参数
来源：http://hz.zhoulong.xyz/gtfumsqnxr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.sufxvd.cn/gtdugdqeeu.html

[T11] Kotlin：协程
来源：http://hz.yj20258.top/gtpjgmnsil.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.tianlin.xyz/gtvafqloum.html

[T12] Kotlin：解构声明
来源：http://hz.mhx1999.top/gtskgtvamn.html

val (a, b) = Pair(1, 2)
来源：http://hz.jlsjyb.cn/gtwkirunke.html

[T13] Kotlin：只读 Map
来源：http://hz.birdmap.top/gtzqrylssp.html

val m = mapOf("a" to 1)
来源：http://hz.hysaishi.cn/gtfcetzcqm.html

[T14] Kotlin：循环
来源：http://hz.cheryme.top/gtnftmxsfr.html

for (i in 1..10) println(i)
来源：http://hz.hysaishi.cn/gtwejlemqu.html

[T15] Kotlin：接口
来源：http://hz.haohaochexian.top/gttndtmogq.html

interface Shape { fun area(): Double }
来源：http://hz.hfpthk.cn/gtvqirgskx.html

[T16] Swift：Hello World
来源：http://hz.andypj.xyz/gtkwvrfrfb.html

print("Hello")
来源：http://hz.mhx1999.top/gtgsrasogp.html

[T17] Swift：变量与常量
来源：http://hz.jiagoushi.top/gthaklgfri.html

var a = 1;  let b = 2
来源：http://hz.yj20258.top/gtrdptgmjc.html

[T18] Swift：字符串插值
来源：http://hz.mhx1999.top/gtemebsrmm.html

"值: \(b)"
来源：http://hz.birdmap.top/gtqlkgejuy.html

[T19] Swift：可选绑定
来源：http://hz.ppjwa.cn/gthbvytpkd.html

if let n = opt { print(n) }
来源：http://hz.hnqzz.top/gtxeusqxld.html

[T20] Swift：数组操作
来源：http://hz.xziqi.cn/gtcjhyausu.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.shanyushiyangkeji.top/gtjqeodwlx.html

[T21] Swift：遍历
来源：http://hz.zhaomingkeji.xyz/gtbebkumca.html

for x in a { print(x) }
来源：http://hz.cdnleiting.top/gtkxxgjbbj.html

[T22] Swift：字典
来源：http://hz.gaohongyu789.top/gtqtwtgzjx.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yangfankeji.com/gtlqcfqrgw.html

[T23] Swift：函数
来源：http://hz.zhiwuduotai.top/gtlgmmkflc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.c1oappe.top/gtlfguuzlb.html

[T24] Swift：闭包
来源：http://hz.guannengcc.top/gtzlfujcmh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jqgufenzy.top/gtwnxkherd.html

[T25] Swift：结构体
来源：http://hz.bjfxy.top/gtyxlfhhdp.html

struct P { var x: Int }
来源：http://hz.hongshengwenyu.top/gtzclljbhv.html

[T26] Swift：类与重写
来源：http://hz.aizwys.cn/gtivatgzus.html

class A: Base { override func f() {} }
来源：http://hz.tanke756.top/gtoiczbiiz.html

[T27] Swift：错误处理
来源：http://hz.havefunace.top/gtujbzirgj.html

do { try f() } catch { print(error) }
来源：http://hz.kuanghao11.cn/gtxqptyojj.html

[T28] Swift：枚举
来源：http://hz.hammf.cn/gtcycslmjv.html

enum Color { case red, green }
来源：http://hz.chenlongwang.top/gtljzmygsd.html

[T29] Swift：guard 提前返回
来源：http://hz.havefunace.top/gtevmuuoub.html

guard let x = opt else { return }
来源：http://hz.yuxming.cn/gtcofogstt.html

[T30] Swift：协议
来源：http://hz.hnxiangtu.top/gtpsghzycn.html

protocol Shape { func area() -> Double }
来源：http://hz.pycfn.com/gtkxppzwdf.html

[T31] Lua：Hello World
来源：http://hz.sufxvd.cn/gtgcrtlmjp.html

print("Hello")
来源：http://hz.tanke756.top/gtubqkncsa.html

[T32] Lua：局部变量
来源：http://hz.cqqwz.cn/gtemuxbgsb.html

local a = 1
来源：http://hz.meibo888.top/gttucstsqn.html

[T33] Lua：表（数组）
来源：http://hz.shanyushiyangtech.top/gtwituwrts.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.aibaodan.cn/gtatnwtbzj.html

[T34] Lua：遍历表
来源：http://hz.tian-w.cn/gthebrvtmo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.shuidangran.top/gtpozjsrfb.html

[T35] Lua：字典表
来源：http://hz.jianghu66.top/gtwaocfuue.html

local d = { a = 1 };  d.b = 2
来源：http://hz.cdnleiting.top/gtrltdilxs.html

[T36] Lua：函数
来源：http://hz.xylfe.cn/gtxblcgkiv.html

function add(a, b) return a + b end
来源：http://hz.havefunace.top/gtdwqnbrmp.html

[T37] Lua：字符串拼接
来源：http://hz.316326.xyz/gtmsfrnzcm.html

"a" .. "b"
来源：http://hz.jinyuanbaomall.cn/gtyafqlpiq.html

[T38] Lua：条件
来源：http://hz.ydzc1.top/gtaykdcezx.html

if x > 0 then print("正") end
来源：http://hz.sufxvd.cn/gtkmpgkxxf.html

[T39] Lua：模式匹配
来源：http://hz.yj202588.top/gtptlgpwho.html

string.find(s, "%d+")
来源：http://hz.cdnleiting.top/gtswjcseuf.html

[T40] Lua：元表
来源：http://hz.jiagoushi.top/gtilxplhep.html

setmetatable({}, { __index = base })
来源：http://hz.xinyue.icu/gtpzykiicb.html

[T41] Perl：Hello World
来源：http://hz.zhaomingkeji.xyz/gtybvvndnf.html

print "Hello\n";
来源：http://hz.sxryk.cn/gtwpmhufjk.html

[T42] Perl：变量类型
来源：http://hz.daxiang520.top/gtjtccjplr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yonumen.top/gthcykchdm.html

[T43] Perl：字符串插值
来源：http://hz.yuanzhike.top/gtkkucnpvi.html

"值: $a"
来源：http://hz.zdqjudy.top/gtppexiobg.html

[T44] Perl：条件
来源：http://hz.tianlin.xyz/gtajjobucd.html

if ($a > 0) { print "正"; }
来源：http://hz.ivvv.top/gtgpdqlrar.html

[T45] Perl：数组遍历
来源：http://hz.zhiwuduotai.top/gtdlonvnsg.html

for my $x (@arr) { print $x; }
来源：http://hz.quarkkingdee.top/gtatunbyca.html

[T46] Perl：哈希操作
来源：http://hz.dianchejie.cn/gtmyleesgh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yj20258888.top/gtobqkayio.html

[T47] Perl：正则捕获
来源：http://hz.zhoulong.xyz/gtehmxihxs.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.aibaodan.cn/gtuejizcrk.html

[T48] Perl：正则替换
来源：http://hz.havefunace.top/gtrriynlhx.html

$s =~ s/old/new/g;
来源：http://hz.wangshuangyany.cn/gtdzubhhcm.html

[T49] Perl：函数
来源：http://hz.birdmap.top/gtuxdmtgsu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.smart0.xyz/gtgshwbvkx.html

[T50] Perl：逐行读文件
来源：http://hz.yvedp.cn/gtfrlwnipi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yj20258888.top/gtqwapajjp.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.zhaomingkeji.xyz/gtyhixutca.html

[T51] Scala：Hello World
来源：http://hz.iojbl.cn/gtqgksdtkb.html

println("Hello")
来源：http://hz.guannengcc.top/gtoqdtbuyh.html

[T52] Scala：变量
来源：http://hz.ehwqpu.com/gtanvkkwkk.html

val a = 1;  var b = 2
来源：http://hz.zhixingplan.top/gtqowdrwsw.html

[T53] Scala：字符串插值
来源：http://hz.ehwqpu.com/gtfncuchot.html

s"值: $b"
来源：http://hz.jqgufenzy.top/gttcnhwvzn.html

[T54] Scala：集合映射
来源：http://hz.yuxming.cn/gtvtazuaue.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.zhongyouzk.top/gtwkchtcow.html

[T55] Scala：集合过滤
来源：http://hz.shuidangran.top/gtcuqnoxvq.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.kuanghao11.cn/gthltjspun.html

[T56] Scala：样例类
来源：http://hz.yonumen.top/gtzijuqpah.html

case class User(name: String, age: Int)
来源：http://hz.dianchejie.cn/gtfwufslml.html

[T57] Scala：模式匹配
来源：http://hz.hammf.cn/gtfgmweeyg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.yongpay.top/gtqlzrzxhs.html

[T58] Scala：函数定义
来源：http://hz.yangfankeji.com/gtvtroxwos.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.daria6918.cn/gtcrukmbpj.html

[T59] Scala：循环
来源：http://hz.cdnleiting.top/gtnxvgleyw.html

for (i <- 1 to 10) println(i)
来源：http://hz.fzhhl.top/gtnpgzomfs.html

[T60] Scala：折叠
来源：http://hz.jinqigufen.top/gtnphtxhdv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.gzhubu.top/gthvmapbey.html

================================================================================
来源：http://hz.havefunace.top/gtflzbtawh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yj20258.top/gtatmgerey.html

================================================================================
来源：http://hz.fzhhl.top/gtchpxnmrn.html

[U01] Py：创建虚拟环境
来源：http://hz.snrcjt.cn/gtpnxrvrew.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.tian-w.cn/gtwmonwdtk.html

[U02] Py：导出 / 安装依赖
来源：http://hz.daria6918.cn/gtrsgjcvgw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.birdmap.top/gtkqxiogty.html

[U03] Py：加载 .env 配置
来源：http://hz.daria6918.cn/gtxbsgtucx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.xuetiantiany.cn/gtjtyklxbr.html

[U04] Py：变量调试打印
来源：http://hz.jinqigfzy.top/gtzaypvvww.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.chenlongwang.top/gttgegrsok.html

[U05] Py：列表去重且保序
来源：http://hz.pengpengdd.cyou/gtpmvkwhxz.html

list(dict.fromkeys(arr))
来源：http://hz.0kj1m.cn/gtugomeaat.html

[U06] Py：合并两个字典
来源：http://hz.cqqwz.cn/gtwjxgjkhb.html

{**a, **b}
来源：http://hz.yueranfly.top/gtfmmwrxhl.html

[U07] Py：反转字典键值
来源：http://hz.svipenyu.cn/gtvgmfzocg.html

{v: k for k, v in d.items()}
来源：http://hz.yuanzhike.top/gtwdiazuur.html

[U08] Py：展平二维列表
来源：http://hz.nwbrower.top/gttrqcntae.html

[y for x in nested for y in x]
来源：http://hz.hammf.cn/gtvueecgml.html

[U09] Py：字典取最大值的键
来源：http://hz.ehwqpu.com/gtenupnebw.html

max(d, key=d.get)
来源：http://hz.yueranfly.top/gtdwtwcgan.html

[U10] Py：按值排序字典
来源：http://hz.cheryme.top/gtlqxysiyb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.tianlin.xyz/gtmpwotguc.html

[U11] Py：生成器表达式
来源：http://hz.yuanzhike.top/gtjvbymqnv.html

(x * 2 for x in arr)
来源：http://hz.jqgfzy.top/gtacquqrcg.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yuxming.cn/gtypdyvrau.html

Counter(arr).most_common(3)
来源：http://hz.zdqjudy.top/gtmsfmdues.html

[U13] Py：固定长度队列
来源：http://hz.sweek.top/gtjeqckpuv.html

deque(maxlen=10)
来源：http://hz.yj202588.top/gtgxblnlzd.html

[U14] Py：分组收集到列表
来源：http://hz.gotoacloud.top/gtzkioneje.html

defaultdict(list)
来源：http://hz.birdmap.top/gtkesjfhbt.html

[U15] Py：高精度计时
来源：http://hz.gotoacloud.top/gtaiegyosy.html

t = time.perf_counter()
来源：http://hz.kuanghao11.cn/gtulxxbjsb.html

[U16] Py：命令行参数解析
来源：http://hz.guannengcc.top/gtljictlkh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jqgfzy.top/gtlvbwiqlc.html

[U17] Py：初始化日志
来源：http://hz.yonumen.top/gtlntpszqv.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.hywenlv.cn/gtjwjptuyq.html

[U18] Py：预编译正则
来源：http://hz.feifeiyinyue.top/gtgyldymsz.html

pat = re.compile(r"\d+")
来源：http://hz.xuetiantiany.cn/gtiuhxhnlx.html

[U19] Py：正则替换带回调
来源：http://hz.daxiang520.top/gtaoadbqxx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.tianlin.xyz/gtuagrfsow.html

[U20] Py：缓存函数结果
来源：http://hz.zhaomingkeji.xyz/gtcfmiukad.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jianghu66.top/gtxoxevyvw.html

[U21] Py：自定义上下文管理器
来源：http://hz.zhongyouzk.top/gthciloubd.html

@contextlib.contextmanager
来源：http://hz.shuidangran.top/gtvaovaijh.html

[U22] Py：矩阵转置
来源：http://hz.xinyue.icu/gteiwfxjfr.html

list(zip(*m))
来源：http://hz.fengsongda.top/gtrgswwfkh.html

[U23] Py：分块读取大文件
来源：http://hz.cucudq.cn/gtzrvkyslq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.zhoulong.xyz/gtmhwiyybp.html

[U24] Py：路径操作
来源：http://hz.xuanzx.com/gtuowacxlp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.gotoacloud.top/gtbdtfbpqr.html

[U25] Py：CSV 按字典读
来源：http://hz.nanxinkj.top/gtnocdpsuj.html

csv.DictReader(f)
来源：http://hz.meibo888.top/gtywzhizvz.html

[U26] Py：并发下载
来源：http://hz.ywan-chungtsiang.top/gtpkocgcrp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.zycfv.cn/gtklqgsxnz.html

[U27] Py：异步 HTTP
来源：http://hz.redwolf501.top/gtfuswbtcu.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.bjfxy.top/gtaetfnpmu.html

[U28] Py：类型别名
来源：http://hz.pengpengdd.cyou/gtschunjvf.html

UserId = int
来源：http://hz.dashuyun.cn/gtboaysrki.html

[U29] Py：属性校验
来源：http://hz.ydjk.org.cn/gtngiczzcg.html

@property 与 @x.setter 配合
来源：http://hz.shangyingyoupin.top/gtfexobxsc.html

[U30] Py：数据类
来源：http://hz.0kj1m.cn/gtmafrhxht.html

@dataclass(slots=True)
来源：http://hz.pengpengdd.cyou/gtfmhdbsod.html


<!-- 参考信息 -->