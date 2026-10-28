代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://hz.pycfn.com/gtaobssfif.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.havefunace.top/gtilbchfgi.html

fclose(f);
来源：http://hz.vqdsnc.cn/gtcihxqfwg.html

[S12] C：写文件
来源：http://hz.wangdashe.top/gtecrbdafm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hywenlv.cn/gtiiwufhuj.html

[S13] C：宏定义
来源：http://hz.zycfv.cn/gttyhceoge.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zdqjudy.top/gtdjyqthto.html

[S14] C：枚举
来源：http://hz.xingfuxueyuan.xyz/gtvmjosqed.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.smart0.xyz/gtvhbcvsru.html

[S15] C：类型转换
来源：http://hz.zhiwuduotai.top/gtnvrufmew.html

(double) a / b
来源：http://hz.tianlin.xyz/gtsgmpcwwd.html

[S16] C：位操作置位
来源：http://hz.tian-w.cn/gtrkbqmquo.html

x |= (1 << 3);
来源：http://hz.jinghuilouyu.cn/gtoorlzwmy.html

[S17] C：安全拼接字符串
来源：http://hz.shanyushiyangkeji.top/gtsecjtqnp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zdqjudy.top/gtkkrxcrfe.html

[S18] C：命令行参数
来源：http://hz.zhijiandao.cn/gteuzhtdua.html

int main(int argc, char **argv)
来源：http://hz.daria6918.cn/gtnawbuqgd.html

[S19] C：快速排序
来源：http://hz.zhongyouzk.top/gtbsedgjzm.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.gogol.net.cn/gtkeqrbvrn.html

[S20] C：二分查找
来源：http://hz.jinyuanbaomall.cn/gtubksgflr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.daxiang520.top/gtisfmtuya.html

[S21] C：字符类别判断
来源：http://hz.yvedp.cn/gtmnpzvwng.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.cqqwz.cn/gtytwmfmgq.html

[S22] C：字符串转数字
来源：http://hz.jqgfzy.top/gtrmurwsmw.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yj20258888.top/gtujuutfpj.html

[S23] C：随机数
来源：http://hz.hysaishi.cn/gtxheuioco.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.cheryme.top/gtrqcrzouf.html

[S24] C：获取本地时间
来源：http://hz.c1oappe.top/gtjpfynpaj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ybcxt.top/gtfovoohag.html

[S25] C：内存拷贝
来源：http://hz.fengsongda.top/gtxtwxrldz.html

memcpy(dst, src, n);
来源：http://hz.zhijiandao.cn/gtshavnewd.html

[S26] C：内存清零
来源：http://hz.jianghu66.top/gtbsuhlkce.html

memset(a, 0, sizeof a);
来源：http://hz.meibo888.top/gtebjhqjjz.html

[S27] C：定义常量
来源：http://hz.vqdsnc.cn/gtjkrjzivl.html

const double PI = 3.14159;
来源：http://hz.hammf.cn/gtogozxbji.html

[S28] C：静态变量
来源：http://hz.zhixingplan.top/gtisnifvbs.html

static int counter = 0;
来源：http://hz.jlsjyb.cn/gtvfkqxooz.html

[S29] C：变参函数
来源：http://hz.shuidangran.top/gtantudxtj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.shanyushiyangkeji.top/gtmzczxzar.html

[S30] C：头文件保护
来源：http://hz.jqgfzy.top/gtipkmsgnf.html

#ifndef X_H
来源：http://hz.316326.xyz/gtaudgfeju.html

#define X_H
来源：http://hz.yongpay.top/gtmrpeytwv.html

#endif
来源：http://hz.xuetiantiany.cn/gtqkbvndla.html

[S31] C++：Hello World
来源：http://hz.ydjk.org.cn/gtecroqwlx.html

#include <iostream>
来源：http://hz.meibo888.top/gtsiosajrw.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yj202588.top/gtdspfkchr.html

