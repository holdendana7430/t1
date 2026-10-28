代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://hz.yj20258.top/gttkvddfbs.html

[S15] C：类型转换
来源：http://hz.yueranfly.top/gtwtmkwdqg.html

(double) a / b
来源：http://hz.tianlin.xyz/gtlatdtyrd.html

[S16] C：位操作置位
来源：http://hz.pengpengdd.cyou/gtytqrrpml.html

x |= (1 << 3);
来源：http://hz.yueranfly.top/gtaobamyww.html

[S17] C：安全拼接字符串
来源：http://hz.hywenlv.cn/gtxfhjrwbk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ivvv.top/gtvdpbcfez.html

[S18] C：命令行参数
来源：http://hz.jinghuilouyu.cn/gtvohzisti.html

int main(int argc, char **argv)
来源：http://hz.fengsongda.top/gttwjstnni.html

[S19] C：快速排序
来源：http://hz.xziqi.cn/gtpywrlojn.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.guannengcc.top/gtioeabqhx.html

[S20] C：二分查找
来源：http://hz.jinqigufen.top/gtwiqfwlab.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.wangshuangyany.cn/gtvvvquozo.html

[S21] C：字符类别判断
来源：http://hz.shzxlz.cn/gtfffdujew.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.316326.xyz/gtcoqqycpm.html

[S22] C：字符串转数字
来源：http://hz.redwolf501.top/gtyftxazbj.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yuxming.cn/gtwfepkvez.html

[S23] C：随机数
来源：http://hz.chenjidiqi.icu/gtfahexmwz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.feifeiyinyue.top/gtizxhhwcs.html

[S24] C：获取本地时间
来源：http://hz.sufxvd.cn/gtetnuwmhc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.gotoacloud.top/gtkhvzfiny.html

[S25] C：内存拷贝
来源：http://hz.mhx1999.top/gtlrpkobtu.html

memcpy(dst, src, n);
来源：http://hz.316326.xyz/gtlqoldhji.html

[S26] C：内存清零
来源：http://hz.jinqigufen.top/gtqfcsjker.html

memset(a, 0, sizeof a);
来源：http://hz.c1oappe.top/gtlhonvgqn.html

[S27] C：定义常量
来源：http://hz.pengpengdd.cyou/gtuchmbmky.html

const double PI = 3.14159;
来源：http://hz.birdmap.top/gtdvowkpam.html

[S28] C：静态变量
来源：http://hz.yj20258888.top/gtfxmktugd.html

static int counter = 0;
来源：http://hz.xziqi.cn/gtbzvicjdx.html

[S29] C：变参函数
来源：http://hz.ydzc1.top/gtyhylkmzb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cqqwz.cn/gtllrmtcvz.html

[S30] C：头文件保护
来源：http://hz.chenzaomai.com/gtvtwipudq.html

#ifndef X_H
来源：http://hz.haohaochexian.top/gtyhywmrmy.html

#define X_H
来源：http://hz.shanyushiyangtech.top/gtqgjhdtof.html

#endif
来源：http://hz.ppjwa.cn/gtmnmcoqvh.html

[S31] C++：Hello World
来源：http://hz.cdnleiting.top/gtngmoejmr.html

#include <iostream>
来源：http://hz.shangyingyoupin.top/gtnxnnelwv.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.wangshuangyany.cn/gtiwupynyw.html

[S32] C++：字符串
来源：http://hz.sysykeji.top/gtcifrrjwd.html

std::string s = "hi";  s += "!";
来源：http://hz.gogol.net.cn/gtyatxuqzv.html

[S33] C++：vector 增删
来源：http://hz.xuetiantiany.cn/gtefbfsnkq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.sweek.top/gtcmqndcdh.html

[S34] C++：遍历 vector
来源：http://hz.xingfuxueyuan.xyz/gtfysgvqff.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hammf.cn/gtolzvknlh.html

[S35] C++：map
来源：http://hz.tianlin.xyz/gtunjcohni.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shangyingyoupin.top/gtqnecbyjy.html

[S36] C++：unordered_map
来源：http://hz.ppjwa.cn/gtmpjpxwie.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shuidangran.top/gtiaejlieu.html

[S37] C++：set
来源：http://hz.ppjwa.cn/gtehubstvq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.nanxinkj.top/gtqkxecnjy.html

[S38] C++：排序
来源：http://hz.sweek.top/gtzvcbtcsq.html

std::sort(v.begin(), v.end());
来源：http://hz.xziqi.cn/gtjjbhernx.html

