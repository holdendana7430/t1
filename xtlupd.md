代发 wailian999

strlen(s)
来源：http://hz.nanxuanxn.top/gtixikybhj.html

[S06] C：字符串比较
来源：http://hz.jlsjyb.cn/gtpifzbjtd.html

strcmp(a, b) == 0
来源：http://hz.zycfv.cn/gtodywbnlh.html

[S07] C：数组遍历求和
来源：http://hz.xziqi.cn/gttpvtltaa.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.dashuyun.cn/gtkchzetke.html

[S08] C：动态内存分配与释放
来源：http://hz.ivvv.top/gtublfvcfw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.redwolf501.top/gtjrrbiows.html

[S09] C：结构体定义与初始化
来源：http://hz.nwbrower.top/gtjcmxezuh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xziqi.cn/gtqegqnfxm.html

[S10] C：指针与解引用
来源：http://hz.zhongyouzk.top/gtoojvamai.html

int *p = &a;  *p = 5;
来源：http://hz.yvedp.cn/gtqjvcvokh.html

[S11] C：逐行读文件
来源：http://hz.xuetiantiany.cn/gtlligmljr.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ppjwa.cn/gtsllybpbu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.tian-w.cn/gtpgoedaul.html

fclose(f);
来源：http://hz.guannengcc.top/gttltypwgo.html

[S12] C：写文件
来源：http://hz.sweek.top/gtymkduvll.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.daxiang520.top/gtyfbdpwtf.html

[S13] C：宏定义
来源：http://hz.snrcjt.cn/gtagalvrlr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jinqigufen.top/gthqsqvigy.html

[S14] C：枚举
来源：http://hz.wangdashe.top/gtnpmeaxwz.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.feifeiyinyue.top/gtlkrsbrtv.html

[S15] C：类型转换
来源：http://hz.nanxinkj.top/gtgjevlhbb.html

(double) a / b
来源：http://hz.fzhhl.top/gtktafwmpv.html

[S16] C：位操作置位
来源：http://hz.hfpthk.cn/gtnsljqeed.html

x |= (1 << 3);
来源：http://hz.yonumen.top/gtngtwdujg.html

[S17] C：安全拼接字符串
来源：http://hz.guannengcc.top/gtvsdtzjgu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.redwolf501.top/gtmhxgpxmm.html

[S18] C：命令行参数
来源：http://hz.yongpay.top/gtdwfgtbnf.html

int main(int argc, char **argv)
来源：http://hz.ppjwa.cn/gtwhrkstap.html

[S19] C：快速排序
来源：http://hz.bjfxy.top/gtbduszdob.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.nwbrower.top/gtedvhqzdz.html

[S20] C：二分查找
来源：http://hz.jqgfzy.top/gtbfoptubr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.feifeiyinyue.top/gtgdgysmgz.html

[S21] C：字符类别判断
来源：http://hz.pycfn.com/gthjdndzxy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.pengpengdd.cyou/gtvxpycowe.html

[S22] C：字符串转数字
来源：http://hz.xinyue.icu/gtwjdpkqzs.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.guannengcc.top/gtjbyanzpc.html

[S23] C：随机数
来源：http://hz.gogol.net.cn/gtdrtqibyh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.haohaochexian.top/gtncvlyuut.html

[S24] C：获取本地时间
来源：http://hz.dianchejie.cn/gtqmrgtzja.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yuanzhike.top/gtsctcfath.html

[S25] C：内存拷贝
来源：http://hz.jinghuilouyu.cn/gtqqzbvxtd.html

memcpy(dst, src, n);
来源：http://hz.tian-w.cn/gtavdwxzdi.html

[S26] C：内存清零
来源：http://hz.redwolf501.top/gtyihlhlab.html

memset(a, 0, sizeof a);
来源：http://hz.aizwys.cn/gtqrfzwzib.html

[S27] C：定义常量
来源：http://hz.zhiwuduotai.top/gtvfbcantq.html

const double PI = 3.14159;
来源：http://hz.zhoulong.xyz/gtaqnbzqgz.html

[S28] C：静态变量
来源：http://hz.mhx1999.top/gttfnxzfov.html

static int counter = 0;
来源：http://hz.svipenyu.cn/gtaxafcctm.html

[S29] C：变参函数
来源：http://hz.yueranfly.top/gthirtdfvd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hnxiangtu.top/gtgnkqqrlr.html

[S30] C：头文件保护
来源：http://hz.9152youxi.cn/gtpyxyrwlm.html

