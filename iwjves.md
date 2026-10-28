代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://hz.yvedp.cn/gttaeqaxyi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhengqikj.top/gtptmhxuoj.html

fclose(f);
来源：http://hz.zycfv.cn/gtggrulxcw.html

[S12] C：写文件
来源：http://hz.nanxuanxn.top/gtwryybcur.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.shanyushiyangtech.top/gtzdndcdvu.html

[S13] C：宏定义
来源：http://hz.0kj1m.cn/gtlkroswna.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zdqjudy.top/gteducfdlm.html

[S14] C：枚举
来源：http://hz.zhongyouzk.top/gtbjhnftpu.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.birdmap.top/gtykwvhaer.html

[S15] C：类型转换
来源：http://hz.sweek.top/gtvispzvjo.html

(double) a / b
来源：http://hz.xuetiantiany.cn/gtqfaphjzb.html

[S16] C：位操作置位
来源：http://hz.bjfxy.top/gtdbvsjqji.html

x |= (1 << 3);
来源：http://hz.nwbrower.top/gtmlhrzgbp.html

[S17] C：安全拼接字符串
来源：http://hz.cashguo.top/gtkvbzuzcj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jinghuilouyu.cn/gtsyetaqjq.html

[S18] C：命令行参数
来源：http://hz.ydzc1.top/gtayzcvitt.html

int main(int argc, char **argv)
来源：http://hz.shuidangran.top/gtxungeleg.html

[S19] C：快速排序
来源：http://hz.sweek.top/gtgqfksztb.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.meibo888.top/gtposjwehe.html

[S20] C：二分查找
来源：http://hz.gaohongyu789.top/gtlvkniugv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yongpay.top/gtqnmdepbz.html

[S21] C：字符类别判断
来源：http://hz.cashguo.top/gteeaaczft.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.sysykeji.top/gtwnlwqnyx.html

[S22] C：字符串转数字
来源：http://hz.xinyue.icu/gtekgfdiju.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jinqigufen.top/gtrabnofli.html

[S23] C：随机数
来源：http://hz.yvedp.cn/gtbuyuynou.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hnxiangtu.top/gtlwkzphoe.html

[S24] C：获取本地时间
来源：http://hz.yvedp.cn/gtqbugedfv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.andypj.xyz/gtqzuoohyt.html

[S25] C：内存拷贝
来源：http://hz.jinqigfzy.top/gtvxjoajxb.html

memcpy(dst, src, n);
来源：http://hz.ybcxt.top/gtpnldnnyz.html

[S26] C：内存清零
来源：http://hz.yvedp.cn/gtdxletykt.html

memset(a, 0, sizeof a);
来源：http://hz.gotoacloud.top/gtanzpwwfy.html

[S27] C：定义常量
来源：http://hz.ivvv.top/gtiemoyokr.html

const double PI = 3.14159;
来源：http://hz.yonumen.top/gtyboujmqd.html

[S28] C：静态变量
来源：http://hz.gotoacloud.top/gtkrmnbtpw.html

static int counter = 0;
来源：http://hz.xuanzx.com/gtsavfxkos.html

[S29] C：变参函数
来源：http://hz.hnqzz.top/gtjyqscojq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jyoumei.cn/gtaiaysrpi.html

[S30] C：头文件保护
来源：http://hz.sufxvd.cn/gtvwcdmbsw.html

#ifndef X_H
来源：http://hz.dianchejie.cn/gtxjeaemmf.html

#define X_H
来源：http://hz.vqdsnc.cn/gtmmdehlge.html

#endif
来源：http://hz.ywan-chungtsiang.top/gttiauvdnn.html

[S31] C++：Hello World
来源：http://hz.jinghuilouyu.cn/gtpefkygsj.html

#include <iostream>
来源：http://hz.vqdsnc.cn/gtemmzymca.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.birdmap.top/gtkhsblrll.html

[S32] C++：字符串
来源：http://hz.gogol.net.cn/gtcqvwgjne.html

std::string s = "hi";  s += "!";
来源：http://hz.aibaodan.cn/gtkdoysmno.html

[S33] C++：vector 增删
来源：http://hz.316326.xyz/gtfbsawvmg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.tian-w.cn/gtofrdvfjm.html

[S34] C++：遍历 vector
来源：http://hz.hnqzz.top/gtzvyuafce.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jqgufenzy.top/gtyedsolyi.html

[S35] C++：map
来源：http://hz.hysaishi.cn/gtkgesuuxo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nanxinkj.top/gtmdnerquo.html

