代发 wailian999

x |= (1 << 3);
来源：http://hz.yuxming.cn/gtyvihoxdl.html

[S17] C：安全拼接字符串
来源：http://hz.0kj1m.cn/gtmertjslh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.tian-w.cn/gtcotksway.html

[S18] C：命令行参数
来源：http://hz.hammf.cn/gtpzczfuzh.html

int main(int argc, char **argv)
来源：http://hz.zhongyouzk.top/gtrbhwcblh.html

[S19] C：快速排序
来源：http://hz.vqdsnc.cn/gtasoyqqop.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.cucudq.cn/gtwkirsfqy.html

[S20] C：二分查找
来源：http://hz.xziqi.cn/gthvmmwkco.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yj202588.top/gtmnucopwz.html

[S21] C：字符类别判断
来源：http://hz.xuanzx.com/gtazhwpmgv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.guowangkeji.top/gtakmdaiaz.html

[S22] C：字符串转数字
来源：http://hz.sufxvd.cn/gtqgihknff.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yongpay.top/gtjbzafbfc.html

[S23] C：随机数
来源：http://hz.jinghuilouyu.cn/gteosdttsh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.cheryme.top/gtwzdcivsk.html

[S24] C：获取本地时间
来源：http://hz.wangshuangyany.cn/gtvupldrhx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.52xcode.cn/gtnymefkdh.html

[S25] C：内存拷贝
来源：http://hz.xinyue.icu/gtkczhzjme.html

memcpy(dst, src, n);
来源：http://hz.gaohongyu789.top/gtkfdryvjh.html

[S26] C：内存清零
来源：http://hz.jianghu66.top/gtbrfcjrvx.html

memset(a, 0, sizeof a);
来源：http://hz.wangdashe.top/gtvkkyvoem.html

[S27] C：定义常量
来源：http://hz.yueranfly.top/gtpqssqhtl.html

const double PI = 3.14159;
来源：http://hz.yj20258.top/gtzleyhupv.html

[S28] C：静态变量
来源：http://hz.daria6918.cn/gtmsrqgmxv.html

static int counter = 0;
来源：http://hz.9152youxi.cn/gtbepcltvi.html

[S29] C：变参函数
来源：http://hz.smart0.xyz/gtqsytdvkt.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.52xcode.cn/gtnejgyyjy.html

[S30] C：头文件保护
来源：http://hz.zhiwuduotai.top/gtgotagxsf.html

#ifndef X_H
来源：http://hz.yvedp.cn/gtbyhgfqhj.html

#define X_H
来源：http://hz.fzhhl.top/gtlhqhwtnj.html

#endif
来源：http://hz.birdmap.top/gtrwcmgjqy.html

[S31] C++：Hello World
来源：http://hz.c1oappe.top/gtmqnkzvva.html

#include <iostream>
来源：http://hz.yuanzhike.top/gtusgcumng.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.chenjidiqi.icu/gtxwlxhvwu.html

[S32] C++：字符串
来源：http://hz.cqqwz.cn/gtcfbubeht.html

std::string s = "hi";  s += "!";
来源：http://hz.vqdsnc.cn/gtqmzigkfr.html

[S33] C++：vector 增删
来源：http://hz.quarkkingdee.top/gtsosuslew.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jlsjyb.cn/gtptdwaixe.html

[S34] C++：遍历 vector
来源：http://hz.ppjwa.cn/gtyuqlzjug.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yj20258.top/gtmkbeumon.html

[S35] C++：map
来源：http://hz.wangshuangyany.cn/gtznywbzbh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.kuanghao11.cn/gtjcykeblx.html

[S36] C++：unordered_map
来源：http://hz.yuxming.cn/gtmwsgltle.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.snrcjt.cn/gtzsjprkys.html

[S37] C++：set
来源：http://hz.snrcjt.cn/gtirnlgiof.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ywan-chungtsiang.top/gthzkejiss.html

