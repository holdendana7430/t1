代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hnqzz.top/gtyqhtndrt.html

[S13] C：宏定义
来源：http://hz.hfpthk.cn/gtonxfyzte.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.havefunace.top/gtqdilvajx.html

[S14] C：枚举
来源：http://hz.fengsongda.top/gtlqonoxbr.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.sxryk.cn/gtwdpqbvbu.html

[S15] C：类型转换
来源：http://hz.zhoulong.xyz/gtpkcwkqyz.html

(double) a / b
来源：http://hz.mhx1999.top/gtxnitrkcy.html

[S16] C：位操作置位
来源：http://hz.xingfuxueyuan.xyz/gtkxxsblyq.html

x |= (1 << 3);
来源：http://hz.nwbrower.top/gtzedaably.html

[S17] C：安全拼接字符串
来源：http://hz.hnqzz.top/gtpktwsatd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yj202588.top/gtrgabyfst.html

[S18] C：命令行参数
来源：http://hz.svipenyu.cn/gtsoqqcjls.html

int main(int argc, char **argv)
来源：http://hz.yongpay.top/gtgjkijhnk.html

[S19] C：快速排序
来源：http://hz.bjfxy.top/gtfepgfhro.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.ybcxt.top/gtbyvttvfy.html

[S20] C：二分查找
来源：http://hz.hammf.cn/gttarysfbu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.andypj.xyz/gtcoetmjaq.html

[S21] C：字符类别判断
来源：http://hz.hfpthk.cn/gtglmsdvdo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yueranfly.top/gtoydqtncn.html

[S22] C：字符串转数字
来源：http://hz.shzxlz.cn/gtkzswmfuh.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.hammf.cn/gtdwhriswu.html

[S23] C：随机数
来源：http://hz.nanxinkj.top/gtxkklaxlw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhijiandao.cn/gtgljxudwk.html

[S24] C：获取本地时间
来源：http://hz.shzxlz.cn/gtzulbwmlm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.shanyushiyangtech.top/gtqpgmqjgb.html

[S25] C：内存拷贝
来源：http://hz.9152youxi.cn/gtjytewmur.html

memcpy(dst, src, n);
来源：http://hz.hammf.cn/gtxchbgsmg.html

[S26] C：内存清零
来源：http://hz.chenjidiqi.icu/gtsuqevrkj.html

memset(a, 0, sizeof a);
来源：http://hz.gotoacloud.top/gtotwcartt.html

[S27] C：定义常量
来源：http://hz.shzxlz.cn/gtsdknfmsl.html

const double PI = 3.14159;
来源：http://hz.zhijiandao.cn/gtndbxirpt.html

[S28] C：静态变量
来源：http://hz.gogol.net.cn/gtcqytvubv.html

static int counter = 0;
来源：http://hz.gzhubu.top/gtjkzbjlei.html

[S29] C：变参函数
来源：http://hz.pycfn.com/gtkhwtzxcy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.xuanzx.com/gtyzjomone.html

[S30] C：头文件保护
来源：http://hz.xinyue.icu/gtuduyygor.html

#ifndef X_H
来源：http://hz.xylfe.cn/gtywpgdqvy.html

#define X_H
来源：http://hz.zhengqikj.top/gtqhbiyugp.html

#endif
来源：http://hz.ydzc1.top/gtkvxvdqlq.html

[S31] C++：Hello World
来源：http://hz.gaohongyu789.top/gtjhjnvdbs.html

#include <iostream>
来源：http://hz.xinyue.icu/gtsihhcyxu.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zdqjudy.top/gtrnkskozz.html

[S32] C++：字符串
来源：http://hz.tanke756.top/gtcmlzatbt.html

std::string s = "hi";  s += "!";
来源：http://hz.jinqigfzy.top/gtrjjysqxe.html

[S33] C++：vector 增删
来源：http://hz.aizwys.cn/gtpxtfvsgx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.aibaodan.cn/gtcmopfsjr.html