[S36] C++：unordered_map
来源：http://hz.hnxiangtu.top/gtfoibmxba.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shangyingyoupin.top/gtvdhgltus.html

[S37] C++：set
来源：http://hz.guannengcc.top/gtutirbyia.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zdqjudy.top/gtttsncghf.html

[S38] C++：排序
来源：http://hz.ydzc1.top/gtqtppyjec.html

std::sort(v.begin(), v.end());
来源：http://hz.yj20258.top/gtwerlezre.html

[S39] C++：自定义比较器排序
来源：http://hz.nwbrower.top/gtvxejtunf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.sysykeji.top/gtjhhdxzod.html

[S40] C++：查找元素
来源：http://hz.zhijiandao.cn/gtmimgivpy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yuanzhike.top/gtshhydgsw.html

[S41] C++：类与构造函数
来源：http://hz.snrcjt.cn/gtxbjbjjjd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yonumen.top/gtrtzgzqae.html

[S42] C++：继承与虚函数
来源：http://hz.hammf.cn/gtrddcrvqm.html

class B : public Base { public: void f() override {} };
来源：http://hz.jiagoushi.top/gtzseuxfzs.html

[S43] C++：智能指针
来源：http://hz.gotoacloud.top/gtgsokwtjn.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhiwuduotai.top/gtuvwdwaeq.html

[S44] C++：引用传参
来源：http://hz.jinghuilouyu.cn/gtqkwcbqho.html

void inc(int &x) { ++x; }
来源：http://hz.9152youxi.cn/gtzqmbawgi.html

[S45] C++：lambda
来源：http://hz.shangyingyoupin.top/gtpiuxxeuy.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.havefunace.top/gtfnwyrkhc.html

[S46] C++：函数模板
来源：http://hz.zhaomingkeji.xyz/gtoiahsitx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.cqqwz.cn/gttjdokzia.html

[S47] C++：结构化绑定遍历
来源：http://hz.xuetiantiany.cn/gtkytnxwlt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhoulong.xyz/gtjynqanyy.html

[S48] C++：逐行读文件
来源：http://hz.tanke756.top/gtqbwitzhl.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.chenjidiqi.icu/gtmpmryabg.html

while (std::getline(in, line)) { }
来源：http://hz.zhijiandao.cn/gtjpulebqy.html

[S49] C++：写文件
来源：http://hz.tanke756.top/gtzeqcwhkl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ppjwa.cn/gttotniegx.html

[S50] C++：格式化数字
来源：http://hz.mhx1999.top/gtzdcbfrug.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.quarkkingdee.top/gtpgpspfqp.html

[S51] C++：显式类型转换
来源：http://hz.hongshengwenyu.top/gtlfkysjps.html

static_cast<double>(a) / b
来源：http://hz.sysykeji.top/gtrncslyfa.html

[S52] C++：const 与 noexcept
来源：http://hz.zycfv.cn/gtuwxxzzjm.html

int size() const noexcept { return n_; }
来源：http://hz.aibaodan.cn/gtwzdcjvyz.html

[S53] C++：移动语义
来源：http://hz.jinghuilouyu.cn/gtqrsogbus.html

std::vector<int> w = std::move(v);
来源：http://hz.feifeiyinyue.top/gtikmsvdae.html

[S54] C++：异常处理
来源：http://hz.dianchejie.cn/gtsbomjmiz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.snrcjt.cn/gtosmxudwd.html

[S55] C++：结构化绑定
来源：http://hz.hysaishi.cn/gteehlspnm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zdqjudy.top/gtburiekip.html

[S56] C++：optional
来源：http://hz.jiagoushi.top/gtwcmzlvzd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.svipenyu.cn/gtjppxmlbe.html

[S57] C++：编译期常量
来源：http://hz.sufxvd.cn/gtagjotpmx.html

constexpr int N = 10;
来源：http://hz.xinyue.icu/gtejefzudf.html

[S58] C++：命名空间
来源：http://hz.vqdsnc.cn/gtideyftpn.html

namespace ns { int f() { return 1; } }
来源：http://hz.zycfv.cn/gtjzvgxyqf.html

[S59] C++：静态断言
来源：http://hz.smart0.xyz/gtzkqwvycf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.nanxinkj.top/gtjfzsimhv.html

[S60] C++：遍历并删除元素
来源：http://hz.yonumen.top/gtqzjfecki.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.tian-w.cn/gtusbpnbif.html

