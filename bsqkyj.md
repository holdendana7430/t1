代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhijiandao.cn/gtarfpahwo.html

[S08] C：动态内存分配与释放
来源：http://hz.zhaomingkeji.xyz/gtjlhvuddp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.daxiang520.top/gtormwxzwa.html

[S09] C：结构体定义与初始化
来源：http://hz.sweek.top/gtcsnkqnly.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hnqzz.top/gtyqxwuzsz.html

[S10] C：指针与解引用
来源：http://hz.hywenlv.cn/gtoiriggpg.html

int *p = &a;  *p = 5;
来源：http://hz.yonumen.top/gtgraparuq.html

[S11] C：逐行读文件
来源：http://hz.zycfv.cn/gtzwftecwb.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.xuetiantiany.cn/gtfiknjopt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.guowangkeji.top/gtbzrdwuvt.html

fclose(f);
来源：http://hz.shangyingyoupin.top/gtimvyfxqe.html

[S12] C：写文件
来源：http://hz.cheryme.top/gtwiczvmmo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.daria6918.cn/gtwlonfxuu.html

[S13] C：宏定义
来源：http://hz.yuxming.cn/gtwnewcmgg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jinghuilouyu.cn/gtsshaogmg.html

[S14] C：枚举
来源：http://hz.316326.xyz/gtzrrqoogs.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhixingplan.top/gtfrrcvacp.html

[S15] C：类型转换
来源：http://hz.zhaomingkeji.xyz/gtzphsldfs.html

(double) a / b
来源：http://hz.hammf.cn/gtanhzoenu.html

[S16] C：位操作置位
来源：http://hz.daria6918.cn/gtxodcrrvv.html

x |= (1 << 3);
来源：http://hz.shzxlz.cn/gtkvxvphle.html

[S17] C：安全拼接字符串
来源：http://hz.haohaochexian.top/gtlhcwitia.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.pycfn.com/gtincgvepu.html

[S18] C：命令行参数
来源：http://hz.hammf.cn/gtkrceezqz.html

int main(int argc, char **argv)
来源：http://hz.tianlin.xyz/gtysevakbc.html

[S19] C：快速排序
来源：http://hz.ywan-chungtsiang.top/gtekuwwaet.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.tanke756.top/gtlkfdlwac.html

[S20] C：二分查找
来源：http://hz.guannengcc.top/gtrqsolwgz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.wangdashe.top/gtmskagjqk.html

[S21] C：字符类别判断
来源：http://hz.meibo888.top/gtznvgikea.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.gaohongyu789.top/gtncooufdu.html

[S22] C：字符串转数字
来源：http://hz.hammf.cn/gtxsykgcom.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.tianlin.xyz/gtyvdvwlxa.html

[S23] C：随机数
来源：http://hz.gogol.net.cn/gtkosolvbd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jqgufenzy.top/gttqzqybul.html

[S24] C：获取本地时间
来源：http://hz.jinghuilouyu.cn/gtfirwblhb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.dianchejie.cn/gtjpwdypzc.html

[S25] C：内存拷贝
来源：http://hz.ppjwa.cn/gtnyqzjpnn.html

memcpy(dst, src, n);
来源：http://hz.yj202588.top/gtyuybexwa.html

[S26] C：内存清零
来源：http://hz.hfpthk.cn/gtfcezqsqg.html

memset(a, 0, sizeof a);
来源：http://hz.52xcode.cn/gtnzkgkrxe.html

[S27] C：定义常量
来源：http://hz.hywenlv.cn/gtzdodwtol.html

const double PI = 3.14159;
来源：http://hz.nanxinkj.top/gtxvtdcbid.html

[S28] C：静态变量
来源：http://hz.ydzc1.top/gtopefguwn.html

static int counter = 0;
来源：http://hz.yueranfly.top/gteelatuom.html

[S29] C：变参函数
来源：http://hz.yanxiufei.cn/gtzjwdtzwo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.shanyushiyangtech.top/gtyrbvkcty.html

[S30] C：头文件保护
来源：http://hz.guannengcc.top/gtsywysbvf.html

#ifndef X_H
来源：http://hz.cqqwz.cn/gtgmanpfzi.html

#define X_H
来源：http://hz.jqgufenzy.top/gthghnaivi.html

#endif
来源：http://hz.yuanzhike.top/gthqicgrak.html

[S31] C++：Hello World
来源：http://hz.shangyingyoupin.top/gtnbfxtgti.html