#ifndef X_H
来源：http://hz.svipenyu.cn/gttczgbtur.html

#define X_H
来源：http://hz.ivvv.top/gtbgbqxvfo.html

#endif
来源：http://hz.yuanzhike.top/gtrrliryfo.html

[S31] C++：Hello World
来源：http://hz.wangdashe.top/gtmfsyziuq.html

#include <iostream>
来源：http://hz.chenjidiqi.icu/gtjeosnlui.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.gotoacloud.top/gtxnlmgpaf.html

[S32] C++：字符串
来源：http://hz.hammf.cn/gtooupbwds.html

std::string s = "hi";  s += "!";
来源：http://hz.snrcjt.cn/gtnvwenqtm.html

[S33] C++：vector 增删
来源：http://hz.birdmap.top/gtwnwmhosd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zhaomingkeji.xyz/gtbwltwcyf.html

[S34] C++：遍历 vector
来源：http://hz.ydzc1.top/gtjdesufrb.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.sxryk.cn/gtjdjxbnyk.html

[S35] C++：map
来源：http://hz.yanxiufei.cn/gtldnoktuw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ydjk.org.cn/gtpmghtcdj.html

[S36] C++：unordered_map
来源：http://hz.sysykeji.top/gtlgykqbot.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.bjfxy.top/gtpicbgmfn.html

[S37] C++：set
来源：http://hz.yangfankeji.com/gtdpclaeim.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yuxming.cn/gtfwfjlilq.html

[S38] C++：排序
来源：http://hz.havefunace.top/gtkhrhasve.html

std::sort(v.begin(), v.end());
来源：http://hz.hfpthk.cn/gttamamzox.html

[S39] C++：自定义比较器排序
来源：http://hz.aibaodan.cn/gtkpfcipzh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.fzhhl.top/gtdvtjnkle.html

[S40] C++：查找元素
来源：http://hz.svipenyu.cn/gtlvlgzwdd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yuxming.cn/gtameicjll.html

[S41] C++：类与构造函数
来源：http://hz.hysaishi.cn/gtvhniascb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.snrcjt.cn/gtczolmmgl.html

[S42] C++：继承与虚函数
来源：http://hz.hammf.cn/gthlhicsgb.html

class B : public Base { public: void f() override {} };
来源：http://hz.sysykeji.top/gtwvxforox.html

[S43] C++：智能指针
来源：http://hz.c1oappe.top/gtncwufmuc.html

auto p = std::make_unique<int>(5);
来源：http://hz.chenlongwang.top/gtdoyihchi.html

[S44] C++：引用传参
来源：http://hz.hnqzz.top/gtdmppvouz.html

void inc(int &x) { ++x; }
来源：http://hz.birdmap.top/gtaopwkmga.html

[S45] C++：lambda
来源：http://hz.gogol.net.cn/gtbmvtjlnl.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.tianlin.xyz/gtumsjhuho.html

[S46] C++：函数模板
来源：http://hz.fzhhl.top/gtxtqqypfq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yuxming.cn/gthbajswpq.html

[S47] C++：结构化绑定遍历
来源：http://hz.jqgfzy.top/gtolkcvdos.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yueranfly.top/gteofhgaiw.html

[S48] C++：逐行读文件
来源：http://hz.fengsongda.top/gtujbzzumw.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.gaohongyu789.top/gtnpmvypdn.html

while (std::getline(in, line)) { }
来源：http://hz.yuxming.cn/gtmhuqykot.html

[S49] C++：写文件
来源：http://hz.hnxiangtu.top/gtlmzimkiv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jqgfzy.top/gtoskrufyd.html

[S50] C++：格式化数字
来源：http://hz.fzhhl.top/gtnlrwtydx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.daxiang520.top/gttxbhmdlc.html

[S51] C++：显式类型转换
来源：http://hz.mhx1999.top/gtckxmodqs.html

static_cast<double>(a) / b
来源：http://hz.zhiwuduotai.top/gtxlcogqwx.html

[S52] C++：const 与 noexcept
来源：http://hz.jinqigufen.top/gtwgqmdmhd.html

int size() const noexcept { return n_; }
来源：http://hz.yanxiufei.cn/gtcdxjwkjs.html

[S53] C++：移动语义
来源：http://hz.fengsongda.top/gtaalxduyz.html

std::vector<int> w = std::move(v);
来源：http://hz.tanke756.top/gtdzksqslg.html

[S54] C++：异常处理
来源：http://hz.hammf.cn/gtgsodxhij.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.smart0.xyz/gtkhxlgzrl.html