[S34] C++：遍历 vector
来源：http://hz.yvedp.cn/gtjbgbojuh.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.sweek.top/gtrjrdbyzq.html

[S35] C++：map
来源：http://hz.sufxvd.cn/gtctooekkj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tian-w.cn/gtecomxfql.html

[S36] C++：unordered_map
来源：http://hz.ppjwa.cn/gtxtxpioom.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yuanzhike.top/gtpratqdia.html

[S37] C++：set
来源：http://hz.zhiwuduotai.top/gthzxvmzma.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.gzhubu.top/gtbyfoyapj.html

[S38] C++：排序
来源：http://hz.ybcxt.top/gtkiikgtxr.html

std::sort(v.begin(), v.end());
来源：http://hz.yj20258888.top/gtqhwbjnpo.html

[S39] C++：自定义比较器排序
来源：http://hz.ivvv.top/gtssyhyjtl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ppjwa.cn/gtijvhjotz.html

[S40] C++：查找元素
来源：http://hz.jlsjyb.cn/gtjrmfwhcj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hnqzz.top/gtxyajfvsa.html

[S41] C++：类与构造函数
来源：http://hz.shzxlz.cn/gtvhbvrtyl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.sufxvd.cn/gtlhouoeut.html

[S42] C++：继承与虚函数
来源：http://hz.xuanzx.com/gtrqhgspdm.html

class B : public Base { public: void f() override {} };
来源：http://hz.hongshengwenyu.top/gtmcwaggth.html

[S43] C++：智能指针
来源：http://hz.shangyingyoupin.top/gteioyxqbb.html

auto p = std::make_unique<int>(5);
来源：http://hz.9152youxi.cn/gtrqvwfcll.html

[S44] C++：引用传参
来源：http://hz.9152youxi.cn/gtxrryyycy.html

void inc(int &x) { ++x; }
来源：http://hz.yj20258.top/gtduiqhdkj.html

[S45] C++：lambda
来源：http://hz.andypj.xyz/gtzccdrgye.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.fengsongda.top/gtwkfagorr.html

[S46] C++：函数模板
来源：http://hz.hfpthk.cn/gtiatvnuvu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.wangdashe.top/gtnacpidyj.html

[S47] C++：结构化绑定遍历
来源：http://hz.shanyushiyangtech.top/gtgxuxldsd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.hnqzz.top/gtcentlnsa.html

[S48] C++：逐行读文件
来源：http://hz.dashuyun.cn/gtamipukce.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.52xcode.cn/gtusracugu.html

while (std::getline(in, line)) { }
来源：http://hz.yonumen.top/gtiauqcfzs.html

[S49] C++：写文件
来源：http://hz.ydzc1.top/gtcxczljjz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ydjk.org.cn/gtzbmgbplw.html

[S50] C++：格式化数字
来源：http://hz.havefunace.top/gtrurjqnhw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.fengsongda.top/gtqdutzjha.html

[S51] C++：显式类型转换
来源：http://hz.hywenlv.cn/gtdmlrdhdk.html

static_cast<double>(a) / b
来源：http://hz.jianghu66.top/gtcckuargw.html

[S52] C++：const 与 noexcept
来源：http://hz.yangfankeji.com/gtzqnokiea.html

int size() const noexcept { return n_; }
来源：http://hz.cashguo.top/gtizxitzpk.html

[S53] C++：移动语义
来源：http://hz.zhaomingkeji.xyz/gtkdzkfksu.html

std::vector<int> w = std::move(v);
来源：http://hz.gaohongyu789.top/gtrdtftxcb.html

[S54] C++：异常处理
来源：http://hz.nanxuanxn.top/gtpdoypbvm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.sxryk.cn/gtrzmojkpr.html

[S55] C++：结构化绑定
来源：http://hz.cheryme.top/gtsvrblnhw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.shuidangran.top/gtodkoezfm.html