#include <iostream>
来源：http://hz.zhiwuduotai.top/gtfjgrdyzd.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jlsjyb.cn/gtfdghffin.html

[S32] C++：字符串
来源：http://hz.zycfv.cn/gtciscpszr.html

std::string s = "hi";  s += "!";
来源：http://hz.xylfe.cn/gtqwztufck.html

[S33] C++：vector 增删
来源：http://hz.sufxvd.cn/gtdaoqspqf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shanyushiyangkeji.top/gthuittpwe.html

[S34] C++：遍历 vector
来源：http://hz.c1oappe.top/gthvyekwmd.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hysaishi.cn/gtbtcqualb.html

[S35] C++：map
来源：http://hz.wangdashe.top/gtqmhlbkro.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhijiandao.cn/gtmlbmnwrz.html

[S36] C++：unordered_map
来源：http://hz.smart0.xyz/gtlpbewfbd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.aizwys.cn/gttsdywlhu.html

[S37] C++：set
来源：http://hz.yj202588.top/gtulquaprm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.cucudq.cn/gthgbmomdp.html

[S38] C++：排序
来源：http://hz.yanxiufei.cn/gtwjfzqzmz.html

std::sort(v.begin(), v.end());
来源：http://hz.sweek.top/gtzbjimhjn.html

[S39] C++：自定义比较器排序
来源：http://hz.nanxinkj.top/gtjwrctzbz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yuxming.cn/gtyofyehwm.html

[S40] C++：查找元素
来源：http://hz.shanyushiyangtech.top/gtatwukory.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.havefunace.top/gtppfuuzlz.html

[S41] C++：类与构造函数
来源：http://hz.yanxiufei.cn/gtqmwekilk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yj20258.top/gtvnnufqix.html

[S42] C++：继承与虚函数
来源：http://hz.hysaishi.cn/gtdjqyucga.html

class B : public Base { public: void f() override {} };
来源：http://hz.ywan-chungtsiang.top/gtzbhxiopo.html

[S43] C++：智能指针
来源：http://hz.yangfankeji.com/gtvlcqgpnn.html

auto p = std::make_unique<int>(5);
来源：http://hz.shanyushiyangtech.top/gtseedbsrx.html

[S44] C++：引用传参
来源：http://hz.pengpengdd.cyou/gtksxurgeg.html

void inc(int &x) { ++x; }
来源：http://hz.yueranfly.top/gtzanjhifm.html

[S45] C++：lambda
来源：http://hz.zhijiandao.cn/gtctfwahmk.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.nanxuanxn.top/gtjlryfcuh.html

[S46] C++：函数模板
来源：http://hz.tanke756.top/gtwvwswigf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.andypj.xyz/gthpzxlwrp.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhoulong.xyz/gtkdiyqdnk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.shzxlz.cn/gtgnuroztr.html

[S48] C++：逐行读文件
来源：http://hz.xinyue.icu/gtvsixnrcz.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.svipenyu.cn/gtuggjruyx.html

while (std::getline(in, line)) { }
来源：http://hz.mhx1999.top/gtbrtsyqeq.html

[S49] C++：写文件
来源：http://hz.iojbl.cn/gtpgzmkfmb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yueranfly.top/gtwahxledi.html

[S50] C++：格式化数字
来源：http://hz.snrcjt.cn/gtnhiajzqz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hfpthk.cn/gtvbtkbmcq.html

[S51] C++：显式类型转换
来源：http://hz.aizwys.cn/gtjlfbvijj.html

static_cast<double>(a) / b
来源：http://hz.yongpay.top/gthvdfosek.html

[S52] C++：const 与 noexcept
来源：http://hz.pycfn.com/gtrnubralc.html

int size() const noexcept { return n_; }
来源：http://hz.quarkkingdee.top/gtftsqifxb.html

[S53] C++：移动语义
来源：http://hz.xylfe.cn/gtwgtwtqeb.html

std::vector<int> w = std::move(v);
来源：http://hz.sysykeji.top/gtvglsrgzd.html

[S54] C++：异常处理
来源：http://hz.daria6918.cn/gtakusoptp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.xuanzx.com/gtuwbjjpcf.html

[S55] C++：结构化绑定
来源：http://hz.jyoumei.cn/gtlrbsgayh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.quarkkingdee.top/gtnkvodzqh.html

[S56] C++：optional
来源：http://hz.yuanzhike.top/gtygvkbtke.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.9152youxi.cn/gtmewaokbn.html