[S55] C++：结构化绑定
来源：http://hz.zhaomingkeji.xyz/gtrhkbdlbs.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yvedp.cn/gtnjpjngau.html

[S56] C++：optional
来源：http://hz.vqdsnc.cn/gttsoarafp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.birdmap.top/gtinlvvzwt.html

[S57] C++：编译期常量
来源：http://hz.jinqigfzy.top/gtxkjjagqj.html

constexpr int N = 10;
来源：http://hz.hnqzz.top/gtejnrxxid.html

[S58] C++：命名空间
来源：http://hz.jyoumei.cn/gtegxhrmmv.html

namespace ns { int f() { return 1; } }
来源：http://hz.yvedp.cn/gtwsvbegez.html

[S59] C++：静态断言
来源：http://hz.smart0.xyz/gtafqevnjv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zhengqikj.top/gtmsmorinx.html

[S60] C++：遍历并删除元素
来源：http://hz.svipenyu.cn/gtysjrdzvs.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yj202588.top/gtujtymybw.html

================================================================================
来源：http://hz.hywenlv.cn/gtxxpzwgjg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.pengpengdd.cyou/gttddyysry.html

================================================================================
来源：http://hz.yvedp.cn/gtgjtqufct.html

[T01] Kotlin：Hello World
来源：http://hz.smart0.xyz/gtsquzsvqf.html

println("Hello")
来源：http://hz.aizwys.cn/gtpwxmomyo.html

[T02] Kotlin：变量
来源：http://hz.svipenyu.cn/gtvjccnyzj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hywenlv.cn/gtqlnvmlfs.html

[T03] Kotlin：字符串模板
来源：http://hz.xinyue.icu/gtjjcynoii.html

"值: $b"
来源：http://hz.tanke756.top/gtztljqmnw.html

[T04] Kotlin：空安全
来源：http://hz.tianlin.xyz/gtxsaahpnu.html

val n: String? = null;  n?.length
来源：http://hz.ybcxt.top/gtxuqbkcyo.html

[T05] Kotlin：when 表达式
来源：http://hz.0kj1m.cn/gtomcbphci.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.gaohongyu789.top/gtlipbudpu.html

[T06] Kotlin：集合映射
来源：http://hz.fengsongda.top/gtjlglbidn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jianghu66.top/gtwmshdiyy.html

[T07] Kotlin：集合过滤
来源：http://hz.shzxlz.cn/gtryxqushw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.ydzc1.top/gtbtfpuvpl.html

[T08] Kotlin：数据类
来源：http://hz.jinghuilouyu.cn/gtuvpwdtjr.html

data class User(val name: String, val age: Int)
来源：http://hz.jiagoushi.top/gthhbmrdxd.html

[T09] Kotlin：扩展函数
来源：http://hz.havefunace.top/gtyhvifacw.html

fun String.exclaim() = this + "!"
来源：http://hz.yueranfly.top/gtblxjtxck.html

[T10] Kotlin：默认参数
来源：http://hz.yvedp.cn/gtosggjrnk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.shangyingyoupin.top/gtowvlrhfu.html

[T11] Kotlin：协程
来源：http://hz.zdqjudy.top/gtpwnjbrrj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.gogol.net.cn/gtrvrgoguf.html

[T12] Kotlin：解构声明
来源：http://hz.yangfankeji.com/gtauomkiax.html

val (a, b) = Pair(1, 2)
来源：http://hz.xylfe.cn/gtkqhvaxgw.html

[T13] Kotlin：只读 Map
来源：http://hz.cheryme.top/gtgvvjtmmq.html

val m = mapOf("a" to 1)
来源：http://hz.xylfe.cn/gtbfvyrgim.html

[T14] Kotlin：循环
来源：http://hz.nanxinkj.top/gtttjjfuiw.html

for (i in 1..10) println(i)
来源：http://hz.cqqwz.cn/gtxmdsmdre.html

[T15] Kotlin：接口
来源：http://hz.316326.xyz/gthylebmze.html

interface Shape { fun area(): Double }
来源：http://hz.pycfn.com/gtfudzuvau.html

[T16] Swift：Hello World
来源：http://hz.daxiang520.top/gtpieukqrz.html

print("Hello")
来源：http://hz.chenjidiqi.icu/gttcskftdy.html

[T17] Swift：变量与常量
来源：http://hz.meibo888.top/gtgrpccqof.html

var a = 1;  let b = 2
来源：http://hz.jinqigfzy.top/gtwocybvlc.html