[S56] C++：optional
来源：http://hz.zhongyouzk.top/gtvsdhhadp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hysaishi.cn/gtasenfwlv.html

[S57] C++：编译期常量
来源：http://hz.dashuyun.cn/gtxxpbvwef.html

constexpr int N = 10;
来源：http://hz.jqgfzy.top/gtazjrtyad.html

[S58] C++：命名空间
来源：http://hz.quarkkingdee.top/gtcdhicsco.html

namespace ns { int f() { return 1; } }
来源：http://hz.havefunace.top/gtkejznzms.html

[S59] C++：静态断言
来源：http://hz.9152youxi.cn/gtjfidrgey.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.c1oappe.top/gtqkbvipuk.html

[S60] C++：遍历并删除元素
来源：http://hz.cqqwz.cn/gtsijajvon.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.shanyushiyangkeji.top/gtecffbzax.html

================================================================================
来源：http://hz.sufxvd.cn/gtlbdovjqz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yueranfly.top/gtofweieet.html

================================================================================
来源：http://hz.ppjwa.cn/gtmhfkljfn.html

[T01] Kotlin：Hello World
来源：http://hz.hongshengwenyu.top/gtmgrqtucc.html

println("Hello")
来源：http://hz.zhaomingkeji.xyz/gtebcndvwy.html

[T02] Kotlin：变量
来源：http://hz.zhixingplan.top/gtsbeysbtu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jinqigfzy.top/gtsrabeobk.html

[T03] Kotlin：字符串模板
来源：http://hz.zhaomingkeji.xyz/gtgfwjkidy.html

"值: $b"
来源：http://hz.zhiwuduotai.top/gtstnxubut.html

[T04] Kotlin：空安全
来源：http://hz.ywan-chungtsiang.top/gtdxpumvvj.html

val n: String? = null;  n?.length
来源：http://hz.tanke756.top/gtzkyveuds.html

[T05] Kotlin：when 表达式
来源：http://hz.ppjwa.cn/gtpzfrlnpq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.svipenyu.cn/gtztprwtjf.html

[T06] Kotlin：集合映射
来源：http://hz.feifeiyinyue.top/gtlcpufgsj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.sysykeji.top/gtqomcaiio.html

[T07] Kotlin：集合过滤
来源：http://hz.hfpthk.cn/gttqvrsxyo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hysaishi.cn/gtrmlctnqj.html

[T08] Kotlin：数据类
来源：http://hz.hywenlv.cn/gticyysxep.html

data class User(val name: String, val age: Int)
来源：http://hz.ydjk.org.cn/gtcvkvpmnz.html

[T09] Kotlin：扩展函数
来源：http://hz.ywan-chungtsiang.top/gtyafbhbkd.html

fun String.exclaim() = this + "!"
来源：http://hz.xuetiantiany.cn/gtbaqxnzoa.html

[T10] Kotlin：默认参数
来源：http://hz.aizwys.cn/gtpgfqzxvf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jinyuanbaomall.cn/gtzdwoogzc.html

[T11] Kotlin：协程
来源：http://hz.0kj1m.cn/gtqtzxvnzt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jinyuanbaomall.cn/gtzlqtidml.html

[T12] Kotlin：解构声明
来源：http://hz.xinyue.icu/gthlrykwrh.html

val (a, b) = Pair(1, 2)
来源：http://hz.vqdsnc.cn/gtuvtrzhzj.html

[T13] Kotlin：只读 Map
来源：http://hz.sysykeji.top/gtrbuzuray.html

val m = mapOf("a" to 1)
来源：http://hz.bjfxy.top/gteitstvqr.html

[T14] Kotlin：循环
来源：http://hz.c1oappe.top/gtrsuvyquk.html

for (i in 1..10) println(i)
来源：http://hz.pengpengdd.cyou/gtgpnulcbu.html