[S38] C++：排序
来源：http://hz.yonumen.top/gtlmmbbqyj.html

std::sort(v.begin(), v.end());
来源：http://hz.316326.xyz/gtzbtqkcbw.html

[S39] C++：自定义比较器排序
来源：http://hz.snrcjt.cn/gtnllymqet.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jianghu66.top/gtsvykatap.html

[S40] C++：查找元素
来源：http://hz.iojbl.cn/gtrvxazsjh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xziqi.cn/gtuuwhxkps.html

[S41] C++：类与构造函数
来源：http://hz.gogol.net.cn/gtqjcrckii.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.shanyushiyangtech.top/gtwoynhgtq.html

[S42] C++：继承与虚函数
来源：http://hz.yj202588.top/gtdbizjmjr.html

class B : public Base { public: void f() override {} };
来源：http://hz.pycfn.com/gtpdzqkeos.html

[S43] C++：智能指针
来源：http://hz.ywan-chungtsiang.top/gtgnpzgvgp.html

auto p = std::make_unique<int>(5);
来源：http://hz.tian-w.cn/gtlguadadb.html

[S44] C++：引用传参
来源：http://hz.xuetiantiany.cn/gthurrzvmg.html

void inc(int &x) { ++x; }
来源：http://hz.cashguo.top/gtultdnbgj.html

[S45] C++：lambda
来源：http://hz.dashuyun.cn/gtvndbwqsl.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.iojbl.cn/gtyiykgwwk.html

[S46] C++：函数模板
来源：http://hz.zhengqikj.top/gtahdkhpwp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.wangshuangyany.cn/gtxnvylicl.html

[S47] C++：结构化绑定遍历
来源：http://hz.jqgfzy.top/gtueqhtfxr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jinyuanbaomall.cn/gtaacwpwgl.html

[S48] C++：逐行读文件
来源：http://hz.yuanzhike.top/gtjxjjbzst.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.nanxinkj.top/gtawzxoekn.html

while (std::getline(in, line)) { }
来源：http://hz.yongpay.top/gtrsgtetxp.html

[S49] C++：写文件
来源：http://hz.xylfe.cn/gtaaoqiufs.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ydjk.org.cn/gteukvjckc.html

[S50] C++：格式化数字
来源：http://hz.aizwys.cn/gtapdmtefo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.shzxlz.cn/gtbsinknoy.html

[S51] C++：显式类型转换
来源：http://hz.pycfn.com/gtstatijww.html

static_cast<double>(a) / b
来源：http://hz.jiagoushi.top/gtsjbzikxg.html

[S52] C++：const 与 noexcept
来源：http://hz.guannengcc.top/gtoewolkla.html

int size() const noexcept { return n_; }
来源：http://hz.ppjwa.cn/gtkijgbqvs.html

[S53] C++：移动语义
来源：http://hz.yonumen.top/gttlvfcxzg.html

std::vector<int> w = std::move(v);
来源：http://hz.jinqigfzy.top/gtxnvjwiga.html

[S54] C++：异常处理
来源：http://hz.ivvv.top/gthuiouzmv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hammf.cn/gtnmnamxxd.html

[S55] C++：结构化绑定
来源：http://hz.chenzaomai.com/gtkmfdhmwg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.pengpengdd.cyou/gtprnmftby.html

[S56] C++：optional
来源：http://hz.dianchejie.cn/gtcfslbejs.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hysaishi.cn/gtwtlzgoqe.html

[S57] C++：编译期常量
来源：http://hz.jianghu66.top/gtoullatrl.html

constexpr int N = 10;
来源：http://hz.xuetiantiany.cn/gtlrldhfwv.html

[S58] C++：命名空间
来源：http://hz.hfpthk.cn/gtdccqzgyy.html

namespace ns { int f() { return 1; } }
来源：http://hz.xziqi.cn/gtubyohtjc.html