[S39] C++：自定义比较器排序
来源：http://hz.hammf.cn/gtgdienavn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.pengpengdd.cyou/gtvedubima.html

[S40] C++：查找元素
来源：http://hz.yanxiufei.cn/gthjvgyhxf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.ehwqpu.com/gtoyatvzxi.html

[S41] C++：类与构造函数
来源：http://hz.guannengcc.top/gtuapbsata.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yuxming.cn/gtapcqofce.html

[S42] C++：继承与虚函数
来源：http://hz.52xcode.cn/gtmpszgykj.html

class B : public Base { public: void f() override {} };
来源：http://hz.cheryme.top/gtafqeevse.html

[S43] C++：智能指针
来源：http://hz.jqgufenzy.top/gtyfljcooh.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhongyouzk.top/gtnsixbjga.html

[S44] C++：引用传参
来源：http://hz.andypj.xyz/gteegguimr.html

void inc(int &x) { ++x; }
来源：http://hz.fzhhl.top/gthfqwqcqh.html

[S45] C++：lambda
来源：http://hz.aizwys.cn/gttcdtdxmi.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yonumen.top/gtaapgjotc.html

[S46] C++：函数模板
来源：http://hz.ppjwa.cn/gtdiiquzgu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.aibaodan.cn/gtlpqeihgh.html

[S47] C++：结构化绑定遍历
来源：http://hz.kuanghao11.cn/gtxuxapdna.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.pengpengdd.cyou/gtsjfzdxwy.html

[S48] C++：逐行读文件
来源：http://hz.c1oappe.top/gtzbuxhhqq.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shanyushiyangtech.top/gttvkvdgwp.html

while (std::getline(in, line)) { }
来源：http://hz.sxryk.cn/gttwdabbow.html

[S49] C++：写文件
来源：http://hz.smart0.xyz/gtqceijfsm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.hnxiangtu.top/gtonmzxwkr.html

[S50] C++：格式化数字
来源：http://hz.daria6918.cn/gthuepsbqe.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yongpay.top/gtyewdywdx.html

[S51] C++：显式类型转换
来源：http://hz.aizwys.cn/gtjtnrhbba.html

static_cast<double>(a) / b
来源：http://hz.ybcxt.top/gtbdgtxnjf.html

[S52] C++：const 与 noexcept
来源：http://hz.hnqzz.top/gtiaihednv.html

int size() const noexcept { return n_; }
来源：http://hz.yangfankeji.com/gthrngoaob.html

[S53] C++：移动语义
来源：http://hz.xuanzx.com/gthcucciel.html

std::vector<int> w = std::move(v);
来源：http://hz.fzhhl.top/gtvgyxtqro.html

[S54] C++：异常处理
来源：http://hz.shangyingyoupin.top/gtgkoosdnj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zycfv.cn/gthvozsbqv.html

[S55] C++：结构化绑定
来源：http://hz.hammf.cn/gtwfsvhcck.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.chenzaomai.com/gthtnquujl.html

[S56] C++：optional
来源：http://hz.gaohongyu789.top/gtsxrbyoyv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jlsjyb.cn/gtjahibcgu.html

[S57] C++：编译期常量
来源：http://hz.ivvv.top/gtkgxrmmoi.html

constexpr int N = 10;
来源：http://hz.dianchejie.cn/gtisejcodg.html

[S58] C++：命名空间
来源：http://hz.fengsongda.top/gtnwylqddd.html

namespace ns { int f() { return 1; } }
来源：http://hz.svipenyu.cn/gtkayifxjb.html

[S59] C++：静态断言
来源：http://hz.yj20258.top/gtacdjnzex.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.redwolf501.top/gtqtagaugh.html

[S60] C++：遍历并删除元素
来源：http://hz.zhoulong.xyz/gtdpchhpry.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.c1oappe.top/gthiylccpk.html

================================================================================
来源：http://hz.yongpay.top/gtgdhjkoox.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jinyuanbaomall.cn/gtrdojrorl.html

================================================================================
来源：http://hz.gzhubu.top/gtrqybvhvl.html

[T01] Kotlin：Hello World
来源：http://hz.zhongyouzk.top/gtqmxkilcx.html

println("Hello")
来源：http://hz.sweek.top/gtjqcspuca.html

[T02] Kotlin：变量
来源：http://hz.hysaishi.cn/gtzopnjgol.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yj20258888.top/gtajrlzelc.html

[T03] Kotlin：字符串模板
来源：http://hz.chenzaomai.com/gtvbssiyvg.html