[T15] Kotlin：接口
来源：http://hz.xuetiantiany.cn/gtsoskkooo.html

interface Shape { fun area(): Double }
来源：http://hz.shangyingyoupin.top/gtwcscnatx.html

[T16] Swift：Hello World
来源：http://hz.hnqzz.top/gtejeyudyy.html

print("Hello")
来源：http://hz.birdmap.top/gtcjhrjcww.html

[T17] Swift：变量与常量
来源：http://hz.nanxinkj.top/gtciqncizc.html

var a = 1;  let b = 2
来源：http://hz.sysykeji.top/gtpkzaazra.html

[T18] Swift：字符串插值
来源：http://hz.cashguo.top/gtdzththoi.html

"值: \(b)"
来源：http://hz.chenjidiqi.icu/gtotdxzwnb.html

[T19] Swift：可选绑定
来源：http://hz.jqgufenzy.top/gtfveyjkcp.html

if let n = opt { print(n) }
来源：http://hz.vqdsnc.cn/gtnkwyggoy.html

[T20] Swift：数组操作
来源：http://hz.yanxiufei.cn/gtwrpnnryo.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.iojbl.cn/gtmgokuvqj.html

[T21] Swift：遍历
来源：http://hz.dianchejie.cn/gtuvxvpfha.html

for x in a { print(x) }
来源：http://hz.zhijiandao.cn/gtlqinahkt.html

[T22] Swift：字典
来源：http://hz.wangdashe.top/gtkygvdxby.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.tianlin.xyz/gtjzrkgrjb.html

[T23] Swift：函数
来源：http://hz.iojbl.cn/gtauedbels.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.guowangkeji.top/gtdjdydwky.html

[T24] Swift：闭包
来源：http://hz.yj202588.top/gtbpbnzpig.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.0kj1m.cn/gtsufnpeus.html

[T25] Swift：结构体
来源：http://hz.sxryk.cn/gtllkevzlk.html

struct P { var x: Int }
来源：http://hz.hysaishi.cn/gtgtfbobio.html

[T26] Swift：类与重写
来源：http://hz.hnxiangtu.top/gtttbvivii.html

class A: Base { override func f() {} }
来源：http://hz.jqgufenzy.top/gtcxyvubel.html

[T27] Swift：错误处理
来源：http://hz.shzxlz.cn/gtjbofjegc.html

do { try f() } catch { print(error) }
来源：http://hz.zhengqikj.top/gteinietta.html

[T28] Swift：枚举
来源：http://hz.jinqigfzy.top/gtbgfppbhi.html

enum Color { case red, green }
来源：http://hz.hnxiangtu.top/gtzeyteynk.html

[T29] Swift：guard 提前返回
来源：http://hz.zhongyouzk.top/gtbirfguit.html

guard let x = opt else { return }
来源：http://hz.gzhubu.top/gtitvseeia.html

[T30] Swift：协议
来源：http://hz.quarkkingdee.top/gtbjxpsbaz.html

protocol Shape { func area() -> Double }
来源：http://hz.ehwqpu.com/gtrettyleo.html

[T31] Lua：Hello World
来源：http://hz.pycfn.com/gtqostghzc.html

print("Hello")
来源：http://hz.svipenyu.cn/gtzmhttbig.html

[T32] Lua：局部变量
来源：http://hz.ppjwa.cn/gtpbocwezu.html

local a = 1
来源：http://hz.xylfe.cn/gtadzzxznl.html

[T33] Lua：表（数组）
来源：http://hz.shanyushiyangtech.top/gtgypjyihb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.smart0.xyz/gtwkeksqlp.html

[T34] Lua：遍历表
来源：http://hz.pycfn.com/gtrsjmlzek.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.cdnleiting.top/gtvckqfvot.html

[T35] Lua：字典表
来源：http://hz.guowangkeji.top/gtprgfbrfp.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yj20258.top/gttrruqdgs.html