[S59] C++：静态断言
来源：http://hz.hysaishi.cn/gtrvogftiq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hnqzz.top/gtjyipwdrq.html

[S60] C++：遍历并删除元素
来源：http://hz.zhijiandao.cn/gtdpqkieqp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jqgufenzy.top/gtilxqlblj.html

================================================================================
来源：http://hz.chenzaomai.com/gtrbixsicl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.bjfxy.top/gtiqlsmrvp.html

================================================================================
来源：http://hz.haohaochexian.top/gttorlhapg.html

[T01] Kotlin：Hello World
来源：http://hz.hywenlv.cn/gtvqnhktld.html

println("Hello")
来源：http://hz.cashguo.top/gtugzmrbwx.html

[T02] Kotlin：变量
来源：http://hz.ybcxt.top/gttanafaix.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.9152youxi.cn/gtsaacouse.html

[T03] Kotlin：字符串模板
来源：http://hz.wangshuangyany.cn/gtzxglrwrz.html

"值: $b"
来源：http://hz.yueranfly.top/gtqvgdttkt.html

[T04] Kotlin：空安全
来源：http://hz.ydjk.org.cn/gtnzobmlrk.html

val n: String? = null;  n?.length
来源：http://hz.jqgufenzy.top/gtijiybbfl.html

[T05] Kotlin：when 表达式
来源：http://hz.tian-w.cn/gthbojofph.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.cashguo.top/gtmxkrjnqs.html

[T06] Kotlin：集合映射
来源：http://hz.tianlin.xyz/gtgkujdiyj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.gotoacloud.top/gtjvuejrjs.html

[T07] Kotlin：集合过滤
来源：http://hz.hfpthk.cn/gtpyqvgpxq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jiagoushi.top/gtohzcwbve.html

[T08] Kotlin：数据类
来源：http://hz.haohaochexian.top/gtrhcvvmur.html

data class User(val name: String, val age: Int)
来源：http://hz.cheryme.top/gtjtreyyzl.html

[T09] Kotlin：扩展函数
来源：http://hz.nanxuanxn.top/gtheghxior.html

fun String.exclaim() = this + "!"
来源：http://hz.hywenlv.cn/gtbjqcnlor.html

[T10] Kotlin：默认参数
来源：http://hz.fzhhl.top/gtmuccppuy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.meibo888.top/gtkcbqrsku.html

[T11] Kotlin：协程
来源：http://hz.zhixingplan.top/gtefkpmifu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.wangdashe.top/gtnkhoelmu.html

[T12] Kotlin：解构声明
来源：http://hz.xziqi.cn/gtumlwuvpf.html

val (a, b) = Pair(1, 2)
来源：http://hz.jinyuanbaomall.cn/gtlpbwkmna.html

[T13] Kotlin：只读 Map
来源：http://hz.yangfankeji.com/gtfmjtpvan.html

val m = mapOf("a" to 1)
来源：http://hz.ybcxt.top/gtvkbzikcz.html

[T14] Kotlin：循环
来源：http://hz.jinghuilouyu.cn/gthpidbont.html

for (i in 1..10) println(i)
来源：http://hz.mhx1999.top/gtpogmiywm.html

[T15] Kotlin：接口
来源：http://hz.guowangkeji.top/gtyppuatwi.html

interface Shape { fun area(): Double }
来源：http://hz.ydzc1.top/gtyxwrnjzr.html

[T16] Swift：Hello World
来源：http://hz.yangfankeji.com/gtqstyhraj.html

print("Hello")
来源：http://hz.gaohongyu789.top/gteiocemuu.html

[T17] Swift：变量与常量
来源：http://hz.jlsjyb.cn/gtxtutdnyy.html

var a = 1;  let b = 2
来源：http://hz.daxiang520.top/gtikuybqdh.html

[T18] Swift：字符串插值
来源：http://hz.zhaomingkeji.xyz/gtrqvhnsnz.html

