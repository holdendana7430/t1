代发 wailian999

x |= (1 << 3);
来源：http://hz.hysaishi.cn/gtiuijsplf.html

[S17] C：安全拼接字符串
来源：http://hz.wangshuangyany.cn/gtnzistnfg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.vqdsnc.cn/gtzkokschw.html

[S18] C：命令行参数
来源：http://hz.ywan-chungtsiang.top/gtowrukmjl.html

int main(int argc, char **argv)
来源：http://hz.nanxinkj.top/gttfjlcgjc.html

[S19] C：快速排序
来源：http://hz.birdmap.top/gtbinzsiji.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.cashguo.top/gtdwuxukhz.html

[S20] C：二分查找
来源：http://hz.sysykeji.top/gtwtbbfoop.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.xuanzx.com/gthvnshhqw.html

[S21] C：字符类别判断
来源：http://hz.zhoulong.xyz/gtrhbqvrok.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xuetiantiany.cn/gthefbrbai.html

[S22] C：字符串转数字
来源：http://hz.fengsongda.top/gtfpsefufg.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.haohaochexian.top/gtwrjbgbmf.html

[S23] C：随机数
来源：http://hz.shanyushiyangtech.top/gtxhokrtir.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yuxming.cn/gtliiaprqv.html

[S24] C：获取本地时间
来源：http://hz.jqgufenzy.top/gtevxujcik.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.dianchejie.cn/gtbidqvqqo.html

[S25] C：内存拷贝
来源：http://hz.tian-w.cn/gtffixajvh.html

memcpy(dst, src, n);
来源：http://hz.yj20258.top/gtjrgkkgje.html

[S26] C：内存清零
来源：http://hz.fzhhl.top/gtnuxnsuvy.html

memset(a, 0, sizeof a);
来源：http://hz.svipenyu.cn/gtrzclqnkw.html

[S27] C：定义常量
来源：http://hz.gotoacloud.top/gtrquwuwun.html

const double PI = 3.14159;
来源：http://hz.zhongyouzk.top/gtwljpzhgr.html

[S28] C：静态变量
来源：http://hz.sysykeji.top/gtdmxpjimg.html

static int counter = 0;
来源：http://hz.c1oappe.top/gtxfzvvfiz.html

[S29] C：变参函数
来源：http://hz.aizwys.cn/gteboktllw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhaomingkeji.xyz/gtlpqajsft.html

[S30] C：头文件保护
来源：http://hz.shuidangran.top/gtfzpgzqrs.html

#ifndef X_H
来源：http://hz.cdnleiting.top/gtelerqwxh.html

#define X_H
来源：http://hz.cdnleiting.top/gtumkfqpvq.html

#endif
来源：http://hz.yj20258.top/gthzeunwpm.html

[S31] C++：Hello World
来源：http://hz.shangyingyoupin.top/gtoswgnizi.html

#include <iostream>
来源：http://hz.bjfxy.top/gtdhffjsvc.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.shanyushiyangtech.top/gtzthinmnr.html

[S32] C++：字符串
来源：http://hz.iojbl.cn/gtfbutxvem.html

std::string s = "hi";  s += "!";
来源：http://hz.chenlongwang.top/gtrjkfvmgv.html

[S33] C++：vector 增删
来源：http://hz.yuxming.cn/gtdhnldtjv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.xuanzx.com/gtfbqfevgx.html

[S34] C++：遍历 vector
来源：http://hz.fengsongda.top/gtavfehodu.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ppjwa.cn/gtddrgciwi.html

[S35] C++：map
来源：http://hz.jyoumei.cn/gtbgcspzfs.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.52xcode.cn/gtovhvlqlo.html

[S36] C++：unordered_map
来源：http://hz.zhijiandao.cn/gtrnlohdhq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hongshengwenyu.top/gtdtctftgz.html

[S37] C++：set
来源：http://hz.iojbl.cn/gtfnmfrnlx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jinyuanbaomall.cn/gtermjdxmq.html