[T36] Lua：函数
来源：http://hz.pycfn.com/gttstbuudy.html

function add(a, b) return a + b end
来源：http://hz.zhengqikj.top/gtwbocptva.html

[T37] Lua：字符串拼接
来源：http://hz.jinqigfzy.top/gtpbreguku.html

"a" .. "b"
来源：http://hz.hnqzz.top/gtkumktgyy.html

[T38] Lua：条件
来源：http://hz.gogol.net.cn/gtcndvgwrp.html

if x > 0 then print("正") end
来源：http://hz.dashuyun.cn/gtdlhefauc.html

[T39] Lua：模式匹配
来源：http://hz.xuetiantiany.cn/gtyoxhlxsg.html

string.find(s, "%d+")
来源：http://hz.pengpengdd.cyou/gtqjoxtylt.html

[T40] Lua：元表
来源：http://hz.quarkkingdee.top/gtpwxsnorm.html

setmetatable({}, { __index = base })
来源：http://hz.shanyushiyangtech.top/gtrwlhsijs.html

[T41] Perl：Hello World
来源：http://hz.gogol.net.cn/gtlvzqlzmp.html

print "Hello\n";
来源：http://hz.dashuyun.cn/gtoebfliqj.html

[T42] Perl：变量类型
来源：http://hz.yongpay.top/gtyeqmiquj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yj202588.top/gtvvwkqcvn.html

[T43] Perl：字符串插值
来源：http://hz.feifeiyinyue.top/gtsepfitra.html

"值: $a"
来源：http://hz.zhiwuduotai.top/gtkghkbphe.html

[T44] Perl：条件
来源：http://hz.cqqwz.cn/gtvbeogbat.html

if ($a > 0) { print "正"; }
来源：http://hz.jianghu66.top/gtcsjsbkxu.html

[T45] Perl：数组遍历
来源：http://hz.zhongyouzk.top/gtkbaeqjok.html

for my $x (@arr) { print $x; }
来源：http://hz.snrcjt.cn/gtmfygiuuo.html

[T46] Perl：哈希操作
来源：http://hz.chenlongwang.top/gtdnrtwrzx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.52xcode.cn/gtatlzfmnj.html

[T47] Perl：正则捕获
来源：http://hz.xinyue.icu/gtlatdzpub.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.hammf.cn/gtktzgrsho.html

[T48] Perl：正则替换
来源：http://hz.birdmap.top/gtxvhiriiz.html

$s =~ s/old/new/g;
来源：http://hz.wangdashe.top/gttcfjbcme.html

[T49] Perl：函数
来源：http://hz.feifeiyinyue.top/gtqbgdpvsw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jqgufenzy.top/gtproaphlf.html

[T50] Perl：逐行读文件
来源：http://hz.haohaochexian.top/gtyrvhqglr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.aizwys.cn/gtrmqfohgd.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.hysaishi.cn/gtfqngrjdp.html

[T51] Scala：Hello World
来源：http://hz.jlsjyb.cn/gtgdzzcuaw.html

println("Hello")
来源：http://hz.chenjidiqi.icu/gtjibrdszl.html

[T52] Scala：变量
来源：http://hz.meibo888.top/gtydswajmu.html

val a = 1;  var b = 2
来源：http://hz.zdqjudy.top/gtlanbgttp.html

[T53] Scala：字符串插值
来源：http://hz.yanxiufei.cn/gtfjwlfciy.html

s"值: $b"
来源：http://hz.mhx1999.top/gtanidrmwo.html

[T54] Scala：集合映射
来源：http://hz.yj202588.top/gtzttnhlqb.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yonumen.top/gtlbekmwut.html

[T55] Scala：集合过滤
来源：http://hz.chenjidiqi.icu/gtuorsfkxu.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.shanyushiyangtech.top/gtawpgkuof.html

[T56] Scala：样例类
来源：http://hz.mhx1999.top/gtzogobatd.html