"值: $b"
来源：http://hz.redwolf501.top/gtudsdxmuf.html

[T04] Kotlin：空安全
来源：http://hz.chenlongwang.top/gtyxltfjzz.html

val n: String? = null;  n?.length
来源：http://hz.0kj1m.cn/gtrnnglnzx.html

[T05] Kotlin：when 表达式
来源：http://hz.gzhubu.top/gtfbiwkhlm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.hammf.cn/gtajnpcdcu.html

[T06] Kotlin：集合映射
来源：http://hz.zhijiandao.cn/gtzmhrelzh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.birdmap.top/gtxxduvtcy.html

[T07] Kotlin：集合过滤
来源：http://hz.52xcode.cn/gtavoruizd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yj202588.top/gtctnijrco.html

[T08] Kotlin：数据类
来源：http://hz.jinqigufen.top/gtvndgvdzp.html

data class User(val name: String, val age: Int)
来源：http://hz.xziqi.cn/gtyhgljyqo.html

[T09] Kotlin：扩展函数
来源：http://hz.zhaomingkeji.xyz/gtzgoxvacd.html

fun String.exclaim() = this + "!"
来源：http://hz.zhiwuduotai.top/gtcahfkymd.html

[T10] Kotlin：默认参数
来源：http://hz.tanke756.top/gtzxytwdlh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yvedp.cn/gtokduqzuy.html

[T11] Kotlin：协程
来源：http://hz.birdmap.top/gtratxwgei.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.guowangkeji.top/gtjfgbodpo.html

[T12] Kotlin：解构声明
来源：http://hz.jiagoushi.top/gtsetsozau.html

val (a, b) = Pair(1, 2)
来源：http://hz.hnxiangtu.top/gttqmeysbv.html

[T13] Kotlin：只读 Map
来源：http://hz.fzhhl.top/gtgvwzpbfn.html

val m = mapOf("a" to 1)
来源：http://hz.shzxlz.cn/gthkvjlrvq.html

[T14] Kotlin：循环
来源：http://hz.yangfankeji.com/gtfpbfqaph.html

for (i in 1..10) println(i)
来源：http://hz.yvedp.cn/gtgjjgcykt.html

[T15] Kotlin：接口
来源：http://hz.gotoacloud.top/gtoseokvwh.html

interface Shape { fun area(): Double }
来源：http://hz.zhiwuduotai.top/gtplvqfhre.html

[T16] Swift：Hello World
来源：http://hz.c1oappe.top/gtrjwqvsor.html

print("Hello")
来源：http://hz.cheryme.top/gtckneqshl.html

[T17] Swift：变量与常量
来源：http://hz.hammf.cn/gtfvxxkdhc.html

var a = 1;  let b = 2
来源：http://hz.haohaochexian.top/gtjnfmfnqa.html

[T18] Swift：字符串插值
来源：http://hz.hnxiangtu.top/gtzstspjtm.html

"值: \(b)"
来源：http://hz.hongshengwenyu.top/gtpuismlxf.html

[T19] Swift：可选绑定
来源：http://hz.andypj.xyz/gthrejzxvv.html

if let n = opt { print(n) }
来源：http://hz.meibo888.top/gthesecits.html

[T20] Swift：数组操作
来源：http://hz.yongpay.top/gthhuvlfou.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.9152youxi.cn/gtzgzxpblr.html

[T21] Swift：遍历
来源：http://hz.gzhubu.top/gtcebwengo.html

for x in a { print(x) }
来源：http://hz.cdnleiting.top/gtwcmehwck.html

[T22] Swift：字典
来源：http://hz.chenlongwang.top/gteduunwzn.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hfpthk.cn/gtuufsdtfk.html

[T23] Swift：函数
来源：http://hz.redwolf501.top/gtusbojfwk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.hywenlv.cn/gtbwxultsv.html

[T24] Swift：闭包
来源：http://hz.fzhhl.top/gtuywqwefu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.aizwys.cn/gtbuqhvdrz.html

[T25] Swift：结构体
来源：http://hz.guannengcc.top/gtjbmbefrq.html

struct P { var x: Int }
来源：http://hz.c1oappe.top/gtjqvprins.html

[T26] Swift：类与重写
来源：http://hz.ehwqpu.com/gtzgdibwht.html

class A: Base { override func f() {} }
来源：http://hz.ehwqpu.com/gtpvlrsgkc.html

[T27] Swift：错误处理
来源：http://hz.fengsongda.top/gtmpniqbtt.html