[S32] C++：字符串
来源：http://hz.zhongyouzk.top/gtznbpqlea.html

std::string s = "hi";  s += "!";
来源：http://hz.ydjk.org.cn/gtxpyihmgs.html

[S33] C++：vector 增删
来源：http://hz.aizwys.cn/gtmcjbmgrx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.daria6918.cn/gtqqsqsoar.html

[S34] C++：遍历 vector
来源：http://hz.aizwys.cn/gtpywrqwha.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.316326.xyz/gtaxtebayy.html

[S35] C++：map
来源：http://hz.ehwqpu.com/gtztsolfhy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinyuanbaomall.cn/gtgabgsohw.html

[S36] C++：unordered_map
来源：http://hz.shanyushiyangkeji.top/gtdbhijwry.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.guannengcc.top/gtrgucgmul.html

[S37] C++：set
来源：http://hz.xuanzx.com/gtkqvrwysv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.chenlongwang.top/gtdpxcbvzb.html

[S38] C++：排序
来源：http://hz.c1oappe.top/gtfuygkvxv.html

std::sort(v.begin(), v.end());
来源：http://hz.feifeiyinyue.top/gttrtoihol.html

[S39] C++：自定义比较器排序
来源：http://hz.jlsjyb.cn/gtdzshotrm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhoulong.xyz/gtmlfwwosq.html

[S40] C++：查找元素
来源：http://hz.shangyingyoupin.top/gtduywsiog.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.chenlongwang.top/gtvgxayqgj.html

[S41] C++：类与构造函数
来源：http://hz.hysaishi.cn/gtqzdtbksm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.gotoacloud.top/gtrbokdptf.html

[S42] C++：继承与虚函数
来源：http://hz.nanxinkj.top/gtinwqupcd.html

class B : public Base { public: void f() override {} };
来源：http://hz.c1oappe.top/gtnujdyujo.html

[S43] C++：智能指针
来源：http://hz.hfpthk.cn/gtipprbqid.html

auto p = std::make_unique<int>(5);
来源：http://hz.jyoumei.cn/gtmkisaszl.html

[S44] C++：引用传参
来源：http://hz.ydjk.org.cn/gttjlrkxvt.html

void inc(int &x) { ++x; }
来源：http://hz.cheryme.top/gtbdtgilne.html

[S45] C++：lambda
来源：http://hz.ydzc1.top/gtunxtuuet.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.guowangkeji.top/gtncrmwjkm.html

[S46] C++：函数模板
来源：http://hz.tianlin.xyz/gtsoogwcyd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.9152youxi.cn/gtrfjglelw.html

[S47] C++：结构化绑定遍历
来源：http://hz.gzhubu.top/gtxzyahlpd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.hywenlv.cn/gtazmzpkqd.html

[S48] C++：逐行读文件
来源：http://hz.c1oappe.top/gtxnhhalyf.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shangyingyoupin.top/gthuwwcxko.html

while (std::getline(in, line)) { }
来源：http://hz.wangdashe.top/gtcmldqiwo.html

[S49] C++：写文件
来源：http://hz.jinghuilouyu.cn/gtrecdnqbh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.andypj.xyz/gthvdgochg.html

[S50] C++：格式化数字
来源：http://hz.ivvv.top/gtenbxdcqj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yanxiufei.cn/gtpfvwnyfi.html

[S51] C++：显式类型转换
来源：http://hz.zhaomingkeji.xyz/gtlxquqfys.html

static_cast<double>(a) / b
来源：http://hz.shzxlz.cn/gtkqoxkaof.html

[S52] C++：const 与 noexcept
来源：http://hz.jiagoushi.top/gtrqqbglpg.html

int size() const noexcept { return n_; }
来源：http://hz.bjfxy.top/gtiwmvjlgd.html

[S53] C++：移动语义
来源：http://hz.redwolf501.top/gtezdgyzqt.html