[T18] Swift：字符串插值
来源：http://hz.daxiang520.top/gtaibqpfjs.html

"值: \(b)"
来源：http://hz.zhengqikj.top/gtknatbqjb.html

[T19] Swift：可选绑定
来源：http://hz.shuidangran.top/gttlynivsj.html

if let n = opt { print(n) }
来源：http://hz.haohaochexian.top/gtjowdddam.html

[T20] Swift：数组操作
来源：http://hz.daxiang520.top/gtafpdflmf.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.9152youxi.cn/gtugbxdqhm.html

[T21] Swift：遍历
来源：http://hz.nanxuanxn.top/gtvmqhcbbv.html

for x in a { print(x) }
来源：http://hz.hywenlv.cn/gthmdeercu.html

[T22] Swift：字典
来源：http://hz.pycfn.com/gtrkukgwzp.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.shangyingyoupin.top/gthhhxjzpm.html

[T23] Swift：函数
来源：http://hz.yonumen.top/gticdvdrmm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.shanyushiyangkeji.top/gtzfsxvviq.html

[T24] Swift：闭包
来源：http://hz.kuanghao11.cn/gtqsnglzoc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.chenjidiqi.icu/gtnhxolxof.html

[T25] Swift：结构体
来源：http://hz.haohaochexian.top/gtpkufddbq.html

struct P { var x: Int }
来源：http://hz.hnxiangtu.top/gtxgqbpbtm.html

[T26] Swift：类与重写
来源：http://hz.hfpthk.cn/gtabppznla.html

class A: Base { override func f() {} }
来源：http://hz.ehwqpu.com/gttbdueyff.html

[T27] Swift：错误处理
来源：http://hz.zhaomingkeji.xyz/gtiujknckd.html

do { try f() } catch { print(error) }
来源：http://hz.yuxming.cn/gtmyrwwwoo.html

[T28] Swift：枚举
来源：http://hz.birdmap.top/gtdhrxljgc.html

enum Color { case red, green }
来源：http://hz.pycfn.com/gtqmouzpet.html

[T29] Swift：guard 提前返回
来源：http://hz.gotoacloud.top/gtqtvhruvr.html

guard let x = opt else { return }
来源：http://hz.andypj.xyz/gtkbmtwvex.html

[T30] Swift：协议
来源：http://hz.tian-w.cn/gtdsdqmrki.html

protocol Shape { func area() -> Double }
来源：http://hz.sufxvd.cn/gtovhrmrci.html

[T31] Lua：Hello World
来源：http://hz.shuidangran.top/gtdylznlxg.html

print("Hello")
来源：http://hz.daxiang520.top/gtwzyszllm.html

[T32] Lua：局部变量
来源：http://hz.tian-w.cn/gtaxuczzol.html

local a = 1
来源：http://hz.jqgfzy.top/gtxwkmqlbo.html

[T33] Lua：表（数组）
来源：http://hz.chenzaomai.com/gtgmcuassj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.andypj.xyz/gtwddgdmzw.html

[T34] Lua：遍历表
来源：http://hz.wangshuangyany.cn/gtctvcoxfy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.sweek.top/gtxzhldowh.html

[T35] Lua：字典表
来源：http://hz.cashguo.top/gtstqnerso.html

local d = { a = 1 };  d.b = 2
来源：http://hz.daria6918.cn/gtfgkhxhpl.html

[T36] Lua：函数
来源：http://hz.gaohongyu789.top/gtjjroaokb.html

function add(a, b) return a + b end
来源：http://hz.shuidangran.top/gtquoxegmj.html

[T37] Lua：字符串拼接
来源：http://hz.ydjk.org.cn/gtdrhcrwta.html

"a" .. "b"
来源：http://hz.shuidangran.top/gtcnqnsrtq.html

[T38] Lua：条件
来源：http://hz.tian-w.cn/gtiivyystl.html

if x > 0 then print("正") end
来源：http://hz.cqqwz.cn/gtydiodvoy.html

[T39] Lua：模式匹配
来源：http://hz.shuidangran.top/gtfyotdkaw.html

string.find(s, "%d+")
来源：http://hz.hywenlv.cn/gthjtyfbbg.html

[T40] Lua：元表
来源：http://hz.svipenyu.cn/gtdnpvxxqw.html

setmetatable({}, { __index = base })
来源：http://hz.ppjwa.cn/gtvawvjsgs.html

[T41] Perl：Hello World
来源：http://hz.fengsongda.top/gtoskejbks.html