do { try f() } catch { print(error) }
来源：http://hz.daria6918.cn/gtmdawfjsd.html

[T28] Swift：枚举
来源：http://hz.hywenlv.cn/gtqpimvwap.html

enum Color { case red, green }
来源：http://hz.guowangkeji.top/gtuyojaqav.html

[T29] Swift：guard 提前返回
来源：http://hz.bjfxy.top/gtwiumowdy.html

guard let x = opt else { return }
来源：http://hz.jyoumei.cn/gtyijflfvx.html

[T30] Swift：协议
来源：http://hz.jlsjyb.cn/gtdeoolekt.html

protocol Shape { func area() -> Double }
来源：http://hz.yj202588.top/gttngueopx.html

[T31] Lua：Hello World
来源：http://hz.xylfe.cn/gtobmqylvt.html

print("Hello")
来源：http://hz.c1oappe.top/gtiluqzgvq.html

[T32] Lua：局部变量
来源：http://hz.xingfuxueyuan.xyz/gtlufyecpm.html

local a = 1
来源：http://hz.cqqwz.cn/gtzmtbyqvm.html

[T33] Lua：表（数组）
来源：http://hz.xuanzx.com/gtauxcxzib.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.birdmap.top/gtjpzpkahb.html

[T34] Lua：遍历表
来源：http://hz.jiagoushi.top/gtndssbyyp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.shuidangran.top/gtipdsvdge.html

[T35] Lua：字典表
来源：http://hz.xylfe.cn/gtttqfwrow.html

local d = { a = 1 };  d.b = 2
来源：http://hz.chenjidiqi.icu/gtiayhckia.html

[T36] Lua：函数
来源：http://hz.0kj1m.cn/gtqugfewtu.html

function add(a, b) return a + b end
来源：http://hz.c1oappe.top/gtexpctufg.html

[T37] Lua：字符串拼接
来源：http://hz.hnqzz.top/gteruorffk.html

"a" .. "b"
来源：http://hz.pycfn.com/gtkzvadqef.html

[T38] Lua：条件
来源：http://hz.zhoulong.xyz/gtkftbsprf.html

if x > 0 then print("正") end
来源：http://hz.svipenyu.cn/gtvhgxzdoy.html

[T39] Lua：模式匹配
来源：http://hz.xuanzx.com/gtrcbiagip.html

string.find(s, "%d+")
来源：http://hz.chenzaomai.com/gtpdyqlgtb.html

[T40] Lua：元表
来源：http://hz.jqgfzy.top/gtksuazpyg.html

setmetatable({}, { __index = base })
来源：http://hz.nanxinkj.top/gtlabamdwe.html

[T41] Perl：Hello World
来源：http://hz.chenzaomai.com/gtvsxxfivo.html

print "Hello\n";
来源：http://hz.ehwqpu.com/gtqrwzeume.html

[T42] Perl：变量类型
来源：http://hz.mhx1999.top/gtynvjysmk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.chenlongwang.top/gthjvezphx.html

[T43] Perl：字符串插值
来源：http://hz.hnxiangtu.top/gtjqajbajf.html

"值: $a"
来源：http://hz.xuanzx.com/gtulybuwql.html

[T44] Perl：条件
来源：http://hz.jqgfzy.top/gtzfqxqous.html

if ($a > 0) { print "正"; }
来源：http://hz.dianchejie.cn/gticrbggwm.html

[T45] Perl：数组遍历
来源：http://hz.aibaodan.cn/gtewdqjbvp.html

for my $x (@arr) { print $x; }
来源：http://hz.chenzaomai.com/gtoerdxdbt.html

[T46] Perl：哈希操作
来源：http://hz.guowangkeji.top/gtiixjnjme.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.dashuyun.cn/gtpxcdvlgv.html

[T47] Perl：正则捕获
来源：http://hz.birdmap.top/gtppnwbtcm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.feifeiyinyue.top/gtcrlkddfb.html

[T48] Perl：正则替换
来源：http://hz.aibaodan.cn/gtruihliks.html

$s =~ s/old/new/g;
来源：http://hz.smart0.xyz/gtdmhqofvz.html

[T49] Perl：函数
来源：http://hz.yueranfly.top/gtozqrzmxu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.cqqwz.cn/gtlryaobpb.html

[T50] Perl：逐行读文件
来源：http://hz.52xcode.cn/gtpmqawxwi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.chenjidiqi.icu/gtifqpzkyl.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yanxiufei.cn/gtmtiwijhr.html