================================================================================
来源：http://hz.9152youxi.cn/gtofzatbif.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jqgfzy.top/gttbmpwdzb.html

================================================================================
来源：http://hz.gogol.net.cn/gtmyiytbbe.html

[T01] Kotlin：Hello World
来源：http://hz.yj20258888.top/gtljhthths.html

println("Hello")
来源：http://hz.ybcxt.top/gtsrnqnwyg.html

[T02] Kotlin：变量
来源：http://hz.tianlin.xyz/gtckqigbas.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yongpay.top/gtgtjyqrdc.html

[T03] Kotlin：字符串模板
来源：http://hz.yj20258.top/gtalokdhkq.html

"值: $b"
来源：http://hz.daxiang520.top/gttqjnyfub.html

[T04] Kotlin：空安全
来源：http://hz.ivvv.top/gtdtrfwhaj.html

val n: String? = null;  n?.length
来源：http://hz.yj20258888.top/gtwzdllpxv.html

[T05] Kotlin：when 表达式
来源：http://hz.xingfuxueyuan.xyz/gtdzqndpga.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.fengsongda.top/gtthzresqm.html

[T06] Kotlin：集合映射
来源：http://hz.0kj1m.cn/gtspxmccje.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.iojbl.cn/gtsgzndtpl.html

[T07] Kotlin：集合过滤
来源：http://hz.cucudq.cn/gturnlgmuc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.ydzc1.top/gtbtvnywen.html

[T08] Kotlin：数据类
来源：http://hz.zhaomingkeji.xyz/gtmqnumwoc.html

data class User(val name: String, val age: Int)
来源：http://hz.kuanghao11.cn/gtuooxnwsx.html

[T09] Kotlin：扩展函数
来源：http://hz.shzxlz.cn/gthwntugep.html

fun String.exclaim() = this + "!"
来源：http://hz.nanxuanxn.top/gteuveksdn.html

[T10] Kotlin：默认参数
来源：http://hz.xylfe.cn/gthmrkeglp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zhaomingkeji.xyz/gtdpfaspsx.html

[T11] Kotlin：协程
来源：http://hz.yanxiufei.cn/gtjueeaxds.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.tanke756.top/gtuyfnnbwu.html

[T12] Kotlin：解构声明
来源：http://hz.havefunace.top/gtgdyefhun.html

val (a, b) = Pair(1, 2)
来源：http://hz.tanke756.top/gtyxdosvls.html

[T13] Kotlin：只读 Map
来源：http://hz.chenlongwang.top/gthwstdinj.html

val m = mapOf("a" to 1)
来源：http://hz.xinyue.icu/gtcczjwvaz.html

[T14] Kotlin：循环
来源：http://hz.pycfn.com/gtewkyakcw.html

for (i in 1..10) println(i)
来源：http://hz.chenjidiqi.icu/gtlyyvzvdc.html

[T15] Kotlin：接口
来源：http://hz.daria6918.cn/gtbkxqptsi.html

interface Shape { fun area(): Double }
来源：http://hz.yanxiufei.cn/gtqvqpvuby.html

[T16] Swift：Hello World
来源：http://hz.yvedp.cn/gtuohalirb.html

print("Hello")
来源：http://hz.jyoumei.cn/gtuujpubre.html

[T17] Swift：变量与常量
来源：http://hz.fzhhl.top/gthakapebv.html

var a = 1;  let b = 2
来源：http://hz.sysykeji.top/gtygpsoghp.html

[T18] Swift：字符串插值
来源：http://hz.cdnleiting.top/gtmlqmqshj.html

"值: \(b)"
来源：http://hz.jyoumei.cn/gtyacwtufu.html

[T19] Swift：可选绑定
来源：http://hz.sweek.top/gtsgjcbuvy.html

if let n = opt { print(n) }
来源：http://hz.ydzc1.top/gtholgjkjt.html

[T20] Swift：数组操作
来源：http://hz.smart0.xyz/gtolbhnypq.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.haohaochexian.top/gtitnorpea.html

[T21] Swift：遍历
来源：http://hz.cdnleiting.top/gtsvogktlk.html

for x in a { print(x) }
来源：http://hz.zdqjudy.top/gtmzygrhnj.html

[T22] Swift：字典
来源：http://hz.ywan-chungtsiang.top/gtqmfjhsgw.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jqgufenzy.top/gtwbvslbke.html

[T23] Swift：函数
来源：http://hz.gaohongyu789.top/gtvmdnhcer.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.nanxinkj.top/gtksncjbcc.html