[S57] C++：编译期常量
来源：http://hz.iojbl.cn/gtjqgypjce.html

constexpr int N = 10;
来源：http://hz.nwbrower.top/gtexnvuucp.html

[S58] C++：命名空间
来源：http://hz.ydzc1.top/gtpdaojcfl.html

namespace ns { int f() { return 1; } }
来源：http://hz.fzhhl.top/gtwzdyeyow.html

[S59] C++：静态断言
来源：http://hz.ppjwa.cn/gtgyxrnshy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yvedp.cn/gttflnllak.html

[S60] C++：遍历并删除元素
来源：http://hz.meibo888.top/gtyaurejha.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.pycfn.com/gtlaaoaovg.html

================================================================================
来源：http://hz.nwbrower.top/gtehymcbsp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.bjfxy.top/gtgtkdjuzi.html

================================================================================
来源：http://hz.yvedp.cn/gtsrllebvv.html

[T01] Kotlin：Hello World
来源：http://hz.smart0.xyz/gtzygvreil.html

println("Hello")
来源：http://hz.zycfv.cn/gteemddymd.html

[T02] Kotlin：变量
来源：http://hz.52xcode.cn/gtigzxpnki.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yuanzhike.top/gtmfpdeyib.html

[T03] Kotlin：字符串模板
来源：http://hz.fzhhl.top/gtzwpphwoq.html

"值: $b"
来源：http://hz.wangdashe.top/gtfpruvcra.html

[T04] Kotlin：空安全
来源：http://hz.vqdsnc.cn/gthnupkswg.html

val n: String? = null;  n?.length
来源：http://hz.svipenyu.cn/gtdezvedru.html

[T05] Kotlin：when 表达式
来源：http://hz.feifeiyinyue.top/gtmlthoyjw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.wangdashe.top/gtoqompizv.html

[T06] Kotlin：集合映射
来源：http://hz.yangfankeji.com/gtahmjkcuy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.haohaochexian.top/gtiajppdnr.html

[T07] Kotlin：集合过滤
来源：http://hz.hongshengwenyu.top/gtcxmuaubk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.wangshuangyany.cn/gtenvvujjw.html

[T08] Kotlin：数据类
来源：http://hz.shzxlz.cn/gtvokhzmfx.html

data class User(val name: String, val age: Int)
来源：http://hz.guannengcc.top/gtgxjnukar.html

[T09] Kotlin：扩展函数
来源：http://hz.nanxinkj.top/gtxqdlvpob.html

fun String.exclaim() = this + "!"
来源：http://hz.zhiwuduotai.top/gtgpkbikpc.html

[T10] Kotlin：默认参数
来源：http://hz.zhaomingkeji.xyz/gtvguzhjcc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.nanxuanxn.top/gtcedqoaau.html

[T11] Kotlin：协程
来源：http://hz.chenlongwang.top/gttqdikpck.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yj20258.top/gtudhywhkg.html

[T12] Kotlin：解构声明
来源：http://hz.ybcxt.top/gtuglzlumh.html

val (a, b) = Pair(1, 2)
来源：http://hz.zycfv.cn/gtojzsusrq.html

[T13] Kotlin：只读 Map
来源：http://hz.ybcxt.top/gtqvcskvrn.html

val m = mapOf("a" to 1)
来源：http://hz.dianchejie.cn/gtrehhhoak.html

[T14] Kotlin：循环
来源：http://hz.zhiwuduotai.top/gtmvacfiae.html

for (i in 1..10) println(i)
来源：http://hz.zhiwuduotai.top/gtxanwctgs.html

[T15] Kotlin：接口
来源：http://hz.snrcjt.cn/gtsimembix.html

interface Shape { fun area(): Double }
来源：http://hz.ydjk.org.cn/gtvbvfsmlk.html

[T16] Swift：Hello World
来源：http://hz.yanxiufei.cn/gttxmnwzqt.html

print("Hello")
来源：http://hz.andypj.xyz/gtoqxnwpcl.html

[T17] Swift：变量与常量
来源：http://hz.chenlongwang.top/gtrirkglwn.html

var a = 1;  let b = 2
来源：http://hz.yvedp.cn/gtmmyvydpw.html

[T18] Swift：字符串插值
来源：http://hz.fengsongda.top/gtemefjwjh.html

"值: \(b)"
来源：http://hz.zhiwuduotai.top/gthmyihwxa.html

[T19] Swift：可选绑定
来源：http://hz.zhaomingkeji.xyz/gtfpsjtnlm.html

