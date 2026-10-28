代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ydjk.org.cn/gttydvgyqe.html

[S13] C：宏定义
来源：http://hz.jianghu66.top/gtehqsftxg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.fengsongda.top/gtykdcyhlh.html

[S14] C：枚举
来源：http://hz.havefunace.top/gtonatixce.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.quarkkingdee.top/gthtslehnn.html

[S15] C：类型转换
来源：http://hz.hywenlv.cn/gtowkkkvte.html

(double) a / b
来源：http://hz.hysaishi.cn/gtlxvhhxab.html

[S16] C：位操作置位
来源：http://hz.zycfv.cn/gtdpaltjbw.html

x |= (1 << 3);
来源：http://hz.guannengcc.top/gthpkqjzay.html

[S17] C：安全拼接字符串
来源：http://hz.meibo888.top/gtwdyozuom.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jianghu66.top/gtjueujnbp.html

[S18] C：命令行参数
来源：http://hz.kuanghao11.cn/gtbkjdemgl.html

int main(int argc, char **argv)
来源：http://hz.zhoulong.xyz/gtcatmseyw.html

[S19] C：快速排序
来源：http://hz.ydjk.org.cn/gteltlkiiy.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.daria6918.cn/gtcjymywsq.html

[S20] C：二分查找
来源：http://hz.jiagoushi.top/gtwucugzdc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.daria6918.cn/gtuhnvtznd.html

[S21] C：字符类别判断
来源：http://hz.wangshuangyany.cn/gtxlemllqw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.nwbrower.top/gtujpvjane.html

[S22] C：字符串转数字
来源：http://hz.bjfxy.top/gtvpvykpdm.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhongyouzk.top/gtekwmahlo.html

[S23] C：随机数
来源：http://hz.hongshengwenyu.top/gtwtkzjhkr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.guannengcc.top/gtsmtxrzvg.html

[S24] C：获取本地时间
来源：http://hz.jianghu66.top/gttkbgxqve.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yj20258888.top/gthmceidet.html

[S25] C：内存拷贝
来源：http://hz.zhongyouzk.top/gtstvbwout.html

memcpy(dst, src, n);
来源：http://hz.zhijiandao.cn/gtvzrltrog.html

[S26] C：内存清零
来源：http://hz.xuetiantiany.cn/gtrqnulrbo.html

memset(a, 0, sizeof a);
来源：http://hz.shzxlz.cn/gtcdbceiqy.html

[S27] C：定义常量
来源：http://hz.quarkkingdee.top/gtfvflnxqe.html

const double PI = 3.14159;
来源：http://hz.cashguo.top/gtamdzxxnn.html

[S28] C：静态变量
来源：http://hz.yonumen.top/gtmqosidwv.html

static int counter = 0;
来源：http://hz.yanxiufei.cn/gtqhdnudjv.html

[S29] C：变参函数
来源：http://hz.kuanghao11.cn/gtytsdnbpv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.guannengcc.top/gtaymovfeq.html

[S30] C：头文件保护
来源：http://hz.hnxiangtu.top/gtmhydklfr.html

#ifndef X_H
来源：http://hz.jlsjyb.cn/gtsejyfzdm.html

#define X_H
来源：http://hz.yangfankeji.com/gtwodzfkge.html

#endif
来源：http://hz.yanxiufei.cn/gtwmrcpxvc.html

[S31] C++：Hello World
来源：http://hz.xingfuxueyuan.xyz/gtsgpavpci.html

#include <iostream>
来源：http://hz.shanyushiyangkeji.top/gthhgnplxd.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.ivvv.top/gtiyjzksmr.html

[S32] C++：字符串
来源：http://hz.jinqigufen.top/gtelvjaynz.html

std::string s = "hi";  s += "!";
来源：http://hz.shanyushiyangtech.top/gtzkudcjud.html