[T24] Swift：闭包
来源：http://hz.zhongyouzk.top/gtaewsdblx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.shangyingyoupin.top/gtucvhvdnb.html

[T25] Swift：结构体
来源：http://hz.zhongyouzk.top/gtfeyefyri.html

struct P { var x: Int }
来源：http://hz.zhengqikj.top/gtyjvxfjio.html

[T26] Swift：类与重写
来源：http://hz.daria6918.cn/gtlbundnnq.html

class A: Base { override func f() {} }
来源：http://hz.ywan-chungtsiang.top/gtroqhqucs.html

[T27] Swift：错误处理
来源：http://hz.ydjk.org.cn/gtyiotgujd.html

do { try f() } catch { print(error) }
来源：http://hz.hongshengwenyu.top/gtlulnnhce.html

[T28] Swift：枚举
来源：http://hz.ehwqpu.com/gtkrgfkcvi.html

enum Color { case red, green }
来源：http://hz.yongpay.top/gtpgihttri.html

[T29] Swift：guard 提前返回
来源：http://hz.kuanghao11.cn/gtbaqctpeb.html

guard let x = opt else { return }
来源：http://hz.yonumen.top/gtpujgtmuy.html

[T30] Swift：协议
来源：http://hz.hfpthk.cn/gterhhxcqs.html

protocol Shape { func area() -> Double }
来源：http://hz.yuxming.cn/gtegoapiti.html

[T31] Lua：Hello World
来源：http://hz.jlsjyb.cn/gtnjsjwcmg.html

print("Hello")
来源：http://hz.xuetiantiany.cn/gtlerrkmpv.html

[T32] Lua：局部变量
来源：http://hz.ydjk.org.cn/gtjuhuwoyh.html

local a = 1
来源：http://hz.sysykeji.top/gtyrwadbtr.html

[T33] Lua：表（数组）
来源：http://hz.wangdashe.top/gtiacctsyl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.sxryk.cn/gtucrnpebg.html

[T34] Lua：遍历表
来源：http://hz.316326.xyz/gtabmlspwk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.zhixingplan.top/gtrgnuhens.html

[T35] Lua：字典表
来源：http://hz.yvedp.cn/gtohmzybgf.html

local d = { a = 1 };  d.b = 2
来源：http://hz.aibaodan.cn/gtgammsfhq.html

[T36] Lua：函数
来源：http://hz.hnxiangtu.top/gtvnspprbv.html

function add(a, b) return a + b end
来源：http://hz.cdnleiting.top/gtfcpedccn.html

[T37] Lua：字符串拼接
来源：http://hz.hywenlv.cn/gtuzlfmsqi.html

"a" .. "b"
来源：http://hz.ppjwa.cn/gtxojmgyjt.html

[T38] Lua：条件
来源：http://hz.guowangkeji.top/gtobtlzdsx.html

if x > 0 then print("正") end
来源：http://hz.cashguo.top/gtjoiveydy.html

[T39] Lua：模式匹配
来源：http://hz.tian-w.cn/gtvqdhroll.html

string.find(s, "%d+")
来源：http://hz.xinyue.icu/gteqskjfam.html

[T40] Lua：元表
来源：http://hz.guannengcc.top/gtcutjfpeb.html

setmetatable({}, { __index = base })
来源：http://hz.svipenyu.cn/gtckuuczxd.html

[T41] Perl：Hello World
来源：http://hz.jlsjyb.cn/gtwxfihncq.html

print "Hello\n";
来源：http://hz.hfpthk.cn/gthtmomiee.html

[T42] Perl：变量类型
来源：http://hz.chenlongwang.top/gtyzyqfhwq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yongpay.top/gtweiisaks.html

[T43] Perl：字符串插值
来源：http://hz.yonumen.top/gtuwnmudrn.html

"值: $a"
来源：http://hz.snrcjt.cn/gtevekyhwh.html

[T44] Perl：条件
来源：http://hz.pengpengdd.cyou/gtzvjtsphl.html

if ($a > 0) { print "正"; }
来源：http://hz.gotoacloud.top/gtrproyilk.html

[T45] Perl：数组遍历
来源：http://hz.gzhubu.top/gtqzzeooea.html

for my $x (@arr) { print $x; }
来源：http://hz.redwolf501.top/gtwvrtgayw.html

[T46] Perl：哈希操作
来源：http://hz.chenlongwang.top/gtcdsojzlr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zhongyouzk.top/gtgzslybir.html