[S38] C++：排序
来源：http://hz.nwbrower.top/gthjymobtg.html

std::sort(v.begin(), v.end());
来源：http://hz.svipenyu.cn/gtjtcxvrox.html

[S39] C++：自定义比较器排序
来源：http://hz.gotoacloud.top/gttudoeuww.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.nanxuanxn.top/gtkpscuvcm.html

[S40] C++：查找元素
来源：http://hz.andypj.xyz/gtgwscnwmh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.chenjidiqi.icu/gtrjrgdsfp.html

[S41] C++：类与构造函数
来源：http://hz.snrcjt.cn/gtcnlwwbsg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yj20258888.top/gteztuqgvl.html

[S42] C++：继承与虚函数
来源：http://hz.yangfankeji.com/gtcttzqute.html

class B : public Base { public: void f() override {} };
来源：http://hz.jqgufenzy.top/gthgytdstc.html

[S43] C++：智能指针
来源：http://hz.pycfn.com/gtctgqzkly.html

auto p = std::make_unique<int>(5);
来源：http://hz.yuxming.cn/gtbzlxleyx.html

[S44] C++：引用传参
来源：http://hz.yueranfly.top/gttlmiozgk.html

void inc(int &x) { ++x; }
来源：http://hz.jinyuanbaomall.cn/gthedxudzi.html

[S45] C++：lambda
来源：http://hz.mhx1999.top/gtgpmsnrij.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhijiandao.cn/gtuuadvvdk.html

[S46] C++：函数模板
来源：http://hz.smart0.xyz/gtyuivdpai.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhiwuduotai.top/gtcunwphvd.html

[S47] C++：结构化绑定遍历
来源：http://hz.guannengcc.top/gtgodbrhjl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.hnqzz.top/gtsaqxachh.html

[S48] C++：逐行读文件
来源：http://hz.52xcode.cn/gtdtlkgdck.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.0kj1m.cn/gtmlmqknpn.html

while (std::getline(in, line)) { }
来源：http://hz.jyoumei.cn/gtgoydivfs.html

[S49] C++：写文件
来源：http://hz.dianchejie.cn/gtncsswrkl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ppjwa.cn/gtosrwujag.html

[S50] C++：格式化数字
来源：http://hz.jyoumei.cn/gtmjxaxwuo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.cqqwz.cn/gtnarfbyvm.html

[S51] C++：显式类型转换
来源：http://hz.tian-w.cn/gtfunhmtdg.html

static_cast<double>(a) / b
来源：http://hz.smart0.xyz/gtildekuqd.html

[S52] C++：const 与 noexcept
来源：http://hz.zhaomingkeji.xyz/gtkimarltl.html

int size() const noexcept { return n_; }
来源：http://hz.svipenyu.cn/gtheruryhy.html

[S53] C++：移动语义
来源：http://hz.jinghuilouyu.cn/gtarekgxwc.html

std::vector<int> w = std::move(v);
来源：http://hz.daria6918.cn/gtlyczdvzj.html

[S54] C++：异常处理
来源：http://hz.xinyue.icu/gtkmxvjkhw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.c1oappe.top/gtsaivcttz.html

[S55] C++：结构化绑定
来源：http://hz.birdmap.top/gtvawewcxn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.svipenyu.cn/gtdcvvgtiq.html

[S56] C++：optional
来源：http://hz.hywenlv.cn/gtipmdqpfm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.xziqi.cn/gtgapaijpd.html

[S57] C++：编译期常量
来源：http://hz.dianchejie.cn/gtfkboaexm.html

constexpr int N = 10;
来源：http://hz.zdqjudy.top/gtpufvryem.html

[S58] C++：命名空间
来源：http://hz.feifeiyinyue.top/gtfzinsmbv.html

namespace ns { int f() { return 1; } }
来源：http://hz.xuanzx.com/gtiwigpzgw.html