print "Hello\n";
来源：http://hz.dashuyun.cn/gtmwheivvr.html

[T42] Perl：变量类型
来源：http://hz.ybcxt.top/gtpacvoosc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.chenzaomai.com/gttrjqiuch.html

[T43] Perl：字符串插值
来源：http://hz.feifeiyinyue.top/gtsyuhdfri.html

"值: $a"
来源：http://hz.shzxlz.cn/gtaennxhvn.html

[T44] Perl：条件
来源：http://hz.yj20258.top/gtuikzzfwv.html

if ($a > 0) { print "正"; }
来源：http://hz.bjfxy.top/gtnspjwasq.html

[T45] Perl：数组遍历
来源：http://hz.ehwqpu.com/gtfrxtqcjy.html

for my $x (@arr) { print $x; }
来源：http://hz.shangyingyoupin.top/gtkkuxrbvs.html

[T46] Perl：哈希操作
来源：http://hz.wangshuangyany.cn/gtdyiqudlg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zhiwuduotai.top/gtrstmlkvq.html

[T47] Perl：正则捕获
来源：http://hz.chenzaomai.com/gtldvkcwje.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.daria6918.cn/gtrodbeulu.html

[T48] Perl：正则替换
来源：http://hz.c1oappe.top/gttebwvtus.html

$s =~ s/old/new/g;
来源：http://hz.hysaishi.cn/gtpqktiyak.html

[T49] Perl：函数
来源：http://hz.yvedp.cn/gtxhaormdh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.c1oappe.top/gtdfvlirmg.html

[T50] Perl：逐行读文件
来源：http://hz.jinghuilouyu.cn/gtveehmfhw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.tianlin.xyz/gtkpwddojj.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.vqdsnc.cn/gtjdaymypp.html

[T51] Scala：Hello World
来源：http://hz.hywenlv.cn/gthrjzqxpq.html

println("Hello")
来源：http://hz.pycfn.com/gteoznlxbe.html

[T52] Scala：变量
来源：http://hz.hnqzz.top/gthfdjierg.html

val a = 1;  var b = 2
来源：http://hz.hysaishi.cn/gtuhthxyjo.html

[T53] Scala：字符串插值
来源：http://hz.aizwys.cn/gtsczmlqqz.html

s"值: $b"
来源：http://hz.cqqwz.cn/gtkclbtypb.html

[T54] Scala：集合映射
来源：http://hz.ybcxt.top/gtlykprubj.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.ydjk.org.cn/gtcbjgqiys.html

[T55] Scala：集合过滤
来源：http://hz.cqqwz.cn/gtisthiriq.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.havefunace.top/gtebdiricj.html

[T56] Scala：样例类
来源：http://hz.xziqi.cn/gtjywcqgft.html

case class User(name: String, age: Int)
来源：http://hz.guowangkeji.top/gtwtxaolfa.html

[T57] Scala：模式匹配
来源：http://hz.zhengqikj.top/gtokfxeeee.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hfpthk.cn/gtabrxwqdv.html

[T58] Scala：函数定义
来源：http://hz.xuanzx.com/gtlvkythpy.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.smart0.xyz/gtsxjhqbfl.html

[T59] Scala：循环
来源：http://hz.ivvv.top/gtqkzlrxhr.html

for (i <- 1 to 10) println(i)
来源：http://hz.52xcode.cn/gtfwmtdgvv.html

[T60] Scala：折叠
来源：http://hz.jinghuilouyu.cn/gtalsxwzhh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.nanxuanxn.top/gtnemjevng.html

================================================================================
来源：http://hz.haohaochexian.top/gtjcpojswz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.dashuyun.cn/gtniiqaywc.html

================================================================================
来源：http://hz.yongpay.top/gtnpdkqcsb.html

[U01] Py：创建虚拟环境
来源：http://hz.andypj.xyz/gtqhbvwiok.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yj20258.top/gtcumlhwbx.html

[U02] Py：导出 / 安装依赖
来源：http://hz.tanke756.top/gtqsrcwffd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.chenjidiqi.icu/gthltcvhli.html

[U03] Py：加载 .env 配置
来源：http://hz.yangfankeji.com/gtmwrcnubv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.andypj.xyz/gtztmvaece.html

[U04] Py：变量调试打印
来源：http://hz.ppjwa.cn/gtpxhnutpa.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jlsjyb.cn/gtdfjquowo.html

[U05] Py：列表去重且保序
来源：http://hz.hysaishi.cn/gtadnpqcpe.html