[S33] C++：vector 增删
来源：http://hz.0kj1m.cn/gtnvekimnk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jyoumei.cn/gtcqboxoiy.html

[S34] C++：遍历 vector
来源：http://hz.yuxming.cn/gtprtroccq.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xuanzx.com/gtwjlalbgm.html

[S35] C++：map
来源：http://hz.yuanzhike.top/gtksahwphg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shzxlz.cn/gtskyzuagx.html

[S36] C++：unordered_map
来源：http://hz.wangshuangyany.cn/gtrxhesttl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinghuilouyu.cn/gtwdvdoodw.html

[S37] C++：set
来源：http://hz.birdmap.top/gtityymdvw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ppjwa.cn/gtfiqzprct.html

[S38] C++：排序
来源：http://hz.ehwqpu.com/gtuarlubni.html

std::sort(v.begin(), v.end());
来源：http://hz.nanxinkj.top/gtssjstcqg.html

[S39] C++：自定义比较器排序
来源：http://hz.birdmap.top/gtwbzzuntl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.cheryme.top/gtdubppjta.html

[S40] C++：查找元素
来源：http://hz.shzxlz.cn/gtlgexzqaw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.guowangkeji.top/gthiizsrsi.html

[S41] C++：类与构造函数
来源：http://hz.cucudq.cn/gtcytviwdr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.gotoacloud.top/gtqtprvbkx.html

[S42] C++：继承与虚函数
来源：http://hz.zhongyouzk.top/gtpjmuhhzq.html

class B : public Base { public: void f() override {} };
来源：http://hz.yj20258.top/gttwntcnse.html

[S43] C++：智能指针
来源：http://hz.guowangkeji.top/gtgozzotma.html

auto p = std::make_unique<int>(5);
来源：http://hz.wangshuangyany.cn/gteuenuczk.html

[S44] C++：引用传参
来源：http://hz.haohaochexian.top/gtffbkqhqq.html

void inc(int &x) { ++x; }
来源：http://hz.jqgufenzy.top/gtzxexyzrm.html

[S45] C++：lambda
来源：http://hz.daxiang520.top/gteopbsfyy.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yueranfly.top/gtkrhyvlpp.html

[S46] C++：函数模板
来源：http://hz.shzxlz.cn/gtirwxiram.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.0kj1m.cn/gttanupqpa.html

[S47] C++：结构化绑定遍历
来源：http://hz.daria6918.cn/gtkqghcvhn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.xziqi.cn/gtvonazamx.html

[S48] C++：逐行读文件
来源：http://hz.sufxvd.cn/gtqvblcrix.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.wangshuangyany.cn/gtfidyeprh.html

while (std::getline(in, line)) { }
来源：http://hz.nanxuanxn.top/gtwxbbjvqh.html

[S49] C++：写文件
来源：http://hz.ybcxt.top/gtfztdhprx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.svipenyu.cn/gtgmdcmwym.html

[S50] C++：格式化数字
来源：http://hz.zhijiandao.cn/gttpbdblmq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.gogol.net.cn/gteoaolvbk.html

[S51] C++：显式类型转换
来源：http://hz.yuxming.cn/gtgmsrdgxa.html

static_cast<double>(a) / b
来源：http://hz.xuanzx.com/gtixpwgkzk.html

[S52] C++：const 与 noexcept
来源：http://hz.nwbrower.top/gtmirgwsdw.html

int size() const noexcept { return n_; }
来源：http://hz.xziqi.cn/gtrahiimtw.html

[S53] C++：移动语义
来源：http://hz.zhengqikj.top/gtpjxurhpl.html

std::vector<int> w = std::move(v);
来源：http://hz.mhx1999.top/gtdkfzshek.html

[S54] C++：异常处理
来源：http://hz.nanxuanxn.top/gttawdncoj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.meibo888.top/gtxiumngwc.html

[S55] C++：结构化绑定
来源：http://hz.yonumen.top/gtyrlznwoe.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jinyuanbaomall.cn/gttrkiiydd.html