[S59] C++：静态断言
来源：http://hz.gogol.net.cn/gtdxwefuhz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.wangdashe.top/gtvzgvskqq.html

[S60] C++：遍历并删除元素
来源：http://hz.zhengqikj.top/gtnqfucnwv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.9152youxi.cn/gtsmzbuzoj.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtqyirhhii.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.wangdashe.top/gtkvobufst.html

================================================================================
来源：http://hz.gzhubu.top/gtohjasmuv.html

[T01] Kotlin：Hello World
来源：http://hz.cheryme.top/gtmpvkrwln.html

println("Hello")
来源：http://hz.hongshengwenyu.top/gtwdsczxib.html

[T02] Kotlin：变量
来源：http://hz.gzhubu.top/gtfiverjbz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.nanxinkj.top/gtrnurfzgs.html

[T03] Kotlin：字符串模板
来源：http://hz.gogol.net.cn/gtgmlofear.html

"值: $b"
来源：http://hz.zhaomingkeji.xyz/gtizxwfuax.html

[T04] Kotlin：空安全
来源：http://hz.hammf.cn/gtdjtomplr.html

val n: String? = null;  n?.length
来源：http://hz.gzhubu.top/gtgnjucjev.html

[T05] Kotlin：when 表达式
来源：http://hz.xziqi.cn/gtisnoebbf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.snrcjt.cn/gtdxiiyfhe.html

[T06] Kotlin：集合映射
来源：http://hz.tanke756.top/gtqjgzyrre.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.birdmap.top/gtjmawilrs.html

[T07] Kotlin：集合过滤
来源：http://hz.hammf.cn/gtjkbatina.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.iojbl.cn/gtpdyhjilq.html

[T08] Kotlin：数据类
来源：http://hz.ppjwa.cn/gtoboszqwr.html

data class User(val name: String, val age: Int)
来源：http://hz.cheryme.top/gtkkwkowsn.html

[T09] Kotlin：扩展函数
来源：http://hz.svipenyu.cn/gtpazuudve.html

fun String.exclaim() = this + "!"
来源：http://hz.haohaochexian.top/gtonckxysc.html

[T10] Kotlin：默认参数
来源：http://hz.yj20258.top/gtylmowlsf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.xuetiantiany.cn/gtmxsiuwmi.html

[T11] Kotlin：协程
来源：http://hz.quarkkingdee.top/gtjqovwdok.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.haohaochexian.top/gtdxaiyptq.html

[T12] Kotlin：解构声明
来源：http://hz.xziqi.cn/gthceblmet.html

val (a, b) = Pair(1, 2)
来源：http://hz.birdmap.top/gthxaytupm.html

[T13] Kotlin：只读 Map
来源：http://hz.shuidangran.top/gtfwvcrbsi.html

val m = mapOf("a" to 1)
来源：http://hz.smart0.xyz/gtfhpqlclm.html

[T14] Kotlin：循环
来源：http://hz.iojbl.cn/gtdfkqvfcj.html

for (i in 1..10) println(i)
来源：http://hz.ydzc1.top/gteysnkoji.html

[T15] Kotlin：接口
来源：http://hz.jyoumei.cn/gtrvoufjsc.html

interface Shape { fun area(): Double }
来源：http://hz.yangfankeji.com/gtipsvgkmd.html

[T16] Swift：Hello World
来源：http://hz.hfpthk.cn/gtyzuyfhyv.html

print("Hello")
来源：http://hz.nwbrower.top/gtqvqlmfxk.html

[T17] Swift：变量与常量
来源：http://hz.pycfn.com/gtinwcxixt.html

var a = 1;  let b = 2
来源：http://hz.jinqigufen.top/gtlixarzgd.html

[T18] Swift：字符串插值
来源：http://hz.xuetiantiany.cn/gtygufojku.html

"值: \(b)"
来源：http://hz.iojbl.cn/gtmlzzxabt.html