if let n = opt { print(n) }
来源：http://hz.fengsongda.top/gtgqekktfi.html

[T20] Swift：数组操作
来源：http://hz.yongpay.top/gtjoxtrfjt.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yvedp.cn/gtqipnably.html

[T21] Swift：遍历
来源：http://hz.zhongyouzk.top/gtqfgiufav.html

for x in a { print(x) }
来源：http://hz.shanyushiyangkeji.top/gtsszkynbx.html

[T22] Swift：字典
来源：http://hz.jinghuilouyu.cn/gtnqsyjbfj.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yangfankeji.com/gtterrzphd.html

[T23] Swift：函数
来源：http://hz.feifeiyinyue.top/gtitdqtolp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.xuanzx.com/gtzvmkelve.html

[T24] Swift：闭包
来源：http://hz.gogol.net.cn/gtnoeyunpz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.sxryk.cn/gtjcptogvr.html

[T25] Swift：结构体
来源：http://hz.yonumen.top/gtwhtutgal.html

struct P { var x: Int }
来源：http://hz.chenjidiqi.icu/gtpxqblgze.html

[T26] Swift：类与重写
来源：http://hz.zhoulong.xyz/gtjzpnluqd.html

class A: Base { override func f() {} }
来源：http://hz.hammf.cn/gtohxbtbdl.html

[T27] Swift：错误处理
来源：http://hz.chenlongwang.top/gtjgocbmqq.html

do { try f() } catch { print(error) }
来源：http://hz.cashguo.top/gtaejzamdj.html

[T28] Swift：枚举
来源：http://hz.9152youxi.cn/gthipbpnhe.html

enum Color { case red, green }
来源：http://hz.quarkkingdee.top/gtbcuxsvbp.html

[T29] Swift：guard 提前返回
来源：http://hz.ybcxt.top/gttokoxjka.html

guard let x = opt else { return }
来源：http://hz.zhengqikj.top/gtvdqgkblg.html

[T30] Swift：协议
来源：http://hz.316326.xyz/gtirzaoebt.html

protocol Shape { func area() -> Double }
来源：http://hz.smart0.xyz/gtullagwjj.html

[T31] Lua：Hello World
来源：http://hz.hnxiangtu.top/gthfaoivpv.html

print("Hello")
来源：http://hz.sysykeji.top/gtyhzetytd.html

[T32] Lua：局部变量
来源：http://hz.bjfxy.top/gtnpiopppn.html

local a = 1
来源：http://hz.tanke756.top/gtjhehqskf.html

[T33] Lua：表（数组）
来源：http://hz.quarkkingdee.top/gtxusosxyx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.ywan-chungtsiang.top/gtosdqiuyg.html

[T34] Lua：遍历表
来源：http://hz.mhx1999.top/gtdzpgixqk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.wangdashe.top/gtqraiziai.html

[T35] Lua：字典表
来源：http://hz.zhongyouzk.top/gttjtadnlq.html

local d = { a = 1 };  d.b = 2
来源：http://hz.cheryme.top/gtrunekqko.html

[T36] Lua：函数
来源：http://hz.dianchejie.cn/gtckahpfzh.html

function add(a, b) return a + b end
来源：http://hz.cucudq.cn/gteaoqmkrx.html

[T37] Lua：字符串拼接
来源：http://hz.yj202588.top/gtdvclxqkm.html

"a" .. "b"
来源：http://hz.c1oappe.top/gtavvsypfp.html

[T38] Lua：条件
来源：http://hz.cashguo.top/gtobugtidl.html

if x > 0 then print("正") end
来源：http://hz.shzxlz.cn/gtcwvtxzyf.html

[T39] Lua：模式匹配
来源：http://hz.0kj1m.cn/gtpgcsphem.html

string.find(s, "%d+")
来源：http://hz.shanyushiyangkeji.top/gtpynxipux.html

[T40] Lua：元表
来源：http://hz.yangfankeji.com/gtxuzdoeot.html

setmetatable({}, { __index = base })
来源：http://hz.yj20258.top/gtrnrniske.html

[T41] Perl：Hello World
来源：http://hz.hongshengwenyu.top/gtzmyqqsek.html

print "Hello\n";
来源：http://hz.chenlongwang.top/gtptbvvphu.html

[T42] Perl：变量类型
来源：http://hz.shuidangran.top/gtvwyqklix.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.hongshengwenyu.top/gtbdmadvfh.html