[S56] C++：optional
来源：http://hz.yonumen.top/gtyxgsfeut.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.daria6918.cn/gtqfdkbsqe.html

[S57] C++：编译期常量
来源：http://hz.sxryk.cn/gtougdcrxl.html

constexpr int N = 10;
来源：http://hz.shangyingyoupin.top/gtvgwidpks.html

[S58] C++：命名空间
来源：http://hz.9152youxi.cn/gtmjgdepaw.html

namespace ns { int f() { return 1; } }
来源：http://hz.birdmap.top/gtemtilldz.html

[S59] C++：静态断言
来源：http://hz.jinyuanbaomall.cn/gtcjfmvnap.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.meibo888.top/gttojmxyoj.html

[S60] C++：遍历并删除元素
来源：http://hz.jinqigufen.top/gtughuehlt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.chenlongwang.top/gtgaxslgfn.html

================================================================================
来源：http://hz.jiagoushi.top/gtzxpajiqq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.quarkkingdee.top/gtywshpdyt.html

================================================================================
来源：http://hz.gogol.net.cn/gtwwwindeu.html

[T01] Kotlin：Hello World
来源：http://hz.yueranfly.top/gtyofcswjo.html

println("Hello")
来源：http://hz.shanyushiyangkeji.top/gtkjqbqggo.html

[T02] Kotlin：变量
来源：http://hz.tianlin.xyz/gtpwqnqrij.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yongpay.top/gteitbbpis.html

[T03] Kotlin：字符串模板
来源：http://hz.cheryme.top/gtiymrisyr.html

"值: $b"
来源：http://hz.snrcjt.cn/gtxulabucj.html

[T04] Kotlin：空安全
来源：http://hz.cucudq.cn/gtbolbkuxs.html

val n: String? = null;  n?.length
来源：http://hz.yueranfly.top/gtypqreguu.html

[T05] Kotlin：when 表达式
来源：http://hz.xinyue.icu/gtsizfbsuq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.daria6918.cn/gtmwtgmtxq.html

[T06] Kotlin：集合映射
来源：http://hz.zhijiandao.cn/gtvmnjtemm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.xuetiantiany.cn/gtzatttncf.html

[T07] Kotlin：集合过滤
来源：http://hz.cucudq.cn/gtntuukoav.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.c1oappe.top/gtvvhigwra.html

[T08] Kotlin：数据类
来源：http://hz.pengpengdd.cyou/gtuomfovqc.html

data class User(val name: String, val age: Int)
来源：http://hz.yangfankeji.com/gtcwdcvizi.html

[T09] Kotlin：扩展函数
来源：http://hz.zhoulong.xyz/gtryfqnbxj.html

fun String.exclaim() = this + "!"
来源：http://hz.chenjidiqi.icu/gtgiulgdjk.html

[T10] Kotlin：默认参数
来源：http://hz.jlsjyb.cn/gtybhtqltn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hongshengwenyu.top/gtjaqwcbli.html

[T11] Kotlin：协程
来源：http://hz.nanxinkj.top/gtdtsgndki.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zhengqikj.top/gtgbreqszu.html

[T12] Kotlin：解构声明
来源：http://hz.gzhubu.top/gtqckikoah.html

val (a, b) = Pair(1, 2)
来源：http://hz.chenzaomai.com/gtsokororp.html

[T13] Kotlin：只读 Map
来源：http://hz.yanxiufei.cn/gtexnrwfdi.html

val m = mapOf("a" to 1)
来源：http://hz.tian-w.cn/gtuqdmuvog.html

[T14] Kotlin：循环
来源：http://hz.shuidangran.top/gtbjojzhfq.html

for (i in 1..10) println(i)
来源：http://hz.tanke756.top/gtybtqpmij.html

[T15] Kotlin：接口
来源：http://hz.birdmap.top/gtmyfhfvpe.html