"值: \(b)"
来源：http://hz.gogol.net.cn/gttpivjjwy.html

[T19] Swift：可选绑定
来源：http://hz.zycfv.cn/gticnpnprt.html

if let n = opt { print(n) }
来源：http://hz.gzhubu.top/gtwnnrnmfo.html

[T20] Swift：数组操作
来源：http://hz.zhengqikj.top/gtkoroqaka.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.c1oappe.top/gtuohclaob.html

[T21] Swift：遍历
来源：http://hz.birdmap.top/gtioctblfi.html

for x in a { print(x) }
来源：http://hz.meibo888.top/gtyyxhucdg.html

[T22] Swift：字典
来源：http://hz.jiagoushi.top/gthxvjduue.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.guowangkeji.top/gtuddzcpxm.html

[T23] Swift：函数
来源：http://hz.zhixingplan.top/gtpmnwonek.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.iojbl.cn/gtxvkebisw.html

[T24] Swift：闭包
来源：http://hz.sysykeji.top/gteqhybbce.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.sufxvd.cn/gtojcbemwl.html

[T25] Swift：结构体
来源：http://hz.wangshuangyany.cn/gthznzpzmv.html

struct P { var x: Int }
来源：http://hz.zhijiandao.cn/gtjbqwisae.html

[T26] Swift：类与重写
来源：http://hz.wangshuangyany.cn/gtnmbmkycd.html

class A: Base { override func f() {} }
来源：http://hz.gzhubu.top/gtfuchvere.html

[T27] Swift：错误处理
来源：http://hz.ehwqpu.com/gtigqmhpst.html

do { try f() } catch { print(error) }
来源：http://hz.hnqzz.top/gtgidrifbf.html

[T28] Swift：枚举
来源：http://hz.svipenyu.cn/gtsiuworiq.html

enum Color { case red, green }
来源：http://hz.gaohongyu789.top/gtrywnjwnq.html

[T29] Swift：guard 提前返回
来源：http://hz.redwolf501.top/gtwufplaot.html

guard let x = opt else { return }
来源：http://hz.hnxiangtu.top/gttybkbjjd.html

[T30] Swift：协议
来源：http://hz.gogol.net.cn/gtrcsqmhqj.html

protocol Shape { func area() -> Double }
来源：http://hz.cheryme.top/gtvumpkrvi.html

[T31] Lua：Hello World
来源：http://hz.nwbrower.top/gtvcairchl.html

print("Hello")
来源：http://hz.shanyushiyangkeji.top/gtvnkymish.html

[T32] Lua：局部变量
来源：http://hz.cqqwz.cn/gtuxinzpiv.html

local a = 1
来源：http://hz.0kj1m.cn/gtxooogcpw.html

[T33] Lua：表（数组）
来源：http://hz.zhaomingkeji.xyz/gtjcofjtna.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zycfv.cn/gtzpxkkyhy.html

[T34] Lua：遍历表
来源：http://hz.jinghuilouyu.cn/gtyqfgbquc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.guowangkeji.top/gtuxqwmsmb.html

[T35] Lua：字典表
来源：http://hz.xziqi.cn/gtktvnevlc.html

local d = { a = 1 };  d.b = 2
来源：http://hz.redwolf501.top/gthyvxeujh.html

[T36] Lua：函数
来源：http://hz.0kj1m.cn/gtghrtsvsw.html

function add(a, b) return a + b end
来源：http://hz.ywan-chungtsiang.top/gtmechdvmc.html

[T37] Lua：字符串拼接
来源：http://hz.52xcode.cn/gtxhtinjzt.html

"a" .. "b"
来源：http://hz.shangyingyoupin.top/gtiidsbvoq.html

[T38] Lua：条件
来源：http://hz.ybcxt.top/gtjrfbmqtk.html

if x > 0 then print("正") end
来源：http://hz.feifeiyinyue.top/gtfrpkpgxr.html