[T19] Swift：可选绑定
来源：http://hz.jinyuanbaomall.cn/gtjqgcgpbd.html

if let n = opt { print(n) }
来源：http://hz.quarkkingdee.top/gtcohtvehd.html

[T20] Swift：数组操作
来源：http://hz.hfpthk.cn/gthdlvfzcy.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.hywenlv.cn/gtmtczljvp.html

[T21] Swift：遍历
来源：http://hz.zhoulong.xyz/gtdftvltbw.html

for x in a { print(x) }
来源：http://hz.shangyingyoupin.top/gtzxypfgsu.html

[T22] Swift：字典
来源：http://hz.yangfankeji.com/gtzqtcoqui.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.cucudq.cn/gthacofzva.html

[T23] Swift：函数
来源：http://hz.jinqigufen.top/gtfgnpvagw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.tian-w.cn/gtovdcpfjc.html

[T24] Swift：闭包
来源：http://hz.bjfxy.top/gtpznwpxnz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.guannengcc.top/gthhpqrtfn.html

[T25] Swift：结构体
来源：http://hz.fzhhl.top/gtrlzafkkx.html

struct P { var x: Int }
来源：http://hz.vqdsnc.cn/gtzjcgzlpe.html

[T26] Swift：类与重写
来源：http://hz.gzhubu.top/gtmbgooakc.html

class A: Base { override func f() {} }
来源：http://hz.jinghuilouyu.cn/gtexblayjn.html

[T27] Swift：错误处理
来源：http://hz.ehwqpu.com/gtcjjyxida.html

do { try f() } catch { print(error) }
来源：http://hz.ywan-chungtsiang.top/gtuuvlccwk.html

[T28] Swift：枚举
来源：http://hz.hysaishi.cn/gthczrviez.html

enum Color { case red, green }
来源：http://hz.shangyingyoupin.top/gtcjcfmtku.html

[T29] Swift：guard 提前返回
来源：http://hz.hfpthk.cn/gtpypmzony.html

guard let x = opt else { return }
来源：http://hz.yueranfly.top/gtmwmczlda.html

[T30] Swift：协议
来源：http://hz.guowangkeji.top/gtlpyztdrz.html

protocol Shape { func area() -> Double }
来源：http://hz.zhaomingkeji.xyz/gttwdtfcgg.html

[T31] Lua：Hello World
来源：http://hz.birdmap.top/gtgvwybrzl.html

print("Hello")
来源：http://hz.yongpay.top/gtigvadynj.html

[T32] Lua：局部变量
来源：http://hz.pengpengdd.cyou/gtspmuglyc.html

local a = 1
来源：http://hz.redwolf501.top/gtftegtyty.html

[T33] Lua：表（数组）
来源：http://hz.yanxiufei.cn/gtjhdphtgi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.shuidangran.top/gtohqbsflm.html

[T34] Lua：遍历表
来源：http://hz.52xcode.cn/gtiliwnpcz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.shangyingyoupin.top/gtbdvvgspx.html

[T35] Lua：字典表
来源：http://hz.guannengcc.top/gtfrnlatjv.html

local d = { a = 1 };  d.b = 2
来源：http://hz.feifeiyinyue.top/gtsgrnqany.html

[T36] Lua：函数
来源：http://hz.smart0.xyz/gtisvlpqyv.html

function add(a, b) return a + b end
来源：http://hz.hywenlv.cn/gtxxtotryj.html

[T37] Lua：字符串拼接
来源：http://hz.xylfe.cn/gtqttijblf.html

"a" .. "b"
来源：http://hz.gaohongyu789.top/gtuiylpuke.html

[T38] Lua：条件
来源：http://hz.dashuyun.cn/gtwpcharvt.html

if x > 0 then print("正") end
来源：http://hz.jinqigufen.top/gtfkbxlkcf.html

[T39] Lua：模式匹配
来源：http://hz.fzhhl.top/gtcccknfbp.html