[T43] Perl：字符串插值
来源：http://hz.hongshengwenyu.top/gtpptrubdy.html

"值: $a"
来源：http://hz.havefunace.top/gtjmioexzd.html

[T44] Perl：条件
来源：http://hz.xylfe.cn/gtgzzcltkh.html

if ($a > 0) { print "正"; }
来源：http://hz.hysaishi.cn/gthsyighrp.html

[T45] Perl：数组遍历
来源：http://hz.nwbrower.top/gtzufnxetn.html

for my $x (@arr) { print $x; }
来源：http://hz.wangdashe.top/gtrqdowpjk.html

[T46] Perl：哈希操作
来源：http://hz.hnxiangtu.top/gtvqvrqsvh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jinyuanbaomall.cn/gtymojkhyg.html

[T47] Perl：正则捕获
来源：http://hz.cucudq.cn/gtyavpdjib.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.nwbrower.top/gttvpdmvzp.html

[T48] Perl：正则替换
来源：http://hz.cucudq.cn/gtsnhojavi.html

$s =~ s/old/new/g;
来源：http://hz.cheryme.top/gtmnxrohgp.html

[T49] Perl：函数
来源：http://hz.yj202588.top/gtkkarnyum.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jianghu66.top/gtbnksjtdi.html

[T50] Perl：逐行读文件
来源：http://hz.tanke756.top/gtzlqvsypn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.bjfxy.top/gtnttxkonc.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yj20258888.top/gtoeyjtjbw.html

[T51] Scala：Hello World
来源：http://hz.yuanzhike.top/gtuypdagze.html

println("Hello")
来源：http://hz.xinyue.icu/gtxpoewsne.html

[T52] Scala：变量
来源：http://hz.gotoacloud.top/gtbkuivsjg.html

val a = 1;  var b = 2
来源：http://hz.9152youxi.cn/gtxcchpsrn.html

[T53] Scala：字符串插值
来源：http://hz.xuetiantiany.cn/gtypuyvefo.html

s"值: $b"
来源：http://hz.gotoacloud.top/gtfcnchqny.html

[T54] Scala：集合映射
来源：http://hz.dashuyun.cn/gtjurypuzt.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.chenzaomai.com/gtqhzucwiv.html

[T55] Scala：集合过滤
来源：http://hz.jyoumei.cn/gtprvpbrga.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.ehwqpu.com/gtufyogcfa.html

[T56] Scala：样例类
来源：http://hz.cashguo.top/gtwehdtfdw.html

case class User(name: String, age: Int)
来源：http://hz.redwolf501.top/gtlxgqhviy.html

[T57] Scala：模式匹配
来源：http://hz.dashuyun.cn/gthdsurdkb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.wangdashe.top/gttuugsykt.html

[T58] Scala：函数定义
来源：http://hz.cucudq.cn/gterqtnyzr.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.cdnleiting.top/gtfnckgrxy.html

[T59] Scala：循环
来源：http://hz.tian-w.cn/gtaczfylhq.html

for (i <- 1 to 10) println(i)
来源：http://hz.daria6918.cn/gtrmgdslbx.html

[T60] Scala：折叠
来源：http://hz.ydjk.org.cn/gtyvbakfuz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.xziqi.cn/gthhxovsyj.html

================================================================================
来源：http://hz.hammf.cn/gtuofsjfqo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhongyouzk.top/gtfpsyjykx.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtyzbrpyfj.html

[U01] Py：创建虚拟环境
来源：http://hz.yuxming.cn/gthpzdvubw.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.ydjk.org.cn/gtpfctrqdo.html

[U02] Py：导出 / 安装依赖
来源：http://hz.chenzaomai.com/gteetykhdy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.tanke756.top/gtjwbclfwh.html

[U03] Py：加载 .env 配置
来源：http://hz.yangfankeji.com/gtybiyzpdn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yj20258888.top/gtrrorkbtt.html

[U04] Py：变量调试打印
来源：http://hz.yj20258.top/gtkpsycsmb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jiagoushi.top/gtdtanbpgz.html

[U05] Py：列表去重且保序
来源：http://hz.9152youxi.cn/gtgdgikowq.html

list(dict.fromkeys(arr))
来源：http://hz.hammf.cn/gtlqplpnwn.html

[U06] Py：合并两个字典
来源：http://hz.xingfuxueyuan.xyz/gtfxcgxiah.html

{**a, **b}
来源：http://hz.aibaodan.cn/gtztiivdad.html