[T39] Lua：模式匹配
来源：http://hz.hysaishi.cn/gthxgcoenq.html

string.find(s, "%d+")
来源：http://hz.bjfxy.top/gtaikcugvo.html

[T40] Lua：元表
来源：http://hz.0kj1m.cn/gtwaauqhmr.html

setmetatable({}, { __index = base })
来源：http://hz.birdmap.top/gtlhxnqvxy.html

[T41] Perl：Hello World
来源：http://hz.wangdashe.top/gtesqthtlp.html

print "Hello\n";
来源：http://hz.cdnleiting.top/gttqdlxuuv.html

[T42] Perl：变量类型
来源：http://hz.sysykeji.top/gtnzhhlbxr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.gogol.net.cn/gtarzhxybh.html

[T43] Perl：字符串插值
来源：http://hz.shuidangran.top/gtsvevkzvn.html

"值: $a"
来源：http://hz.mhx1999.top/gtoyfxayso.html

[T44] Perl：条件
来源：http://hz.0kj1m.cn/gtkgvykplr.html

if ($a > 0) { print "正"; }
来源：http://hz.9152youxi.cn/gterpycbnw.html

[T45] Perl：数组遍历
来源：http://hz.yj20258.top/gtdxbjxrro.html

for my $x (@arr) { print $x; }
来源：http://hz.aizwys.cn/gtwvqsntcs.html

[T46] Perl：哈希操作
来源：http://hz.guowangkeji.top/gtpcafthwe.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yvedp.cn/gttezmkcyg.html

[T47] Perl：正则捕获
来源：http://hz.jianghu66.top/gtoonbcrvm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.birdmap.top/gtyzrhnlic.html

[T48] Perl：正则替换
来源：http://hz.fengsongda.top/gtuvbadcbq.html

$s =~ s/old/new/g;
来源：http://hz.vqdsnc.cn/gthslijehm.html

[T49] Perl：函数
来源：http://hz.ivvv.top/gtajoeqtvf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.ybcxt.top/gtwbduhjij.html

[T50] Perl：逐行读文件
来源：http://hz.shzxlz.cn/gtcogpcekb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.meibo888.top/gtwdrplyhf.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.cheryme.top/gtysmwijqp.html

[T51] Scala：Hello World
来源：http://hz.ppjwa.cn/gtybrlbtax.html

println("Hello")
来源：http://hz.cucudq.cn/gtehlebxtt.html

[T52] Scala：变量
来源：http://hz.jyoumei.cn/gtpxaqwyfi.html

val a = 1;  var b = 2
来源：http://hz.yanxiufei.cn/gtygtqncer.html

[T53] Scala：字符串插值
来源：http://hz.jinqigufen.top/gttytyjisi.html

s"值: $b"
来源：http://hz.xylfe.cn/gtfkmocniu.html

[T54] Scala：集合映射
来源：http://hz.aibaodan.cn/gtbukyxdnb.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.meibo888.top/gtxfgigbvq.html

[T55] Scala：集合过滤
来源：http://hz.jlsjyb.cn/gtrkpkfwsb.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.0kj1m.cn/gtcnnbehju.html

[T56] Scala：样例类
来源：http://hz.ehwqpu.com/gtqxznayyj.html

case class User(name: String, age: Int)
来源：http://hz.wangshuangyany.cn/gtlnldfwts.html

[T57] Scala：模式匹配
来源：http://hz.jlsjyb.cn/gtipvqqnad.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hfpthk.cn/gtfitrlgtn.html

[T58] Scala：函数定义
来源：http://hz.zhaomingkeji.xyz/gtkfdzomuf.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.hammf.cn/gtwidwxmcp.html

[T59] Scala：循环
来源：http://hz.vqdsnc.cn/gtmgfoappv.html

for (i <- 1 to 10) println(i)
来源：http://hz.yanxiufei.cn/gthamvzuft.html