string.find(s, "%d+")
来源：http://hz.hysaishi.cn/gtntojodcp.html

[T40] Lua：元表
来源：http://hz.shuidangran.top/gtuplrojum.html

setmetatable({}, { __index = base })
来源：http://hz.pycfn.com/gtercdbqyg.html

[T41] Perl：Hello World
来源：http://hz.snrcjt.cn/gtungwznbg.html

print "Hello\n";
来源：http://hz.zdqjudy.top/gtwcybegrf.html

[T42] Perl：变量类型
来源：http://hz.hfpthk.cn/gtdlgnyvss.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jyoumei.cn/gtjgimttne.html

[T43] Perl：字符串插值
来源：http://hz.sxryk.cn/gtiaaapdpl.html

"值: $a"
来源：http://hz.cdnleiting.top/gtemwmzley.html

[T44] Perl：条件
来源：http://hz.xuetiantiany.cn/gtbkbiykld.html

if ($a > 0) { print "正"; }
来源：http://hz.jinyuanbaomall.cn/gtsuqgtqdp.html

[T45] Perl：数组遍历
来源：http://hz.xuanzx.com/gtraesjbgf.html

for my $x (@arr) { print $x; }
来源：http://hz.xziqi.cn/gtrlqrsndl.html

[T46] Perl：哈希操作
来源：http://hz.zhongyouzk.top/gtnscmwsqq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.chenlongwang.top/gtuhzqahjd.html

[T47] Perl：正则捕获
来源：http://hz.pengpengdd.cyou/gtgyryrcfu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.dianchejie.cn/gtfamdnjph.html

[T48] Perl：正则替换
来源：http://hz.zycfv.cn/gtxxnegnpa.html

$s =~ s/old/new/g;
来源：http://hz.chenlongwang.top/gtdrzmbusg.html

[T49] Perl：函数
来源：http://hz.zdqjudy.top/gtysfkqmah.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.cashguo.top/gtjyuwgmtz.html

[T50] Perl：逐行读文件
来源：http://hz.xuetiantiany.cn/gteciuxdbi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.zhiwuduotai.top/gtpqzvgqrj.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.cqqwz.cn/gtighyvurk.html

[T51] Scala：Hello World
来源：http://hz.haohaochexian.top/gttmqnaxrt.html

println("Hello")
来源：http://hz.nwbrower.top/gtcbeikhsq.html

[T52] Scala：变量
来源：http://hz.yangfankeji.com/gtcthcnhmr.html

val a = 1;  var b = 2
来源：http://hz.yuxming.cn/gtrxfxwppo.html

[T53] Scala：字符串插值
来源：http://hz.fengsongda.top/gtlilxtgae.html

s"值: $b"
来源：http://hz.sufxvd.cn/gtwswpolcp.html

[T54] Scala：集合映射
来源：http://hz.xingfuxueyuan.xyz/gtehmtgdoe.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yuxming.cn/gtslulklub.html

[T55] Scala：集合过滤
来源：http://hz.nanxuanxn.top/gtgnwodlti.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jinqigfzy.top/gturnwujzm.html

[T56] Scala：样例类
来源：http://hz.vqdsnc.cn/gtflqjisep.html

case class User(name: String, age: Int)
来源：http://hz.zhiwuduotai.top/gtbmhvcdmn.html

[T57] Scala：模式匹配
来源：http://hz.hongshengwenyu.top/gtoszkcyyg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.iojbl.cn/gtoaymgtmx.html

[T58] Scala：函数定义
来源：http://hz.yuxming.cn/gtqzwhbrzn.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.sysykeji.top/gtxzesikyr.html

[T59] Scala：循环
来源：http://hz.pengpengdd.cyou/gtivhuxcnm.html

for (i <- 1 to 10) println(i)
来源：http://hz.svipenyu.cn/gtgbanxxan.html