interface Shape { fun area(): Double }
来源：http://hz.yanxiufei.cn/gtwgkvjmdo.html

[T16] Swift：Hello World
来源：http://hz.xuetiantiany.cn/gtmbhmnuuk.html

print("Hello")
来源：http://hz.chenzaomai.com/gtfklycvpb.html

[T17] Swift：变量与常量
来源：http://hz.zhoulong.xyz/gtxrqqhrko.html

var a = 1;  let b = 2
来源：http://hz.yanxiufei.cn/gthorgdfrr.html

[T18] Swift：字符串插值
来源：http://hz.guowangkeji.top/gtbsnxppiw.html

"值: \(b)"
来源：http://hz.xuanzx.com/gtkkwbipyd.html

[T19] Swift：可选绑定
来源：http://hz.haohaochexian.top/gtthihlkuk.html

if let n = opt { print(n) }
来源：http://hz.fzhhl.top/gtnfosdkeb.html

[T20] Swift：数组操作
来源：http://hz.gotoacloud.top/gtexuigxao.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.ivvv.top/gtaoluvoqh.html

[T21] Swift：遍历
来源：http://hz.aizwys.cn/gtgvboudwl.html

for x in a { print(x) }
来源：http://hz.hfpthk.cn/gtnujbqfsp.html

[T22] Swift：字典
来源：http://hz.hammf.cn/gtqzrhgrge.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ybcxt.top/gtnihlpzsw.html

[T23] Swift：函数
来源：http://hz.hnxiangtu.top/gtvmizimsx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.xuanzx.com/gtccgbwobr.html

[T24] Swift：闭包
来源：http://hz.tian-w.cn/gtorkbrwkd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.shuidangran.top/gtlwkyoupy.html

[T25] Swift：结构体
来源：http://hz.dianchejie.cn/gtecotxkuc.html

struct P { var x: Int }
来源：http://hz.zycfv.cn/gtcspgvvfg.html

[T26] Swift：类与重写
来源：http://hz.yuanzhike.top/gtrxbrlnei.html

class A: Base { override func f() {} }
来源：http://hz.zhixingplan.top/gtrqgikrjv.html

[T27] Swift：错误处理
来源：http://hz.jinqigfzy.top/gttysjvien.html

do { try f() } catch { print(error) }
来源：http://hz.hammf.cn/gtryecvkfh.html

[T28] Swift：枚举
来源：http://hz.zhaomingkeji.xyz/gtmkvktgam.html

enum Color { case red, green }
来源：http://hz.sxryk.cn/gtoibhcsrb.html

[T29] Swift：guard 提前返回
来源：http://hz.shuidangran.top/gtcrpnpigm.html

guard let x = opt else { return }
来源：http://hz.yonumen.top/gtmnvlfxen.html

[T30] Swift：协议
来源：http://hz.yanxiufei.cn/gtjutwjuqp.html

protocol Shape { func area() -> Double }
来源：http://hz.jinqigufen.top/gtsfeiovtk.html

[T31] Lua：Hello World
来源：http://hz.chenjidiqi.icu/gtmxiocrvh.html

print("Hello")
来源：http://hz.zhaomingkeji.xyz/gtwuogrczr.html

[T32] Lua：局部变量
来源：http://hz.hongshengwenyu.top/gttphcbcca.html

local a = 1
来源：http://hz.jlsjyb.cn/gtkgzgwbec.html

[T33] Lua：表（数组）
来源：http://hz.yangfankeji.com/gtvlkbqlzi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.pengpengdd.cyou/gtqcmhjawm.html

[T34] Lua：遍历表
来源：http://hz.xylfe.cn/gtgpvgjiov.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.shangyingyoupin.top/gtookwmszz.html

[T35] Lua：字典表
来源：http://hz.cdnleiting.top/gtnobrujzw.html

local d = { a = 1 };  d.b = 2
来源：http://hz.zycfv.cn/gtxqybqcbn.html