[T60] Scala：折叠
来源：http://hz.wangshuangyany.cn/gtjfmgsdsh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.xylfe.cn/gtwregnwnr.html

================================================================================
来源：http://hz.quarkkingdee.top/gtkdpaeymz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yonumen.top/gtzrdwnmvh.html

================================================================================
来源：http://hz.jiagoushi.top/gtmykkootp.html

[U01] Py：创建虚拟环境
来源：http://hz.cucudq.cn/gtgqkbjbxg.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.ybcxt.top/gtnkulyesv.html

[U02] Py：导出 / 安装依赖
来源：http://hz.tanke756.top/gtbhtnekpd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jqgufenzy.top/gtgfattydz.html

[U03] Py：加载 .env 配置
来源：http://hz.9152youxi.cn/gttucbchze.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.pycfn.com/gtkibiaclb.html

[U04] Py：变量调试打印
来源：http://hz.chenlongwang.top/gtooezcanj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.pycfn.com/gtolpduxfd.html

[U05] Py：列表去重且保序
来源：http://hz.dashuyun.cn/gtampaxfsz.html

list(dict.fromkeys(arr))
来源：http://hz.hywenlv.cn/gtvjrmpcag.html

[U06] Py：合并两个字典
来源：http://hz.cdnleiting.top/gthdbvibtd.html

{**a, **b}
来源：http://hz.kuanghao11.cn/gtmpmurlkr.html

[U07] Py：反转字典键值
来源：http://hz.smart0.xyz/gtgxksugjo.html

{v: k for k, v in d.items()}
来源：http://hz.jinqigfzy.top/gtcczqrhvc.html

[U08] Py：展平二维列表
来源：http://hz.quarkkingdee.top/gtvufpzkqu.html

[y for x in nested for y in x]
来源：http://hz.xinyue.icu/gtqquhdwux.html

[U09] Py：字典取最大值的键
来源：http://hz.daria6918.cn/gtvdglhfvp.html

max(d, key=d.get)
来源：http://hz.shuidangran.top/gtpkfigzew.html

[U10] Py：按值排序字典
来源：http://hz.chenlongwang.top/gtkxmraftg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.dianchejie.cn/gtczmjmkdj.html

[U11] Py：生成器表达式
来源：http://hz.yuanzhike.top/gtgukmhnev.html

(x * 2 for x in arr)
来源：http://hz.quarkkingdee.top/gtsqkvpzzc.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.xylfe.cn/gtdrsnssev.html

Counter(arr).most_common(3)
来源：http://hz.ybcxt.top/gtuldbnbjt.html

[U13] Py：固定长度队列
来源：http://hz.zhoulong.xyz/gtrorarxki.html

deque(maxlen=10)
来源：http://hz.fzhhl.top/gtzmdekkdd.html

[U14] Py：分组收集到列表
来源：http://hz.zhaomingkeji.xyz/gtktoahngk.html

defaultdict(list)
来源：http://hz.shuidangran.top/gtzborvlxn.html

[U15] Py：高精度计时
来源：http://hz.yj202588.top/gtguuomffh.html

t = time.perf_counter()
来源：http://hz.andypj.xyz/gtkkgulafi.html

[U16] Py：命令行参数解析
来源：http://hz.yj202588.top/gtaiiqwfts.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.tianlin.xyz/gtomfnzxuz.html

[U17] Py：初始化日志
来源：http://hz.zhongyouzk.top/gtcpobvfdw.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.redwolf501.top/gtikwnbnyb.html

[U18] Py：预编译正则
来源：http://hz.nanxuanxn.top/gtxoetusek.html

pat = re.compile(r"\d+")
来源：http://hz.0kj1m.cn/gtkcvdixrw.html

[U19] Py：正则替换带回调
来源：http://hz.nwbrower.top/gtyowphrgu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.sufxvd.cn/gtffucneli.html

[U20] Py：缓存函数结果
来源：http://hz.wangshuangyany.cn/gtqtnqyded.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yongpay.top/gtoiqfbzei.html