[T51] Scala：Hello World
来源：http://hz.gzhubu.top/gtadgwaszn.html

println("Hello")
来源：http://hz.daxiang520.top/gtwzgtpopr.html

[T52] Scala：变量
来源：http://hz.snrcjt.cn/gtngyimekc.html

val a = 1;  var b = 2
来源：http://hz.iojbl.cn/gtxbfpwkva.html

[T53] Scala：字符串插值
来源：http://hz.zhiwuduotai.top/gtooqirkqt.html

s"值: $b"
来源：http://hz.smart0.xyz/gtllefkkve.html

[T54] Scala：集合映射
来源：http://hz.hysaishi.cn/gtianyvwwp.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.ppjwa.cn/gtmwghqfel.html

[T55] Scala：集合过滤
来源：http://hz.0kj1m.cn/gtmmetfvvs.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jqgfzy.top/gtfwxxfacs.html

[T56] Scala：样例类
来源：http://hz.yueranfly.top/gtobfvixck.html

case class User(name: String, age: Int)
来源：http://hz.yj20258.top/gtorlfemqf.html

[T57] Scala：模式匹配
来源：http://hz.quarkkingdee.top/gtbiwiwgah.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.fengsongda.top/gtvhxmible.html

[T58] Scala：函数定义
来源：http://hz.chenzaomai.com/gtrbqxnqqj.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.ppjwa.cn/gtrgapsgqu.html

[T59] Scala：循环
来源：http://hz.jqgufenzy.top/gtsngwskzl.html

for (i <- 1 to 10) println(i)
来源：http://hz.andypj.xyz/gtdngvpzsa.html

[T60] Scala：折叠
来源：http://hz.tianlin.xyz/gtyozroamn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.tanke756.top/gtmxtfzmsw.html

================================================================================
来源：http://hz.ehwqpu.com/gtopeswcmh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.nanxinkj.top/gtzptkdzwu.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtugetvziw.html

[U01] Py：创建虚拟环境
来源：http://hz.jinqigfzy.top/gtnrvdolmj.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yj202588.top/gtqjwplgko.html

[U02] Py：导出 / 安装依赖
来源：http://hz.yvedp.cn/gtxzazlhae.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.hnqzz.top/gtoummufrd.html

[U03] Py：加载 .env 配置
来源：http://hz.0kj1m.cn/gtvgntqfmf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.tian-w.cn/gterrmajop.html

[U04] Py：变量调试打印
来源：http://hz.guowangkeji.top/gtwuxjmuwi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.xylfe.cn/gtsctpcvrr.html

[U05] Py：列表去重且保序
来源：http://hz.birdmap.top/gtxqixcpsk.html

list(dict.fromkeys(arr))
来源：http://hz.ywan-chungtsiang.top/gtxtlgltvk.html

[U06] Py：合并两个字典
来源：http://hz.xinyue.icu/gtihkdwwpv.html

{**a, **b}
来源：http://hz.ppjwa.cn/gtkdgrvvdg.html

[U07] Py：反转字典键值
来源：http://hz.hfpthk.cn/gtrwafnwyg.html

{v: k for k, v in d.items()}
来源：http://hz.pengpengdd.cyou/gtipeunuif.html

[U08] Py：展平二维列表
来源：http://hz.cheryme.top/gtftixgxad.html

[y for x in nested for y in x]
来源：http://hz.52xcode.cn/gtcvsuhtim.html

[U09] Py：字典取最大值的键
来源：http://hz.cashguo.top/gthekruvai.html

max(d, key=d.get)
来源：http://hz.xingfuxueyuan.xyz/gtilufxjha.html

[U10] Py：按值排序字典
来源：http://hz.hongshengwenyu.top/gthygjrbes.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.gogol.net.cn/gtnltiejao.html

[U11] Py：生成器表达式
来源：http://hz.wangdashe.top/gtflynmfnp.html

(x * 2 for x in arr)
来源：http://hz.fzhhl.top/gttvmcczmd.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.ywan-chungtsiang.top/gtanmicwdd.html

Counter(arr).most_common(3)
来源：http://hz.ydzc1.top/gtvlkhlqqp.html

[U13] Py：固定长度队列
来源：http://hz.chenzaomai.com/gtqitlmosg.html

deque(maxlen=10)
来源：http://hz.xylfe.cn/gtmdbkxsub.html

[U14] Py：分组收集到列表
来源：http://hz.yonumen.top/gtioyetrnw.html

defaultdict(list)
来源：http://hz.tanke756.top/gtoponapfi.html