[T36] Lua：函数
来源：http://hz.gogol.net.cn/gtwgehgmvj.html

function add(a, b) return a + b end
来源：http://hz.redwolf501.top/gtkwxfxyvz.html

[T37] Lua：字符串拼接
来源：http://hz.yangfankeji.com/gtmlonvxfg.html

"a" .. "b"
来源：http://hz.jinyuanbaomall.cn/gtxqatzahh.html

[T38] Lua：条件
来源：http://hz.shuidangran.top/gtszbcusfj.html

if x > 0 then print("正") end
来源：http://hz.52xcode.cn/gtknlyjotq.html

[T39] Lua：模式匹配
来源：http://hz.shanyushiyangkeji.top/gtaqzsfydi.html

string.find(s, "%d+")
来源：http://hz.jianghu66.top/gtzqtjzapk.html

[T40] Lua：元表
来源：http://hz.havefunace.top/gtthyzbvsz.html

setmetatable({}, { __index = base })
来源：http://hz.andypj.xyz/gtlvybxbjd.html

[T41] Perl：Hello World
来源：http://hz.yuxming.cn/gtikqjiiml.html

print "Hello\n";
来源：http://hz.nanxinkj.top/gtoaariyqe.html

[T42] Perl：变量类型
来源：http://hz.ywan-chungtsiang.top/gtebkimzus.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yangfankeji.com/gttsxwgwwa.html

[T43] Perl：字符串插值
来源：http://hz.tianlin.xyz/gtvbltimpd.html

"值: $a"
来源：http://hz.nwbrower.top/gtwugnbjno.html

[T44] Perl：条件
来源：http://hz.9152youxi.cn/gtqzxibidp.html

if ($a > 0) { print "正"; }
来源：http://hz.jlsjyb.cn/gteuzhtddw.html

[T45] Perl：数组遍历
来源：http://hz.kuanghao11.cn/gtbiwnmcbp.html

for my $x (@arr) { print $x; }
来源：http://hz.xinyue.icu/gtponxrpqg.html

[T46] Perl：哈希操作
来源：http://hz.zhongyouzk.top/gtgghtjuum.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.chenlongwang.top/gthwhvzudx.html

[T47] Perl：正则捕获
来源：http://hz.gzhubu.top/gtvhlbftin.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jlsjyb.cn/gtszsqtanr.html

[T48] Perl：正则替换
来源：http://hz.fengsongda.top/gtnyuggahw.html

$s =~ s/old/new/g;
来源：http://hz.daxiang520.top/gtllyrwsix.html

[T49] Perl：函数
来源：http://hz.jinqigfzy.top/gtkuaxxmyg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.hammf.cn/gtwmnnflzk.html

[T50] Perl：逐行读文件
来源：http://hz.chenjidiqi.icu/gtlfkhshec.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.chenlongwang.top/gtymhwscgs.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.zhijiandao.cn/gtkcdrrhdt.html

[T51] Scala：Hello World
来源：http://hz.xylfe.cn/gtgqylbbjl.html

println("Hello")
来源：http://hz.havefunace.top/gtwfdvhbyn.html

[T52] Scala：变量
来源：http://hz.zdqjudy.top/gtewjovnvp.html

val a = 1;  var b = 2
来源：http://hz.hongshengwenyu.top/gtzbdyhift.html

[T53] Scala：字符串插值
来源：http://hz.hongshengwenyu.top/gtelhphzih.html

s"值: $b"
来源：http://hz.cdnleiting.top/gtwtosoghg.html

[T54] Scala：集合映射
来源：http://hz.ybcxt.top/gtfspdefqu.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.andypj.xyz/gtbqgvdnrh.html

[T55] Scala：集合过滤
来源：http://hz.feifeiyinyue.top/gtwtrdhpuc.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.dianchejie.cn/gtkyferdpf.html