[U07] Py：反转字典键值
来源：http://hz.havefunace.top/gtvxcwwfar.html

{v: k for k, v in d.items()}
来源：http://hz.ybcxt.top/gtzaedqjxv.html

[U08] Py：展平二维列表
来源：http://hz.jiagoushi.top/gthteubjgi.html

[y for x in nested for y in x]
来源：http://hz.hnqzz.top/gtpzwhrmfd.html

[U09] Py：字典取最大值的键
来源：http://hz.gzhubu.top/gtjqohcwiz.html

max(d, key=d.get)
来源：http://hz.meibo888.top/gtenzvicrb.html

[U10] Py：按值排序字典
来源：http://hz.havefunace.top/gtmldkymta.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yj202588.top/gtwdwfbgjp.html

[U11] Py：生成器表达式
来源：http://hz.52xcode.cn/gthtjoyway.html

(x * 2 for x in arr)
来源：http://hz.kuanghao11.cn/gtqrdfguhi.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.mhx1999.top/gtrhconqfa.html

Counter(arr).most_common(3)
来源：http://hz.9152youxi.cn/gtfbtdclry.html

[U13] Py：固定长度队列
来源：http://hz.jiagoushi.top/gthlnxawbm.html

deque(maxlen=10)
来源：http://hz.yanxiufei.cn/gtkmvevljy.html

[U14] Py：分组收集到列表
来源：http://hz.iojbl.cn/gtsppifrdk.html

defaultdict(list)
来源：http://hz.feifeiyinyue.top/gtunrfzxsq.html

[U15] Py：高精度计时
来源：http://hz.daxiang520.top/gtajqxysdc.html

t = time.perf_counter()
来源：http://hz.mhx1999.top/gtfdokumcl.html

[U16] Py：命令行参数解析
来源：http://hz.wangdashe.top/gtihvcnkqz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.gzhubu.top/gtimnivbpb.html

[U17] Py：初始化日志
来源：http://hz.sufxvd.cn/gtmgrwvohi.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.ydjk.org.cn/gtccnpaeor.html

[U18] Py：预编译正则
来源：http://hz.316326.xyz/gtmqnhfdup.html

pat = re.compile(r"\d+")
来源：http://hz.sufxvd.cn/gtcariqpjl.html

[U19] Py：正则替换带回调
来源：http://hz.wangdashe.top/gtoetizdcj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.shangyingyoupin.top/gtxaqypsoj.html

[U20] Py：缓存函数结果
来源：http://hz.jinghuilouyu.cn/gtbjcpyrny.html

@functools.lru_cache(maxsize=None)
来源：http://hz.hnxiangtu.top/gtbfvlaxsx.html

[U21] Py：自定义上下文管理器
来源：http://hz.meibo888.top/gtbynxqcfv.html

@contextlib.contextmanager
来源：http://hz.316326.xyz/gtabfjgeby.html

[U22] Py：矩阵转置
来源：http://hz.mhx1999.top/gtnfhlwfds.html

list(zip(*m))
来源：http://hz.ywan-chungtsiang.top/gtbakgngbv.html

[U23] Py：分块读取大文件
来源：http://hz.hammf.cn/gtobavgymz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.hnqzz.top/gtcvtqhuhy.html

[U24] Py：路径操作
来源：http://hz.jianghu66.top/gtzmjggaug.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.snrcjt.cn/gtgqkdwyhu.html

[U25] Py：CSV 按字典读
来源：http://hz.yanxiufei.cn/gtonpnisdv.html

csv.DictReader(f)
来源：http://hz.cucudq.cn/gtntktghho.html

[U26] Py：并发下载
来源：http://hz.xylfe.cn/gtkclwwxsr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.zhengqikj.top/gtwrbqgoyj.html

[U27] Py：异步 HTTP
来源：http://hz.ydjk.org.cn/gtjroeyuzv.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.yongpay.top/gtvraddgwo.html

[U28] Py：类型别名
来源：http://hz.tian-w.cn/gtefyozfli.html

UserId = int
来源：http://hz.cqqwz.cn/gtosbtbecz.html

[U29] Py：属性校验
来源：http://hz.vqdsnc.cn/gtgbngfwyt.html

@property 与 @x.setter 配合
来源：http://hz.nanxinkj.top/gtznhrblzu.html

[U30] Py：数据类
来源：http://hz.yonumen.top/gtgejrcboo.html

@dataclass(slots=True)
来源：http://hz.ivvv.top/gtrvfnlcax.html


<!-- 参考信息 -->