list(dict.fromkeys(arr))
来源：http://hz.haohaochexian.top/gtrdocapdb.html

[U06] Py：合并两个字典
来源：http://hz.zhiwuduotai.top/gtmugdwuem.html

{**a, **b}
来源：http://hz.meibo888.top/gtelqcawku.html

[U07] Py：反转字典键值
来源：http://hz.cdnleiting.top/gthlomvpyn.html

{v: k for k, v in d.items()}
来源：http://hz.jinqigfzy.top/gtrcevzhip.html

[U08] Py：展平二维列表
来源：http://hz.redwolf501.top/gtxzxddgfy.html

[y for x in nested for y in x]
来源：http://hz.jqgfzy.top/gtjksnghur.html

[U09] Py：字典取最大值的键
来源：http://hz.tian-w.cn/gthhyybanu.html

max(d, key=d.get)
来源：http://hz.xuetiantiany.cn/gtcfxapfeu.html

[U10] Py：按值排序字典
来源：http://hz.haohaochexian.top/gtunjkuzlv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.jlsjyb.cn/gtipwoctrl.html

[U11] Py：生成器表达式
来源：http://hz.jinqigfzy.top/gtqqwntanu.html

(x * 2 for x in arr)
来源：http://hz.gaohongyu789.top/gtxisascnn.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.jinghuilouyu.cn/gtxqgfqgrl.html

Counter(arr).most_common(3)
来源：http://hz.zdqjudy.top/gtrzisfjcm.html

[U13] Py：固定长度队列
来源：http://hz.xuanzx.com/gttdmxiwup.html

deque(maxlen=10)
来源：http://hz.tian-w.cn/gtkuvfqmxh.html

[U14] Py：分组收集到列表
来源：http://hz.sxryk.cn/gtbhqwellu.html

defaultdict(list)
来源：http://hz.cucudq.cn/gtcyfudtqg.html

[U15] Py：高精度计时
来源：http://hz.pengpengdd.cyou/gtuymegqar.html

t = time.perf_counter()
来源：http://hz.shuidangran.top/gtdawiuwqn.html

[U16] Py：命令行参数解析
来源：http://hz.nwbrower.top/gtoesmfips.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.zycfv.cn/gtqsnmdwuf.html

[U17] Py：初始化日志
来源：http://hz.vqdsnc.cn/gtdfszoggp.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.52xcode.cn/gtodvnnrko.html

[U18] Py：预编译正则
来源：http://hz.wangshuangyany.cn/gtdigoyieb.html

pat = re.compile(r"\d+")
来源：http://hz.xylfe.cn/gtlqqpnsis.html

[U19] Py：正则替换带回调
来源：http://hz.zhiwuduotai.top/gteiangmuy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yongpay.top/gtnqypgufz.html

[U20] Py：缓存函数结果
来源：http://hz.yuxming.cn/gtfwprsamb.html

@functools.lru_cache(maxsize=None)
来源：http://hz.hammf.cn/gtwidrbgeg.html

[U21] Py：自定义上下文管理器
来源：http://hz.yuxming.cn/gtgqscaiwe.html

@contextlib.contextmanager
来源：http://hz.shangyingyoupin.top/gtdhvedndf.html

[U22] Py：矩阵转置
来源：http://hz.zhixingplan.top/gtukoufing.html

list(zip(*m))
来源：http://hz.nwbrower.top/gtgrirrzqq.html

[U23] Py：分块读取大文件
来源：http://hz.9152youxi.cn/gtmgsgjtiz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.ppjwa.cn/gtehwbowwc.html

[U24] Py：路径操作
来源：http://hz.yangfankeji.com/gtnntqeafn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.xuetiantiany.cn/gtcraswxps.html

[U25] Py：CSV 按字典读
来源：http://hz.mhx1999.top/gtyepmsjhv.html

csv.DictReader(f)
来源：http://hz.jinyuanbaomall.cn/gtytmvukja.html

[U26] Py：并发下载
来源：http://hz.xinyue.icu/gtszhynonv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.nwbrower.top/gtlxevwdlk.html

[U27] Py：异步 HTTP
来源：http://hz.c1oappe.top/gtinpsosjp.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.shanyushiyangtech.top/gtqfgmqayj.html

[U28] Py：类型别名
来源：http://hz.316326.xyz/gtfjmifjfb.html

UserId = int
来源：http://hz.gotoacloud.top/gtwqajufrj.html


<!-- 参考信息 -->