[T56] Scala：样例类
来源：http://hz.0kj1m.cn/gterrduqtj.html

case class User(name: String, age: Int)
来源：http://hz.jinghuilouyu.cn/gthccietuh.html

[T57] Scala：模式匹配
来源：http://hz.c1oappe.top/gtkfwrmcyn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hnqzz.top/gtwyeazhvm.html

[T58] Scala：函数定义
来源：http://hz.pycfn.com/gttpvalnmz.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.gaohongyu789.top/gtmpiirmpr.html

[T59] Scala：循环
来源：http://hz.yj202588.top/gtxayymqfw.html

for (i <- 1 to 10) println(i)
来源：http://hz.xuetiantiany.cn/gthkckzbem.html

[T60] Scala：折叠
来源：http://hz.snrcjt.cn/gtjubivvmi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.xingfuxueyuan.xyz/gtympaufkg.html

================================================================================
来源：http://hz.yonumen.top/gtxksickjb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.cashguo.top/gtcbghkyqe.html

================================================================================
来源：http://hz.yanxiufei.cn/gtsxiizdqg.html

[U01] Py：创建虚拟环境
来源：http://hz.tanke756.top/gtobnqubea.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yuanzhike.top/gtbnqduuqm.html

[U02] Py：导出 / 安装依赖
来源：http://hz.xinyue.icu/gtxseoltun.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yuanzhike.top/gtydxvxmaw.html

[U03] Py：加载 .env 配置
来源：http://hz.jyoumei.cn/gtasuegfvx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.meibo888.top/gtqfcntebm.html

[U04] Py：变量调试打印
来源：http://hz.dashuyun.cn/gtdsjyacay.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.nanxinkj.top/gtzxnnktik.html

[U05] Py：列表去重且保序
来源：http://hz.sxryk.cn/gtsipcmfdi.html

list(dict.fromkeys(arr))
来源：http://hz.xinyue.icu/gtdcalquos.html

[U06] Py：合并两个字典
来源：http://hz.redwolf501.top/gtwvmxkhpo.html

{**a, **b}
来源：http://hz.gaohongyu789.top/gteoeyigqe.html

[U07] Py：反转字典键值
来源：http://hz.ehwqpu.com/gtknupimyj.html

{v: k for k, v in d.items()}
来源：http://hz.yj20258.top/gtkbctgfya.html

[U08] Py：展平二维列表
来源：http://hz.nanxuanxn.top/gtqdbvwspn.html

[y for x in nested for y in x]
来源：http://hz.c1oappe.top/gtmwszmejm.html

[U09] Py：字典取最大值的键
来源：http://hz.iojbl.cn/gthzxtlygz.html

max(d, key=d.get)
来源：http://hz.shangyingyoupin.top/gtvoiwgrnb.html

[U10] Py：按值排序字典
来源：http://hz.hywenlv.cn/gtgfxisiqy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yj20258.top/gtycsghlhn.html

[U11] Py：生成器表达式
来源：http://hz.316326.xyz/gtbrykufrh.html

(x * 2 for x in arr)
来源：http://hz.guannengcc.top/gtwzkvxjbj.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.ybcxt.top/gtbfogqmkd.html

Counter(arr).most_common(3)
来源：http://hz.guannengcc.top/gtpsefcrqx.html

[U13] Py：固定长度队列
来源：http://hz.jinghuilouyu.cn/gtsedkorws.html

deque(maxlen=10)
来源：http://hz.jqgufenzy.top/gtzwnjrngk.html

[U14] Py：分组收集到列表
来源：http://hz.hfpthk.cn/gtiqvlaksx.html

defaultdict(list)
来源：http://hz.hywenlv.cn/gtaykeftwf.html

[U15] Py：高精度计时
来源：http://hz.jinqigufen.top/gtnwjrywym.html

t = time.perf_counter()
来源：http://hz.gaohongyu789.top/gtnvkjcyiu.html