[U21] Py：自定义上下文管理器
来源：http://hz.wangshuangyany.cn/gtjncrkjip.html

@contextlib.contextmanager
来源：http://hz.wangshuangyany.cn/gtcuzxlfqu.html

[U22] Py：矩阵转置
来源：http://hz.gotoacloud.top/gthcovrtgu.html

list(zip(*m))
来源：http://hz.shanyushiyangtech.top/gtofevkvqb.html

[U23] Py：分块读取大文件
来源：http://hz.hfpthk.cn/gtwvfgetmw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.svipenyu.cn/gtkarawndw.html

[U24] Py：路径操作
来源：http://hz.yj20258.top/gtlyhvujzz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.shzxlz.cn/gtlthqkuen.html

[U25] Py：CSV 按字典读
来源：http://hz.meibo888.top/gtrrjaigka.html

csv.DictReader(f)
来源：http://hz.xziqi.cn/gtvostzikv.html

[U26] Py：并发下载
来源：http://hz.fzhhl.top/gtcolrdfkr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.nanxuanxn.top/gtwpibgyeb.html

[U27] Py：异步 HTTP
来源：http://hz.zhiwuduotai.top/gtzbebfqro.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.sufxvd.cn/gtiftaizyc.html

[U28] Py：类型别名
来源：http://hz.yueranfly.top/gtibgyzxhy.html

UserId = int
来源：http://hz.tianlin.xyz/gtwkwmrmvd.html

[U29] Py：属性校验
来源：http://hz.redwolf501.top/gtjmoyrtbd.html

@property 与 @x.setter 配合
来源：http://hz.shuidangran.top/gtizvpjdll.html

[U30] Py：数据类
来源：http://hz.smart0.xyz/gtdjlkbkyg.html

@dataclass(slots=True)
来源：http://hz.daria6918.cn/gtinjjaqoy.html

[U31] Py：单测
来源：http://hz.yj20258888.top/gttpjnvonq.html

python -m pytest -q
来源：http://hz.jinyuanbaomall.cn/gteqlokfny.html

[U32] Py：代码格式化
来源：http://hz.guannengcc.top/gthbfksxpi.html

ruff format . && ruff check --fix .
来源：http://hz.pycfn.com/gtrthtzjoj.html

[U33] Py：打包发布
来源：http://hz.c1oappe.top/gteysvfjrp.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.chenlongwang.top/gtzherassu.html

[U34] Py：判断编码
来源：http://hz.yonumen.top/gtpcmrqpny.html

chardet.detect(raw)
来源：http://hz.hnqzz.top/gtgivzryfb.html

[U35] Py：发送邮件
来源：http://hz.sxryk.cn/gtembbbwgh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.xingfuxueyuan.xyz/gtdadfmmpe.html

[U36] Py：定时任务
来源：http://hz.aizwys.cn/gtsgybvhnl.html

schedule.every(10).minutes.do(job)
来源：http://hz.quarkkingdee.top/gtmfrwamou.html

[U37] Py：读写 Excel
来源：http://hz.jinyuanbaomall.cn/gteupsxepu.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.xingfuxueyuan.xyz/gtebzilzer.html

[U38] Py：获取脚本所在目录
来源：http://hz.ivvv.top/gtujiruepx.html

Path(__file__).resolve().parent
来源：http://hz.birdmap.top/gtbntzzqxk.html

[U39] Py：判断是否在交互环境
来源：http://hz.zhengqikj.top/gtpgvlqeiu.html

sys.stdout.isatty()
来源：http://hz.yanxiufei.cn/gtrypegztr.html

[U40] Py：打印到标准错误
来源：http://hz.zdqjudy.top/gtfugbbixy.html

print("err", file=sys.stderr)
来源：http://hz.andypj.xyz/gtdwwkwnio.html


<!-- 参考信息 -->