std::vector<int> w = std::move(v);
来源：http://hz.hongshengwenyu.top/gtzugoziux.html

[S54] C++：异常处理
来源：http://hz.iojbl.cn/gtkljogewf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.cdnleiting.top/gtjdosghqu.html

[S55] C++：结构化绑定
来源：http://hz.shzxlz.cn/gtjzszhgjk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.hongshengwenyu.top/gtrdnhbqgj.html

[S56] C++：optional
来源：http://hz.svipenyu.cn/gtkayefpyu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhixingplan.top/gtjcaynenh.html

[S57] C++：编译期常量
来源：http://hz.zdqjudy.top/gtjvwfrmoe.html

constexpr int N = 10;
来源：http://hz.jinqigfzy.top/gttsnfciai.html

[S58] C++：命名空间
来源：http://hz.feifeiyinyue.top/gtpayibnii.html

namespace ns { int f() { return 1; } }
来源：http://hz.cheryme.top/gtgtaibzgd.html

[S59] C++：静态断言
来源：http://hz.hnxiangtu.top/gtnraucbsp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.quarkkingdee.top/gtknuarfez.html

[S60] C++：遍历并删除元素
来源：http://hz.xingfuxueyuan.xyz/gtsuswapey.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yj20258.top/gtyqcwwdbm.html

================================================================================
来源：http://hz.dashuyun.cn/gtijrouxky.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.gaohongyu789.top/gtcfelyulr.html

================================================================================
来源：http://hz.hammf.cn/gtsvjaibqz.html

[T01] Kotlin：Hello World
来源：http://hz.kuanghao11.cn/gtxlyvmvhr.html

println("Hello")
来源：http://hz.chenzaomai.com/gtmnlckpyr.html

[T02] Kotlin：变量
来源：http://hz.hammf.cn/gtvcmeycko.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jyoumei.cn/gtvhiwdoxo.html

[T03] Kotlin：字符串模板
来源：http://hz.xuanzx.com/gtwyftakna.html

"值: $b"
来源：http://hz.meibo888.top/gtunhgadyp.html

[T04] Kotlin：空安全
来源：http://hz.xingfuxueyuan.xyz/gtshwazmnq.html

val n: String? = null;  n?.length
来源：http://hz.xuetiantiany.cn/gtccfaikbl.html

[T05] Kotlin：when 表达式
来源：http://hz.smart0.xyz/gttwnmrunj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jlsjyb.cn/gtrdpnlsuh.html

[T06] Kotlin：集合映射
来源：http://hz.wangshuangyany.cn/gtakemfvgt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.shzxlz.cn/gteaftwwsq.html

[T07] Kotlin：集合过滤
来源：http://hz.gotoacloud.top/gtycdekpfg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.ybcxt.top/gtgrurvwfc.html

[T08] Kotlin：数据类
来源：http://hz.ehwqpu.com/gtxmtczplr.html

data class User(val name: String, val age: Int)
来源：http://hz.tanke756.top/gtnmzymwnt.html

[T09] Kotlin：扩展函数
来源：http://hz.jyoumei.cn/gtpkphyric.html

fun String.exclaim() = this + "!"
来源：http://hz.jlsjyb.cn/gtbxpzbawh.html

[T10] Kotlin：默认参数
来源：http://hz.jqgfzy.top/gtspcvulls.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.tanke756.top/gtxwnpcqym.html

[T11] Kotlin：协程
来源：http://hz.jinyuanbaomall.cn/gtvjhlldwm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.hfpthk.cn/gtfhmgtknx.html

[T12] Kotlin：解构声明
来源：http://hz.yonumen.top/gtkvioepso.html

val (a, b) = Pair(1, 2)
来源：http://hz.sxryk.cn/gtytsnoopt.html

[T13] Kotlin：只读 Map
来源：http://hz.andypj.xyz/gtvwyjfquq.html