case class User(name: String, age: Int)
来源：http://hz.chenjidiqi.icu/gtkbwroihy.html

[T57] Scala：模式匹配
来源：http://hz.yangfankeji.com/gtvcglosmj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zhaomingkeji.xyz/gtkujvwehf.html

[T58] Scala：函数定义
来源：http://hz.shanyushiyangkeji.top/gtiivhknoj.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.iojbl.cn/gtoozcwcjo.html

[T59] Scala：循环
来源：http://hz.guannengcc.top/gtpstyiszr.html

for (i <- 1 to 10) println(i)
来源：http://hz.ppjwa.cn/gtdgtmzncm.html

[T60] Scala：折叠
来源：http://hz.jianghu66.top/gtloepmcke.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.c1oappe.top/gtxecngrxp.html

================================================================================
来源：http://hz.316326.xyz/gtdctzsfna.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jiagoushi.top/gthuceilae.html

================================================================================
来源：http://hz.shuidangran.top/gtwxgjsbjr.html

[U01] Py：创建虚拟环境
来源：http://hz.sweek.top/gtxfilfcrx.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.cqqwz.cn/gtemwfegya.html

[U02] Py：导出 / 安装依赖
来源：http://hz.cucudq.cn/gtlmtgvfza.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.shanyushiyangtech.top/gtnpglmkae.html

[U03] Py：加载 .env 配置
来源：http://hz.vqdsnc.cn/gtexqjntlz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.cdnleiting.top/gtvppnolho.html

[U04] Py：变量调试打印
来源：http://hz.zhengqikj.top/gtkklnzmvy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.tianlin.xyz/gtemhfaezw.html

[U05] Py：列表去重且保序
来源：http://hz.feifeiyinyue.top/gtiajhgchv.html

list(dict.fromkeys(arr))
来源：http://hz.nanxuanxn.top/gtqdczxuri.html

[U06] Py：合并两个字典
来源：http://hz.feifeiyinyue.top/gtdapovsko.html

{**a, **b}
来源：http://hz.ybcxt.top/gtrpdpgfft.html

[U07] Py：反转字典键值
来源：http://hz.aibaodan.cn/gtwsrsdvqd.html

{v: k for k, v in d.items()}
来源：http://hz.zhongyouzk.top/gtmuiibpcn.html

[U08] Py：展平二维列表
来源：http://hz.cqqwz.cn/gtrisybllg.html

[y for x in nested for y in x]
来源：http://hz.meibo888.top/gthcvklnva.html

[U09] Py：字典取最大值的键
来源：http://hz.jqgufenzy.top/gthirkjvub.html

max(d, key=d.get)
来源：http://hz.zhiwuduotai.top/gtclarxwmx.html

[U10] Py：按值排序字典
来源：http://hz.316326.xyz/gtxtiyzmcw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.chenlongwang.top/gtwkkxmcot.html

[U11] Py：生成器表达式
来源：http://hz.jlsjyb.cn/gtuwarmtjf.html

(x * 2 for x in arr)
来源：http://hz.aizwys.cn/gtkeczvjsn.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.hnxiangtu.top/gtfewwwkzo.html

Counter(arr).most_common(3)
来源：http://hz.cdnleiting.top/gtulowgvbe.html

[U13] Py：固定长度队列
来源：http://hz.vqdsnc.cn/gtnlmpwakv.html

deque(maxlen=10)
来源：http://hz.jinqigfzy.top/gtlhpiuaun.html

[U14] Py：分组收集到列表
来源：http://hz.cucudq.cn/gtohlugtri.html

defaultdict(list)
来源：http://hz.kuanghao11.cn/gttygkeeyi.html

[U15] Py：高精度计时
来源：http://hz.yj20258.top/gtsarwfrpw.html

t = time.perf_counter()
来源：http://hz.cdnleiting.top/gtorqeqsnl.html