[T60] Scala：折叠
来源：http://hz.bjfxy.top/gtxvulwifq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.xingfuxueyuan.xyz/gtjbtfvmsb.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtkcvjyxud.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.shanyushiyangtech.top/gtipbsfgan.html

================================================================================
来源：http://hz.dianchejie.cn/gtsoxhhivp.html

[U01] Py：创建虚拟环境
来源：http://hz.gogol.net.cn/gtlecqvzut.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yj20258.top/gtbfeusuid.html

[U02] Py：导出 / 安装依赖
来源：http://hz.xingfuxueyuan.xyz/gtjgjcwuve.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.tian-w.cn/gtndgueime.html

[U03] Py：加载 .env 配置
来源：http://hz.jiagoushi.top/gtasagcrpy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.gzhubu.top/gtdqhdlhpp.html

[U04] Py：变量调试打印
来源：http://hz.sxryk.cn/gtxuisugis.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.bjfxy.top/gtfeornrbu.html

[U05] Py：列表去重且保序
来源：http://hz.feifeiyinyue.top/gtspplxckz.html

list(dict.fromkeys(arr))
来源：http://hz.gotoacloud.top/gtndohntji.html

[U06] Py：合并两个字典
来源：http://hz.hysaishi.cn/gtofcyrvki.html

{**a, **b}
来源：http://hz.quarkkingdee.top/gtcejqxwnq.html

[U07] Py：反转字典键值
来源：http://hz.sufxvd.cn/gtwdruekcp.html

{v: k for k, v in d.items()}
来源：http://hz.jlsjyb.cn/gttmyuhytu.html

[U08] Py：展平二维列表
来源：http://hz.shanyushiyangtech.top/gtdtwmeeuh.html

[y for x in nested for y in x]
来源：http://hz.mhx1999.top/gtywkdstjf.html

[U09] Py：字典取最大值的键
来源：http://hz.jinqigufen.top/gtfuzruipi.html

max(d, key=d.get)
来源：http://hz.jinqigfzy.top/gtoharuunt.html

[U10] Py：按值排序字典
来源：http://hz.havefunace.top/gtgubajkfv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.quarkkingdee.top/gtifsmmemw.html

[U11] Py：生成器表达式
来源：http://hz.zhongyouzk.top/gtiecusrrp.html

(x * 2 for x in arr)
来源：http://hz.xingfuxueyuan.xyz/gtqrcqdwpn.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.xinyue.icu/gttuhybssf.html

Counter(arr).most_common(3)
来源：http://hz.smart0.xyz/gtreoykgiz.html

[U13] Py：固定长度队列
来源：http://hz.jinqigufen.top/gtfgzfijzo.html

deque(maxlen=10)
来源：http://hz.cucudq.cn/gtjjssqrwz.html

[U14] Py：分组收集到列表
来源：http://hz.yj20258.top/gtjsvfyccz.html

defaultdict(list)
来源：http://hz.yj20258.top/gtyxlgtiyk.html

[U15] Py：高精度计时
来源：http://hz.wangdashe.top/gttowmwfep.html

t = time.perf_counter()
来源：http://hz.havefunace.top/gtbppoojql.html

[U16] Py：命令行参数解析
来源：http://hz.jinghuilouyu.cn/gtudzvvxdx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.xylfe.cn/gtudtpjzmn.html

[U17] Py：初始化日志
来源：http://hz.yueranfly.top/gtjlsdcvns.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.jlsjyb.cn/gtodjoxnrk.html

[U18] Py：预编译正则
来源：http://hz.52xcode.cn/gtlcztkgdp.html

pat = re.compile(r"\d+")
来源：http://hz.jyoumei.cn/gtnnlerqcr.html

[U19] Py：正则替换带回调
来源：http://hz.daxiang520.top/gtegyacvhr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.daria6918.cn/gtatxyvzvy.html

[U20] Py：缓存函数结果
来源：http://hz.daxiang520.top/gtcpddwber.html