val m = mapOf("a" to 1)
来源：http://hz.mhx1999.top/gtduwgbbvt.html

[T14] Kotlin：循环
来源：http://hz.gotoacloud.top/gthufabrix.html

for (i in 1..10) println(i)
来源：http://hz.hongshengwenyu.top/gtbzuxzrij.html

[T15] Kotlin：接口
来源：http://hz.jlsjyb.cn/gtpsbwexxd.html

interface Shape { fun area(): Double }
来源：http://hz.andypj.xyz/gtetusducq.html

[T16] Swift：Hello World
来源：http://hz.yuxming.cn/gtymsgslmf.html

print("Hello")
来源：http://hz.ywan-chungtsiang.top/gtbleovqkv.html

[T17] Swift：变量与常量
来源：http://hz.svipenyu.cn/gtvaqoygsn.html

var a = 1;  let b = 2
来源：http://hz.xylfe.cn/gtspwsynqk.html

[T18] Swift：字符串插值
来源：http://hz.smart0.xyz/gtrempaovh.html

"值: \(b)"
来源：http://hz.hnxiangtu.top/gtacaxeruu.html

[T19] Swift：可选绑定
来源：http://hz.haohaochexian.top/gtxhcxwwqf.html

if let n = opt { print(n) }
来源：http://hz.gaohongyu789.top/gtjvwfkctq.html

[T20] Swift：数组操作
来源：http://hz.fengsongda.top/gtwcposwnu.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.cucudq.cn/gtzabkhfnb.html

[T21] Swift：遍历
来源：http://hz.zycfv.cn/gtkgwjcjqw.html

for x in a { print(x) }
来源：http://hz.smart0.xyz/gtukdnnhof.html

[T22] Swift：字典
来源：http://hz.zhixingplan.top/gtwacrbkxz.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.cdnleiting.top/gtfrgpnegi.html

[T23] Swift：函数
来源：http://hz.dashuyun.cn/gtbyzbxzsz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.birdmap.top/gtqukjwywr.html

[T24] Swift：闭包
来源：http://hz.cdnleiting.top/gtvybgjese.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.daxiang520.top/gtqhkdaiks.html

[T25] Swift：结构体
来源：http://hz.wangshuangyany.cn/gtyarkjzuj.html

struct P { var x: Int }
来源：http://hz.guowangkeji.top/gtqajmdaap.html

[T26] Swift：类与重写
来源：http://hz.tianlin.xyz/gtzitplrmj.html

class A: Base { override func f() {} }
来源：http://hz.ehwqpu.com/gtqkukbtgl.html

[T27] Swift：错误处理
来源：http://hz.yangfankeji.com/gtdofdwfkb.html

do { try f() } catch { print(error) }
来源：http://hz.wangshuangyany.cn/gtlcdjzqaq.html

[T28] Swift：枚举
来源：http://hz.shzxlz.cn/gtrdqihuxi.html

enum Color { case red, green }
来源：http://hz.jqgufenzy.top/gtrkawvpfh.html

[T29] Swift：guard 提前返回
来源：http://hz.feifeiyinyue.top/gtrnlltsjt.html

guard let x = opt else { return }
来源：http://hz.sweek.top/gtuzkxqtcv.html

[T30] Swift：协议
来源：http://hz.9152youxi.cn/gtjioyoyrk.html

protocol Shape { func area() -> Double }
来源：http://hz.feifeiyinyue.top/gtvbbbegnn.html

[T31] Lua：Hello World
来源：http://hz.hywenlv.cn/gtjamwukku.html

print("Hello")
来源：http://hz.wangdashe.top/gtjnmcyuzh.html

[T32] Lua：局部变量
来源：http://hz.yonumen.top/gthlnaovjk.html

local a = 1
来源：http://hz.tian-w.cn/gtaojzvdqc.html