[T47] Perl：正则捕获
来源：http://hz.ppjwa.cn/gtrwkyrhiq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.quarkkingdee.top/gtpblfzsbk.html

[T48] Perl：正则替换
来源：http://hz.birdmap.top/gtzblmiwfr.html

$s =~ s/old/new/g;
来源：http://hz.vqdsnc.cn/gtlxuvdndv.html

[T49] Perl：函数
来源：http://hz.fengsongda.top/gtbnpsvznu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.xziqi.cn/gtmgyifeai.html

[T50] Perl：逐行读文件
来源：http://hz.guannengcc.top/gtkgpayzvm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.nanxuanxn.top/gttrligwxk.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.meibo888.top/gtgalcvtja.html

[T51] Scala：Hello World
来源：http://hz.yonumen.top/gtdtakrxun.html

println("Hello")
来源：http://hz.yueranfly.top/gtraivrfdx.html

[T52] Scala：变量
来源：http://hz.316326.xyz/gtcluzrpbl.html

val a = 1;  var b = 2
来源：http://hz.hammf.cn/gtwolwpvuq.html

[T53] Scala：字符串插值
来源：http://hz.tanke756.top/gtevamfxbl.html

s"值: $b"
来源：http://hz.cqqwz.cn/gtcwqvlzcf.html

[T54] Scala：集合映射
来源：http://hz.dianchejie.cn/gtnmdtcwsq.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.zdqjudy.top/gtbaipnwhy.html

[T55] Scala：集合过滤
来源：http://hz.pengpengdd.cyou/gtnovtocsc.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.havefunace.top/gtpssnpoyq.html

[T56] Scala：样例类
来源：http://hz.shzxlz.cn/gtofeznjst.html

case class User(name: String, age: Int)
来源：http://hz.hongshengwenyu.top/gtgxtszevg.html

[T57] Scala：模式匹配
来源：http://hz.xuanzx.com/gtkditkrrc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.jlsjyb.cn/gtvvkwdfep.html

[T58] Scala：函数定义
来源：http://hz.birdmap.top/gtoemyixdn.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.andypj.xyz/gthhheedvs.html

[T59] Scala：循环
来源：http://hz.zdqjudy.top/gtqyvyrthy.html

for (i <- 1 to 10) println(i)
来源：http://hz.yvedp.cn/gtpzuljgks.html

[T60] Scala：折叠
来源：http://hz.yangfankeji.com/gtemhfreuf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.52xcode.cn/gtrnuzkxwg.html

================================================================================
来源：http://hz.ehwqpu.com/gtigingtlg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.52xcode.cn/gtkkcqzdof.html

================================================================================
来源：http://hz.zhijiandao.cn/gtiklhprbm.html

[U01] Py：创建虚拟环境
来源：http://hz.jyoumei.cn/gtqdocluhh.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.cheryme.top/gtfuqyoolb.html

[U02] Py：导出 / 安装依赖
来源：http://hz.zhixingplan.top/gtoovdddwe.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yvedp.cn/gtaaresfqs.html

[U03] Py：加载 .env 配置
来源：http://hz.yj202588.top/gtulvmijhx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.feifeiyinyue.top/gtnxkdycmv.html

[U04] Py：变量调试打印
来源：http://hz.tianlin.xyz/gtdnvfrcvz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.sweek.top/gtpatgkwpg.html

[U05] Py：列表去重且保序
来源：http://hz.ehwqpu.com/gtnfeycrmm.html

list(dict.fromkeys(arr))
来源：http://hz.ywan-chungtsiang.top/gtprcbvzam.html

[U06] Py：合并两个字典
来源：http://hz.zhengqikj.top/gtcxkwjhrj.html

{**a, **b}
来源：http://hz.fzhhl.top/gtddjspjdi.html

[U07] Py：反转字典键值
来源：http://hz.andypj.xyz/gtkfmkzavy.html

{v: k for k, v in d.items()}
来源：http://hz.chenlongwang.top/gtijxonruw.html

[U08] Py：展平二维列表
来源：http://hz.yuanzhike.top/gtupgseaty.html

[y for x in nested for y in x]
来源：http://hz.yuxming.cn/gtnlndgcqp.html

[U09] Py：字典取最大值的键
来源：http://hz.hammf.cn/gtxunoxdxo.html

max(d, key=d.get)
来源：http://hz.mhx1999.top/gtfroctwnd.html

[U10] Py：按值排序字典
来源：http://hz.yvedp.cn/gtzkwamimz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.hnxiangtu.top/gtfofoosob.html