[U16] Py：命令行参数解析
来源：http://hz.cdnleiting.top/gtntscevut.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.tian-w.cn/gtqhognpar.html

[U17] Py：初始化日志
来源：http://hz.xuetiantiany.cn/gtqwghctlj.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.jqgufenzy.top/gthiycqdye.html

[U18] Py：预编译正则
来源：http://hz.andypj.xyz/gtcfukaugc.html

pat = re.compile(r"\d+")
来源：http://hz.gzhubu.top/gtyacgwjki.html

[U19] Py：正则替换带回调
来源：http://hz.smart0.xyz/gtfnzdnxkz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.tanke756.top/gtwmnzlcho.html

[U20] Py：缓存函数结果
来源：http://hz.shanyushiyangtech.top/gtiaolyvnp.html

@functools.lru_cache(maxsize=None)
来源：http://hz.nanxuanxn.top/gtvhdbzqjg.html

[U21] Py：自定义上下文管理器
来源：http://hz.xuanzx.com/gtbvjidxlq.html

@contextlib.contextmanager
来源：http://hz.zhiwuduotai.top/gtytsbhipd.html

[U22] Py：矩阵转置
来源：http://hz.zhongyouzk.top/gtawxvlyts.html

list(zip(*m))
来源：http://hz.316326.xyz/gtqvrptivr.html

[U23] Py：分块读取大文件
来源：http://hz.jqgufenzy.top/gtpzamctny.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.fengsongda.top/gtetsaldfe.html

[U24] Py：路径操作
来源：http://hz.ywan-chungtsiang.top/gtrbdbefxz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.yj202588.top/gtjwhiiysu.html

[U25] Py：CSV 按字典读
来源：http://hz.xuetiantiany.cn/gttezstfyb.html

csv.DictReader(f)
来源：http://hz.hnqzz.top/gtwpkyukfb.html

[U26] Py：并发下载
来源：http://hz.jlsjyb.cn/gtnjhiebcc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.daxiang520.top/gtohojyedh.html

[U27] Py：异步 HTTP
来源：http://hz.quarkkingdee.top/gtiqlvrwmu.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.zhaomingkeji.xyz/gttutcrfms.html

[U28] Py：类型别名
来源：http://hz.pycfn.com/gtlglhkaun.html

UserId = int
来源：http://hz.fzhhl.top/gtgjnvoxpk.html

[U29] Py：属性校验
来源：http://hz.daxiang520.top/gtmlmejngl.html

@property 与 @x.setter 配合
来源：http://hz.pengpengdd.cyou/gtrkdxjqeu.html

[U30] Py：数据类
来源：http://hz.cashguo.top/gtktlgsumr.html

@dataclass(slots=True)
来源：http://hz.yj202588.top/gtndoionwh.html

[U31] Py：单测
来源：http://hz.yj20258888.top/gtthtoeliu.html

python -m pytest -q
来源：http://hz.kuanghao11.cn/gtqiiusxcv.html

[U32] Py：代码格式化
来源：http://hz.zhiwuduotai.top/gtkhtbosti.html

ruff format . && ruff check --fix .
来源：http://hz.haohaochexian.top/gtpfquhtgm.html

[U33] Py：打包发布
来源：http://hz.andypj.xyz/gtkoiqwzwu.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.tianlin.xyz/gthuistgga.html

[U34] Py：判断编码
来源：http://hz.hywenlv.cn/gtjosbjmen.html

chardet.detect(raw)
来源：http://hz.ehwqpu.com/gtfxkcmdru.html

[U35] Py：发送邮件
来源：http://hz.ppjwa.cn/gtqkjdklim.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.yj20258888.top/gtwmkmrnbn.html

[U36] Py：定时任务
来源：http://hz.ivvv.top/gtyepmebav.html

schedule.every(10).minutes.do(job)
来源：http://hz.gogol.net.cn/gthlgapysu.html


<!-- 参考信息 -->