[T33] Lua：表（数组）
来源：http://hz.guowangkeji.top/gtklliezun.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.sufxvd.cn/gtpgsbuehv.html

[T34] Lua：遍历表
来源：http://hz.ivvv.top/gtjybcfqfu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yvedp.cn/gtzxwkrpjd.html

[T35] Lua：字典表
来源：http://hz.yangfankeji.com/gtwdvyavtd.html

local d = { a = 1 };  d.b = 2
来源：http://hz.fengsongda.top/gtgtjewtki.html

[T36] Lua：函数
来源：http://hz.jqgufenzy.top/gttqcojjao.html

function add(a, b) return a + b end
来源：http://hz.jinyuanbaomall.cn/gtqoweimll.html

[T37] Lua：字符串拼接
来源：http://hz.cucudq.cn/gtcuwyxbbi.html

"a" .. "b"
来源：http://hz.sufxvd.cn/gtwkdidbwa.html

[T38] Lua：条件
来源：http://hz.hfpthk.cn/gtwdpdfrqn.html

if x > 0 then print("正") end
来源：http://hz.yonumen.top/gtyoglqkly.html

[T39] Lua：模式匹配
来源：http://hz.aizwys.cn/gtffsjobpz.html

string.find(s, "%d+")
来源：http://hz.andypj.xyz/gtadtqkkqt.html

[T40] Lua：元表
来源：http://hz.jlsjyb.cn/gtxmnbydcs.html

setmetatable({}, { __index = base })
来源：http://hz.yj202588.top/gtdqgljmgl.html

[T41] Perl：Hello World
来源：http://hz.kuanghao11.cn/gtscvvtvli.html

print "Hello\n";
来源：http://hz.gaohongyu789.top/gtagrofmnx.html

[T42] Perl：变量类型
来源：http://hz.andypj.xyz/gthhrmnpuv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.wangdashe.top/gtcdpwijpq.html

[T43] Perl：字符串插值
来源：http://hz.zhixingplan.top/gtdoenhupn.html

"值: $a"
来源：http://hz.dianchejie.cn/gtbentupam.html

[T44] Perl：条件
来源：http://hz.guannengcc.top/gtwptbzuuq.html

if ($a > 0) { print "正"; }
来源：http://hz.chenlongwang.top/gtxnbnshyk.html

[T45] Perl：数组遍历
来源：http://hz.kuanghao11.cn/gtjdrvmyqd.html

for my $x (@arr) { print $x; }
来源：http://hz.daxiang520.top/gtjezkdfbw.html

[T46] Perl：哈希操作
来源：http://hz.xingfuxueyuan.xyz/gtmlofogie.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yuanzhike.top/gtgjnxsnrt.html

[T47] Perl：正则捕获
来源：http://hz.nanxuanxn.top/gtfrktiosw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yvedp.cn/gtdmfwstsx.html

[T48] Perl：正则替换
来源：http://hz.tian-w.cn/gtdcfluewh.html

$s =~ s/old/new/g;
来源：http://hz.quarkkingdee.top/gtklydtjta.html

[T49] Perl：函数
来源：http://hz.yangfankeji.com/gtxogdilks.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.havefunace.top/gtbdebywaq.html

[T50] Perl：逐行读文件
来源：http://hz.jinqigufen.top/gtpikttnky.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jinqigufen.top/gtmuadqqbk.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yongpay.top/gtrggpqqdv.html

[T51] Scala：Hello World
来源：http://hz.iojbl.cn/gtrppnnrip.html

println("Hello")
来源：http://hz.nanxuanxn.top/gtwnhcjfro.html

[T52] Scala：变量
来源：http://hz.zhoulong.xyz/gtmupzdzeb.html

val a = 1;  var b = 2
来源：http://hz.sweek.top/gtxqyworac.html

[T53] Scala：字符串插值
来源：http://hz.tanke756.top/gtfjtfkave.html

s"值: $b"
来源：http://hz.jinyuanbaomall.cn/gtohtsmqhe.html