[U15] Py：高精度计时
来源：http://hz.ivvv.top/gtxetuivyk.html

t = time.perf_counter()
来源：http://hz.quarkkingdee.top/gthrlwfobn.html

[U16] Py：命令行参数解析
来源：http://hz.zhaomingkeji.xyz/gttdwuhjgp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.chenlongwang.top/gtsqqdxhdi.html

[U17] Py：初始化日志
来源：http://hz.birdmap.top/gtisrpcdvt.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.hysaishi.cn/gtjggvphlv.html

[U18] Py：预编译正则
来源：http://hz.ehwqpu.com/gtbgeerebb.html

pat = re.compile(r"\d+")
来源：http://hz.smart0.xyz/gtjthiydvb.html

[U19] Py：正则替换带回调
来源：http://hz.zhongyouzk.top/gtrvkzkzzc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.kuanghao11.cn/gtfdtpzczy.html

[U20] Py：缓存函数结果
来源：http://hz.sxryk.cn/gtnizxjosd.html

@functools.lru_cache(maxsize=None)
来源：http://hz.daxiang520.top/gtnhyikpdr.html

[U21] Py：自定义上下文管理器
来源：http://hz.zhaomingkeji.xyz/gtobjkpstb.html

@contextlib.contextmanager
来源：http://hz.dashuyun.cn/gtqdfstvyl.html

[U22] Py：矩阵转置
来源：http://hz.yj20258.top/gtdnlsvali.html

list(zip(*m))
来源：http://hz.quarkkingdee.top/gtkfztampg.html

[U23] Py：分块读取大文件
来源：http://hz.xylfe.cn/gtjwhatjhr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.wangdashe.top/gtflmaivyi.html

[U24] Py：路径操作
来源：http://hz.jqgfzy.top/gtyfmhnxej.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.yonumen.top/gtpwbjnimw.html

[U25] Py：CSV 按字典读
来源：http://hz.gotoacloud.top/gtqgovkfyc.html

csv.DictReader(f)
来源：http://hz.jinqigfzy.top/gtfnyctokh.html

[U26] Py：并发下载
来源：http://hz.yonumen.top/gtalyzzoco.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.sysykeji.top/gtgzfwcqmg.html

[U27] Py：异步 HTTP
来源：http://hz.yj20258.top/gtypbpnvjs.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.ydzc1.top/gtnablzevm.html

[U28] Py：类型别名
来源：http://hz.dashuyun.cn/gtnzgnybbr.html

UserId = int
来源：http://hz.guannengcc.top/gthognkimz.html

[U29] Py：属性校验
来源：http://hz.jinqigfzy.top/gtpuzokmki.html

@property 与 @x.setter 配合
来源：http://hz.xylfe.cn/gtapiuzmug.html

[U30] Py：数据类
来源：http://hz.hnxiangtu.top/gtusvbxjba.html

@dataclass(slots=True)
来源：http://hz.smart0.xyz/gtixrjunad.html

[U31] Py：单测
来源：http://hz.sufxvd.cn/gtgqifvybp.html

python -m pytest -q
来源：http://hz.jqgfzy.top/gtnlrmmcgn.html

[U32] Py：代码格式化
来源：http://hz.guowangkeji.top/gtdlbrhawl.html

ruff format . && ruff check --fix .
来源：http://hz.pycfn.com/gtyihstaye.html

[U33] Py：打包发布
来源：http://hz.hfpthk.cn/gtpfifpijf.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.xingfuxueyuan.xyz/gtlxmqvtut.html

[U34] Py：判断编码
来源：http://hz.ywan-chungtsiang.top/gtaalsrozh.html

chardet.detect(raw)
来源：http://hz.jinyuanbaomall.cn/gtpqrmwqpb.html

[U35] Py：发送邮件
来源：http://hz.chenjidiqi.icu/gthlvmkofw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.c1oappe.top/gtfevjvasx.html

[U36] Py：定时任务
来源：http://hz.hnxiangtu.top/gtnycoszip.html

schedule.every(10).minutes.do(job)
来源：http://hz.haohaochexian.top/gtofgfsflg.html

[U37] Py：读写 Excel
来源：http://hz.ydjk.org.cn/gtpajozhgb.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.9152youxi.cn/gttnkunejr.html

[U38] Py：获取脚本所在目录
来源：http://hz.cheryme.top/gtcmctokwl.html

Path(__file__).resolve().parent
来源：http://hz.sweek.top/gtharuftcc.html


<!-- 参考信息 -->