[U11] Py：生成器表达式
来源：http://hz.jlsjyb.cn/gtyumwytgo.html

(x * 2 for x in arr)
来源：http://hz.yj202588.top/gtvylnleyi.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.hfpthk.cn/gtmsjafsxp.html

Counter(arr).most_common(3)
来源：http://hz.316326.xyz/gtmpkadudi.html

[U13] Py：固定长度队列
来源：http://hz.hnxiangtu.top/gtwhvluklg.html

deque(maxlen=10)
来源：http://hz.jyoumei.cn/gtjfqpfydu.html

[U14] Py：分组收集到列表
来源：http://hz.chenlongwang.top/gtfstvnkho.html

defaultdict(list)
来源：http://hz.xuetiantiany.cn/gtaxzjuxbg.html

[U15] Py：高精度计时
来源：http://hz.hywenlv.cn/gtoyaduoom.html

t = time.perf_counter()
来源：http://hz.jinghuilouyu.cn/gtptevmlmq.html

[U16] Py：命令行参数解析
来源：http://hz.xziqi.cn/gtidfdhhzd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.daxiang520.top/gtuuvvexey.html

[U17] Py：初始化日志
来源：http://hz.shanyushiyangtech.top/gthjtxnszt.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.xingfuxueyuan.xyz/gtvuiikqio.html

[U18] Py：预编译正则
来源：http://hz.c1oappe.top/gtstncnchk.html

pat = re.compile(r"\d+")
来源：http://hz.tanke756.top/gtiaddryjn.html

[U19] Py：正则替换带回调
来源：http://hz.nanxinkj.top/gtfdygwhpf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.316326.xyz/gtrqrbfsgs.html

[U20] Py：缓存函数结果
来源：http://hz.dashuyun.cn/gtawzoykti.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jianghu66.top/gtzcheyzpi.html

[U21] Py：自定义上下文管理器
来源：http://hz.aibaodan.cn/gtqmlhcgur.html

@contextlib.contextmanager
来源：http://hz.chenlongwang.top/gtpnnijzbe.html

[U22] Py：矩阵转置
来源：http://hz.wangshuangyany.cn/gtvzrmqfke.html

list(zip(*m))
来源：http://hz.9152youxi.cn/gtgoixktbi.html

[U23] Py：分块读取大文件
来源：http://hz.cqqwz.cn/gtzcumdfhe.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.jinyuanbaomall.cn/gtbnlabqjt.html

[U24] Py：路径操作
来源：http://hz.jianghu66.top/gtfoaiogml.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.haohaochexian.top/gtvrbxwfcs.html

[U25] Py：CSV 按字典读
来源：http://hz.gaohongyu789.top/gtpuzqwvgs.html

csv.DictReader(f)
来源：http://hz.tian-w.cn/gtfoqqawzf.html

[U26] Py：并发下载
来源：http://hz.hnqzz.top/gtvkxefxyy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.shanyushiyangkeji.top/gtredvkszt.html

[U27] Py：异步 HTTP
来源：http://hz.wangdashe.top/gtuymlvxwa.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.quarkkingdee.top/gtpkjngdgx.html

[U28] Py：类型别名
来源：http://hz.pycfn.com/gtwwlmhjzp.html

UserId = int
来源：http://hz.chenjidiqi.icu/gtvuwapwts.html

[U29] Py：属性校验
来源：http://hz.hywenlv.cn/gtqgkjdmqo.html

@property 与 @x.setter 配合
来源：http://hz.aizwys.cn/gtmlibndko.html

[U30] Py：数据类
来源：http://hz.9152youxi.cn/gttgamfpeb.html

@dataclass(slots=True)
来源：http://hz.hammf.cn/gtmyrrrndf.html

[U31] Py：单测
来源：http://hz.andypj.xyz/gtyfrdkfaa.html

python -m pytest -q
来源：http://hz.yanxiufei.cn/gtbcxfvkqm.html

[U32] Py：代码格式化
来源：http://hz.yangfankeji.com/gtojqrypqd.html

ruff format . && ruff check --fix .
来源：http://hz.0kj1m.cn/gtukdmgjwr.html

[U33] Py：打包发布
来源：http://hz.andypj.xyz/gtqpvyyzvi.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.jlsjyb.cn/gtwgcepbky.html

[U34] Py：判断编码
来源：http://hz.yonumen.top/gtpfvzxirh.html

chardet.detect(raw)
来源：http://hz.jinqigfzy.top/gtbzwvwspd.html


<!-- 参考信息 -->