[T54] Scala：集合映射
来源：http://hz.bjfxy.top/gtnbpbwqqt.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.hammf.cn/gtfoednjut.html

[T55] Scala：集合过滤
来源：http://hz.chenlongwang.top/gtiwmvnbrn.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.cqqwz.cn/gtfsmvcrmj.html

[T56] Scala：样例类
来源：http://hz.havefunace.top/gtppswbwqh.html

case class User(name: String, age: Int)
来源：http://hz.quarkkingdee.top/gtleiuuqel.html

[T57] Scala：模式匹配
来源：http://hz.ydjk.org.cn/gtcgkodxey.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.tanke756.top/gthzhumeko.html

[T58] Scala：函数定义
来源：http://hz.xylfe.cn/gtoaayzvwq.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.gzhubu.top/gtskklqhdx.html

[T59] Scala：循环
来源：http://hz.zhiwuduotai.top/gtlxhupdnx.html

for (i <- 1 to 10) println(i)
来源：http://hz.jqgufenzy.top/gtcxallrrz.html

[T60] Scala：折叠
来源：http://hz.sufxvd.cn/gtchdinkgk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.nanxinkj.top/gtbyhaeaab.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtfpikuuvq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhengqikj.top/gtghfnuwba.html

================================================================================
来源：http://hz.ydzc1.top/gtgsgzchlm.html

[U01] Py：创建虚拟环境
来源：http://hz.ydjk.org.cn/gtqwtweyzu.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.aibaodan.cn/gtnjchkinh.html

[U02] Py：导出 / 安装依赖
来源：http://hz.gzhubu.top/gtvqvqjhmb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.haohaochexian.top/gtppuxsfhw.html

[U03] Py：加载 .env 配置
来源：http://hz.havefunace.top/gtumnamnxq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.xinyue.icu/gtrkkcsmwh.html

[U04] Py：变量调试打印
来源：http://hz.jiagoushi.top/gtdsjxklaw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.cheryme.top/gtmzhtjyql.html

[U05] Py：列表去重且保序
来源：http://hz.zhengqikj.top/gtkcyuxyxh.html

list(dict.fromkeys(arr))
来源：http://hz.zhengqikj.top/gtsodmskmb.html

[U06] Py：合并两个字典
来源：http://hz.xziqi.cn/gtqlxikdxz.html

{**a, **b}
来源：http://hz.9152youxi.cn/gtifntwrwy.html

[U07] Py：反转字典键值
来源：http://hz.cdnleiting.top/gthduyqhvj.html

{v: k for k, v in d.items()}
来源：http://hz.xingfuxueyuan.xyz/gthhsyvgmt.html

[U08] Py：展平二维列表
来源：http://hz.iojbl.cn/gtslrjvaoc.html

[y for x in nested for y in x]
来源：http://hz.gaohongyu789.top/gtufimsqjm.html

[U09] Py：字典取最大值的键
来源：http://hz.ydjk.org.cn/gtzjnxfvjg.html

max(d, key=d.get)
来源：http://hz.hysaishi.cn/gtsvpcnjpd.html

[U10] Py：按值排序字典
来源：http://hz.jinghuilouyu.cn/gtlbuyshep.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yueranfly.top/gtemjldrai.html

[U11] Py：生成器表达式
来源：http://hz.yvedp.cn/gtgxjnlqef.html

(x * 2 for x in arr)
来源：http://hz.jianghu66.top/gtvuvqtfry.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.ivvv.top/gtdvyxnrim.html

Counter(arr).most_common(3)
来源：http://hz.fzhhl.top/gtwuxduqpt.html

[U13] Py：固定长度队列
来源：http://hz.guannengcc.top/gtlkldhocs.html

deque(maxlen=10)
来源：http://hz.cheryme.top/gtouxxxfcp.html