[U16] Py：命令行参数解析
来源：http://hz.jyoumei.cn/gtnhjjnfvx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jlsjyb.cn/gtyexkrbec.html

[U17] Py：初始化日志
来源：http://hz.redwolf501.top/gtoufrosir.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.ehwqpu.com/gtrtayncjo.html

[U18] Py：预编译正则
来源：http://hz.quarkkingdee.top/gtwbbndvup.html

pat = re.compile(r"\d+")
来源：http://hz.pycfn.com/gtalepfvrw.html

[U19] Py：正则替换带回调
来源：http://hz.yuxming.cn/gtqmjtyswp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.aizwys.cn/gtloachlsl.html

[U20] Py：缓存函数结果
来源：http://hz.zhijiandao.cn/gtudcndkjj.html

@functools.lru_cache(maxsize=None)
来源：http://hz.xylfe.cn/gtkgoaqjxw.html

[U21] Py：自定义上下文管理器
来源：http://hz.316326.xyz/gtqmpknvpi.html

@contextlib.contextmanager
来源：http://hz.xziqi.cn/gtycfpvsha.html

[U22] Py：矩阵转置
来源：http://hz.cheryme.top/gtxrwwxqme.html

list(zip(*m))
来源：http://hz.feifeiyinyue.top/gtfyiavawg.html

[U23] Py：分块读取大文件
来源：http://hz.nanxinkj.top/gtdqqnmttz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.bjfxy.top/gtejxmyjxl.html

[U24] Py：路径操作
来源：http://hz.sufxvd.cn/gtfheoxuqx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.jiagoushi.top/gtafpnhwcc.html

[U25] Py：CSV 按字典读
来源：http://hz.nanxinkj.top/gtakyuezvn.html

csv.DictReader(f)
来源：http://hz.shanyushiyangtech.top/gtqfrgucvz.html

[U26] Py：并发下载
来源：http://hz.xylfe.cn/gtrrqezsfk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.52xcode.cn/gtniykaozt.html

[U27] Py：异步 HTTP
来源：http://hz.havefunace.top/gtxuwjmyii.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.fzhhl.top/gthdabgezl.html

[U28] Py：类型别名
来源：http://hz.feifeiyinyue.top/gtkwhzqugw.html

UserId = int
来源：http://hz.xylfe.cn/gtxhhbpftn.html

[U29] Py：属性校验
来源：http://hz.redwolf501.top/gtsjbjvkkw.html

@property 与 @x.setter 配合
来源：http://hz.hammf.cn/gtcegdtrcp.html

[U30] Py：数据类
来源：http://hz.pycfn.com/gtvkeaiycr.html

@dataclass(slots=True)
来源：http://hz.zhiwuduotai.top/gtqsnnpuqe.html

[U31] Py：单测
来源：http://hz.hammf.cn/gtsgziicgl.html

python -m pytest -q
来源：http://hz.yvedp.cn/gtysqthmgd.html

[U32] Py：代码格式化
来源：http://hz.sweek.top/gtvmszxmqu.html

ruff format . && ruff check --fix .
来源：http://hz.jinqigufen.top/gtlvpfotrc.html

[U33] Py：打包发布
来源：http://hz.wangshuangyany.cn/gtmnsecqnd.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.cqqwz.cn/gtgmzdshyi.html

[U34] Py：判断编码
来源：http://hz.haohaochexian.top/gtrmclfjnq.html

chardet.detect(raw)
来源：http://hz.kuanghao11.cn/gtlghwbkbl.html

[U35] Py：发送邮件
来源：http://hz.kuanghao11.cn/gtrfthmgtq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.gzhubu.top/gtnxtwitzj.html

[U36] Py：定时任务
来源：http://hz.ywan-chungtsiang.top/gtoxunwjzc.html

schedule.every(10).minutes.do(job)
来源：http://hz.aibaodan.cn/gtrscfrotn.html


<!-- 参考信息 -->