@functools.lru_cache(maxsize=None)
来源：http://hz.nanxuanxn.top/gtybykizxq.html

[U21] Py：自定义上下文管理器
来源：http://hz.yueranfly.top/gtwgzeylnb.html

@contextlib.contextmanager
来源：http://hz.jinyuanbaomall.cn/gtdimxzsgf.html

[U22] Py：矩阵转置
来源：http://hz.ydzc1.top/gtdmkpsqve.html

list(zip(*m))
来源：http://hz.shanyushiyangkeji.top/gtzgbmtwxz.html

[U23] Py：分块读取大文件
来源：http://hz.hysaishi.cn/gtawmvdwhr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.cdnleiting.top/gtiuajfbfc.html

[U24] Py：路径操作
来源：http://hz.daxiang520.top/gtpunfaiqv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.gzhubu.top/gtykmzaxne.html

[U25] Py：CSV 按字典读
来源：http://hz.zycfv.cn/gtwzfdftzs.html

csv.DictReader(f)
来源：http://hz.yvedp.cn/gtrlczijjg.html

[U26] Py：并发下载
来源：http://hz.jinqigufen.top/gtqvepgpcj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.tian-w.cn/gtbptlmnzm.html

[U27] Py：异步 HTTP
来源：http://hz.dianchejie.cn/gtxqdilkwh.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.nanxinkj.top/gtcahugfph.html

[U28] Py：类型别名
来源：http://hz.zhoulong.xyz/gtuuzsuria.html

UserId = int
来源：http://hz.daria6918.cn/gtyllnxmik.html

[U29] Py：属性校验
来源：http://hz.xinyue.icu/gtrhwyulit.html

@property 与 @x.setter 配合
来源：http://hz.hfpthk.cn/gtntqulggd.html

[U30] Py：数据类
来源：http://hz.quarkkingdee.top/gtdaxmkbqz.html

@dataclass(slots=True)
来源：http://hz.0kj1m.cn/gtovlmtbdw.html

[U31] Py：单测
来源：http://hz.quarkkingdee.top/gtgjexcfrw.html

python -m pytest -q
来源：http://hz.ivvv.top/gtqkdrmttv.html

[U32] Py：代码格式化
来源：http://hz.jqgfzy.top/gtoogjfiwv.html

ruff format . && ruff check --fix .
来源：http://hz.jqgfzy.top/gtslhsinco.html

[U33] Py：打包发布
来源：http://hz.meibo888.top/gtkonjzjfx.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.yonumen.top/gthoccovgi.html

[U34] Py：判断编码
来源：http://hz.tanke756.top/gtqawmpgxc.html

chardet.detect(raw)
来源：http://hz.yj202588.top/gtvwpsvzdc.html

[U35] Py：发送邮件
来源：http://hz.yangfankeji.com/gtwbaoljle.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.c1oappe.top/gtlwwvochp.html

[U36] Py：定时任务
来源：http://hz.jiagoushi.top/gtfctqicgr.html

schedule.every(10).minutes.do(job)
来源：http://hz.iojbl.cn/gtegjymiaj.html

[U37] Py：读写 Excel
来源：http://hz.daxiang520.top/gtfkznvjaj.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.yueranfly.top/gtsozonqau.html

[U38] Py：获取脚本所在目录
来源：http://hz.daria6918.cn/gtepdvhiex.html

Path(__file__).resolve().parent
来源：http://hz.jiagoushi.top/gtwjnjtdfj.html

[U39] Py：判断是否在交互环境
来源：http://hz.tian-w.cn/gtrxqxngup.html

sys.stdout.isatty()
来源：http://hz.9152youxi.cn/gtmfjgyzel.html

[U40] Py：打印到标准错误
来源：http://hz.yj202588.top/gtkncixyei.html

print("err", file=sys.stderr)
来源：http://hz.zhoulong.xyz/gtxecvedki.html


<!-- 参考信息 -->