[U14] Py：分组收集到列表
来源：http://hz.jiagoushi.top/gtbivzcvat.html

defaultdict(list)
来源：http://hz.hnxiangtu.top/gtoxwywwsi.html

[U15] Py：高精度计时
来源：http://hz.chenzaomai.com/gtbmszupuv.html

t = time.perf_counter()
来源：http://hz.meibo888.top/gtqiaqrsgd.html

[U16] Py：命令行参数解析
来源：http://hz.meibo888.top/gtdyedhsnz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.ppjwa.cn/gthwjukpfx.html

[U17] Py：初始化日志
来源：http://hz.shzxlz.cn/gtnjxlibsb.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.birdmap.top/gtryzhnpky.html

[U18] Py：预编译正则
来源：http://hz.shanyushiyangkeji.top/gthyhogbrk.html

pat = re.compile(r"\d+")
来源：http://hz.zhengqikj.top/gtlvhwsfwb.html

[U19] Py：正则替换带回调
来源：http://hz.zhixingplan.top/gtvybtlaqt.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yueranfly.top/gtjtglcfby.html

[U20] Py：缓存函数结果
来源：http://hz.feifeiyinyue.top/gtfwbqpeuj.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jinqigfzy.top/gtbaclptoh.html

[U21] Py：自定义上下文管理器
来源：http://hz.zhaomingkeji.xyz/gtlvyzgzde.html

@contextlib.contextmanager
来源：http://hz.yongpay.top/gtkuvpyers.html

[U22] Py：矩阵转置
来源：http://hz.tianlin.xyz/gtieadtrwk.html

list(zip(*m))
来源：http://hz.ppjwa.cn/gtvoxdtykv.html

[U23] Py：分块读取大文件
来源：http://hz.shanyushiyangtech.top/gtuosgsrva.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.0kj1m.cn/gtptytuhkz.html

[U24] Py：路径操作
来源：http://hz.hfpthk.cn/gtuxcgmwin.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.9152youxi.cn/gtiwrrwsti.html

[U25] Py：CSV 按字典读
来源：http://hz.zycfv.cn/gtgpewvzds.html

csv.DictReader(f)
来源：http://hz.xinyue.icu/gtrllpsuul.html

[U26] Py：并发下载
来源：http://hz.xylfe.cn/gtetbfieea.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.ivvv.top/gtxrqlbazy.html

[U27] Py：异步 HTTP
来源：http://hz.zhaomingkeji.xyz/gtuiqsqpez.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.xinyue.icu/gtpcuabjvn.html

[U28] Py：类型别名
来源：http://hz.haohaochexian.top/gtqojxuqwz.html

UserId = int
来源：http://hz.chenzaomai.com/gtudbqsnpi.html

[U29] Py：属性校验
来源：http://hz.jinyuanbaomall.cn/gtgecmdtvw.html

@property 与 @x.setter 配合
来源：http://hz.ybcxt.top/gthgcuqgvz.html

[U30] Py：数据类
来源：http://hz.hnqzz.top/gtstmrkwpf.html

@dataclass(slots=True)
来源：http://hz.vqdsnc.cn/gtvcyrrorn.html

[U31] Py：单测
来源：http://hz.xuanzx.com/gtnyczsyui.html

python -m pytest -q
来源：http://hz.kuanghao11.cn/gtuxdjpbiu.html

[U32] Py：代码格式化
来源：http://hz.xylfe.cn/gtolrcfibm.html

ruff format . && ruff check --fix .
来源：http://hz.aizwys.cn/gtcxqvjizj.html

[U33] Py：打包发布
来源：http://hz.fzhhl.top/gtimcvgnfu.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.yangfankeji.com/gtbchamgsq.html

[U34] Py：判断编码
来源：http://hz.tanke756.top/gtyyxezavq.html

chardet.detect(raw)
来源：http://hz.jyoumei.cn/gtgrldxlpx.html


<!-- 参考信息 -->