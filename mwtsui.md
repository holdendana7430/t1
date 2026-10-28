代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jianghu66.top/gtldwhuxvr.html

[S13] C：宏定义
来源：http://hz.hnqzz.top/gtelcoosjn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.meibo888.top/gtyfsmdlbs.html

[S14] C：枚举
来源：http://hz.meibo888.top/gtfaspxfdq.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zycfv.cn/gtwrnlvyhp.html

[S15] C：类型转换
来源：http://hz.ivvv.top/gtepgwvzvp.html

(double) a / b
来源：http://hz.vqdsnc.cn/gtlgzwrvfs.html

[S16] C：位操作置位
来源：http://hz.yj20258.top/gtzztrsrpn.html

x |= (1 << 3);
来源：http://hz.meibo888.top/gtsubxdptn.html

[S17] C：安全拼接字符串
来源：http://hz.cashguo.top/gtbthyzvtl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.cqqwz.cn/gtwtojcagx.html

[S18] C：命令行参数
来源：http://hz.shangyingyoupin.top/gtosgznwds.html

int main(int argc, char **argv)
来源：http://hz.xylfe.cn/gtariukurk.html

[S19] C：快速排序
来源：http://hz.yongpay.top/gtnymxmigk.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hysaishi.cn/gtydddxfcv.html

[S20] C：二分查找
来源：http://hz.xuetiantiany.cn/gttlatypdu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.mhx1999.top/gtorjuqapu.html

[S21] C：字符类别判断
来源：http://hz.zhijiandao.cn/gtrkmmmnpf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.nwbrower.top/gttunrlskl.html

[S22] C：字符串转数字
来源：http://hz.shzxlz.cn/gtuczygdhi.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhaomingkeji.xyz/gtjfvidaxs.html

[S23] C：随机数
来源：http://hz.zhoulong.xyz/gtbfynftqh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.daxiang520.top/gtgrdiqctv.html

[S24] C：获取本地时间
来源：http://hz.iojbl.cn/gtkrgclnax.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.andypj.xyz/gtsofcijwk.html

[S25] C：内存拷贝
来源：http://hz.shzxlz.cn/gttyphmbau.html

memcpy(dst, src, n);
来源：http://hz.pengpengdd.cyou/gtizmupigg.html

[S26] C：内存清零
来源：http://hz.316326.xyz/gtebbpvagw.html

memset(a, 0, sizeof a);
来源：http://hz.jinghuilouyu.cn/gtwffwmrfh.html

[S27] C：定义常量
来源：http://hz.yanxiufei.cn/gtbrldbtag.html

const double PI = 3.14159;
来源：http://hz.cucudq.cn/gtmvoabaks.html

[S28] C：静态变量
来源：http://hz.zdqjudy.top/gtnhxodgho.html

static int counter = 0;
来源：http://hz.cheryme.top/gtjqmzheae.html

[S29] C：变参函数
来源：http://hz.feifeiyinyue.top/gtgjvcuxyb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ivvv.top/gtprqejtwu.html

[S30] C：头文件保护
来源：http://hz.zhijiandao.cn/gtklbffugh.html

#ifndef X_H
来源：http://hz.svipenyu.cn/gtencuhzdz.html

#define X_H
来源：http://hz.52xcode.cn/gtpdyvgqwd.html

#endif
来源：http://hz.zhixingplan.top/gtnptrygng.html

[S31] C++：Hello World
来源：http://hz.sweek.top/gttiqmophq.html

#include <iostream>
来源：http://hz.zhoulong.xyz/gtnvbtojlm.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.bjfxy.top/gtkrtmgzhi.html

[S32] C++：字符串
来源：http://hz.yueranfly.top/gthbtsytou.html

std::string s = "hi";  s += "!";
来源：http://hz.daria6918.cn/gtxlwwhxwk.html

[S33] C++：vector 增删
来源：http://hz.yonumen.top/gtrxcivlya.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yonumen.top/gtknuxhvuh.html

[S34] C++：遍历 vector
来源：http://hz.c1oappe.top/gtkqkzfiyv.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.quarkkingdee.top/gtjxvvvrem.html

[S35] C++：map
来源：http://hz.hammf.cn/gtoimyjngq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.0kj1m.cn/gtufzfbrnd.html

[S36] C++：unordered_map
来源：http://hz.zhengqikj.top/gtlvzqkqqp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xuetiantiany.cn/gtermmgdyd.html

[S37] C++：set
来源：http://hz.ywan-chungtsiang.top/gtasastuua.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.feifeiyinyue.top/gtcfzfooti.html

[S38] C++：排序
来源：http://hz.ivvv.top/gtdxcsrqrl.html

std::sort(v.begin(), v.end());
来源：http://hz.bjfxy.top/gtrcchkneo.html

[S39] C++：自定义比较器排序
来源：http://hz.nanxinkj.top/gtdslucbvk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.xziqi.cn/gtbebefdpw.html

[S40] C++：查找元素
来源：http://hz.daxiang520.top/gtskyqwjeh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.daxiang520.top/gtpoufjnof.html

[S41] C++：类与构造函数
来源：http://hz.redwolf501.top/gtqwzvaogh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.gogol.net.cn/gtagultpom.html

[S42] C++：继承与虚函数
来源：http://hz.9152youxi.cn/gtbhhrryyq.html

class B : public Base { public: void f() override {} };
来源：http://hz.yuxming.cn/gtnmbwmmip.html

[S43] C++：智能指针
来源：http://hz.zycfv.cn/gtkbisknlv.html

auto p = std::make_unique<int>(5);
来源：http://hz.yangfankeji.com/gthtfpyobd.html

[S44] C++：引用传参
来源：http://hz.cdnleiting.top/gtkyzqwyle.html

void inc(int &x) { ++x; }
来源：http://hz.cucudq.cn/gtooasqcnb.html

[S45] C++：lambda
来源：http://hz.jqgfzy.top/gtijajedaa.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.dashuyun.cn/gtqrwwxxfp.html

[S46] C++：函数模板
来源：http://hz.yvedp.cn/gtkjtktscu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yangfankeji.com/gtdkirdxwf.html

[S47] C++：结构化绑定遍历
来源：http://hz.yueranfly.top/gternsibrb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhoulong.xyz/gttisdmtkp.html

[S48] C++：逐行读文件
来源：http://hz.daria6918.cn/gtdhtrfgdo.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yanxiufei.cn/gtmplceysp.html

while (std::getline(in, line)) { }
来源：http://hz.yangfankeji.com/gtwahkliwi.html

[S49] C++：写文件
来源：http://hz.c1oappe.top/gtojaechcz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ywan-chungtsiang.top/gtpsbubamo.html

[S50] C++：格式化数字
来源：http://hz.xingfuxueyuan.xyz/gtywfabogi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jqgfzy.top/gtmzpqtosk.html

[S51] C++：显式类型转换
来源：http://hz.kuanghao11.cn/gtgxyrlufr.html

static_cast<double>(a) / b
来源：http://hz.jinghuilouyu.cn/gtwajftehx.html

[S52] C++：const 与 noexcept
来源：http://hz.xingfuxueyuan.xyz/gtsunikjoi.html

int size() const noexcept { return n_; }
来源：http://hz.smart0.xyz/gtxwwhjkxq.html

[S53] C++：移动语义
来源：http://hz.nanxuanxn.top/gtvxozztjr.html

std::vector<int> w = std::move(v);
来源：http://hz.jiagoushi.top/gtzmhdcjld.html

[S54] C++：异常处理
来源：http://hz.hnxiangtu.top/gtgsgptndm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.xziqi.cn/gtaslwfwyv.html

[S55] C++：结构化绑定
来源：http://hz.yuxming.cn/gttorcybnz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.gaohongyu789.top/gtljpzzvue.html

[S56] C++：optional
来源：http://hz.0kj1m.cn/gtaaxoznmn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhongyouzk.top/gtwirvojrs.html

[S57] C++：编译期常量
来源：http://hz.fzhhl.top/gteytrcjqc.html

constexpr int N = 10;
来源：http://hz.tanke756.top/gtglzxtyjh.html

[S58] C++：命名空间
来源：http://hz.yj20258.top/gtomjbccfn.html

namespace ns { int f() { return 1; } }
来源：http://hz.xziqi.cn/gtcuubmnaj.html

[S59] C++：静态断言
来源：http://hz.birdmap.top/gtkvkdvqme.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jinyuanbaomall.cn/gtjleiheui.html

[S60] C++：遍历并删除元素
来源：http://hz.kuanghao11.cn/gtozkgrvig.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.ydjk.org.cn/gtbgrgbvhv.html

================================================================================
来源：http://hz.iojbl.cn/gtfzdrharm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yj20258888.top/gttrtrrmkm.html

================================================================================
来源：http://hz.zhoulong.xyz/gtqfnunupg.html

[T01] Kotlin：Hello World
来源：http://hz.yangfankeji.com/gtmiqwfnlp.html

println("Hello")
来源：http://hz.zhaomingkeji.xyz/gtacsseezo.html

[T02] Kotlin：变量
来源：http://hz.0kj1m.cn/gttsflbnvk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.9152youxi.cn/gtdsylitad.html

[T03] Kotlin：字符串模板
来源：http://hz.jinghuilouyu.cn/gtahkofrxd.html

"值: $b"
来源：http://hz.fengsongda.top/gtcrwudorz.html

[T04] Kotlin：空安全
来源：http://hz.cashguo.top/gtzhwpfhor.html

val n: String? = null;  n?.length
来源：http://hz.chenjidiqi.icu/gtctuygsar.html

[T05] Kotlin：when 表达式
来源：http://hz.quarkkingdee.top/gtnnxguftb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jlsjyb.cn/gthmzyhlzy.html

[T06] Kotlin：集合映射
来源：http://hz.zhixingplan.top/gtxymsbqml.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.wangdashe.top/gtoxpobfxj.html

[T07] Kotlin：集合过滤
来源：http://hz.c1oappe.top/gtfnkhqvah.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.cheryme.top/gtejrpbzwo.html

[T08] Kotlin：数据类
来源：http://hz.hnqzz.top/gtntaakuuf.html

data class User(val name: String, val age: Int)
来源：http://hz.zhoulong.xyz/gtfvhdbcex.html

[T09] Kotlin：扩展函数
来源：http://hz.tian-w.cn/gtedqcqpmb.html

fun String.exclaim() = this + "!"
来源：http://hz.shzxlz.cn/gtpixsyisw.html

[T10] Kotlin：默认参数
来源：http://hz.gzhubu.top/gtmmqthxnv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hysaishi.cn/gtskritcbs.html

[T11] Kotlin：协程
来源：http://hz.ydjk.org.cn/gtahyqelbr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.pycfn.com/gtlgqbnsms.html

[T12] Kotlin：解构声明
来源：http://hz.yueranfly.top/gtcibyulvg.html

val (a, b) = Pair(1, 2)
来源：http://hz.cdnleiting.top/gtcjnefefq.html

[T13] Kotlin：只读 Map
来源：http://hz.jinghuilouyu.cn/gtztcpntvn.html

val m = mapOf("a" to 1)
来源：http://hz.kuanghao11.cn/gtjwbnqgnx.html

[T14] Kotlin：循环
来源：http://hz.wangshuangyany.cn/gtulyoyedf.html

for (i in 1..10) println(i)
来源：http://hz.pengpengdd.cyou/gtbljgzyss.html

[T15] Kotlin：接口
来源：http://hz.birdmap.top/gtedmnfsnm.html

interface Shape { fun area(): Double }
来源：http://hz.xylfe.cn/gtvvfjujff.html

[T16] Swift：Hello World
来源：http://hz.ydjk.org.cn/gtxrcbpukm.html

print("Hello")
来源：http://hz.c1oappe.top/gtobtrozzs.html

[T17] Swift：变量与常量
来源：http://hz.c1oappe.top/gtdcwluelv.html

var a = 1;  let b = 2
来源：http://hz.yueranfly.top/gtdixhdysz.html

[T18] Swift：字符串插值
来源：http://hz.ywan-chungtsiang.top/gtgenjzzyr.html

"值: \(b)"
来源：http://hz.pycfn.com/gtzwceyvma.html

[T19] Swift：可选绑定
来源：http://hz.hnxiangtu.top/gtytyrndzk.html

if let n = opt { print(n) }
来源：http://hz.cdnleiting.top/gtdqqrwtrd.html

[T20] Swift：数组操作
来源：http://hz.wangdashe.top/gtewgutuqa.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.aizwys.cn/gtodlttrlk.html

[T21] Swift：遍历
来源：http://hz.hysaishi.cn/gteigcncge.html

for x in a { print(x) }
来源：http://hz.aibaodan.cn/gtesrsyluj.html

[T22] Swift：字典
来源：http://hz.cqqwz.cn/gtflwwqkab.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.chenzaomai.com/gthsahmpov.html

[T23] Swift：函数
来源：http://hz.jiagoushi.top/gtgmntokcm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.chenzaomai.com/gtzyfiwivw.html

[T24] Swift：闭包
来源：http://hz.hywenlv.cn/gthshidiok.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jinyuanbaomall.cn/gtfarzryyz.html

[T25] Swift：结构体
来源：http://hz.shangyingyoupin.top/gtouquyjpt.html

struct P { var x: Int }
来源：http://hz.feifeiyinyue.top/gtfuzjzsvf.html

[T26] Swift：类与重写
来源：http://hz.jyoumei.cn/gtluhrozap.html

class A: Base { override func f() {} }
来源：http://hz.haohaochexian.top/gtaagqkpuw.html

[T27] Swift：错误处理
来源：http://hz.sysykeji.top/gtqkorbmsc.html

do { try f() } catch { print(error) }
来源：http://hz.daxiang520.top/gtyacetzcn.html

[T28] Swift：枚举
来源：http://hz.zhoulong.xyz/gtfzzpjspk.html

enum Color { case red, green }
来源：http://hz.xuanzx.com/gtinsnvymp.html

[T29] Swift：guard 提前返回
来源：http://hz.316326.xyz/gtgsighbwy.html

guard let x = opt else { return }
来源：http://hz.daria6918.cn/gtxgpecmxn.html

[T30] Swift：协议
来源：http://hz.guowangkeji.top/gtgtuzunmm.html

protocol Shape { func area() -> Double }
来源：http://hz.jlsjyb.cn/gtgvtlfaec.html

[T31] Lua：Hello World
来源：http://hz.yonumen.top/gthemjqdnj.html

print("Hello")
来源：http://hz.gaohongyu789.top/gtdmabwwcr.html

[T32] Lua：局部变量
来源：http://hz.zhongyouzk.top/gtjsytqsyc.html

local a = 1
来源：http://hz.meibo888.top/gtrsuvudek.html

[T33] Lua：表（数组）
来源：http://hz.c1oappe.top/gtgojtvldb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.hfpthk.cn/gtpbchjmub.html

[T34] Lua：遍历表
来源：http://hz.hnqzz.top/gtudkzmpnb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.aizwys.cn/gtlsyfyxqp.html

[T35] Lua：字典表
来源：http://hz.zhixingplan.top/gtyirzkqlt.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jinyuanbaomall.cn/gtqndfgavp.html

[T36] Lua：函数
来源：http://hz.ydjk.org.cn/gttdirrzdq.html

function add(a, b) return a + b end
来源：http://hz.zycfv.cn/gtyaanpguh.html

[T37] Lua：字符串拼接
来源：http://hz.jinyuanbaomall.cn/gtgshumxrh.html

"a" .. "b"
来源：http://hz.ybcxt.top/gtmianjpss.html

[T38] Lua：条件
来源：http://hz.chenlongwang.top/gtsrsfgdyx.html

if x > 0 then print("正") end
来源：http://hz.hywenlv.cn/gtbjbyrrgt.html

[T39] Lua：模式匹配
来源：http://hz.chenjidiqi.icu/gtevzrvlbn.html

string.find(s, "%d+")
来源：http://hz.kuanghao11.cn/gtozwztnbg.html

[T40] Lua：元表
来源：http://hz.yj202588.top/gtahoarnkx.html

setmetatable({}, { __index = base })
来源：http://hz.9152youxi.cn/gtpvvrlyam.html

[T41] Perl：Hello World
来源：http://hz.zhongyouzk.top/gtsxkahzzg.html

print "Hello\n";
来源：http://hz.bjfxy.top/gtprieyglh.html

[T42] Perl：变量类型
来源：http://hz.iojbl.cn/gtddbclujd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.aizwys.cn/gtkhzczzan.html

[T43] Perl：字符串插值
来源：http://hz.yongpay.top/gtzqridcoo.html

"值: $a"
来源：http://hz.ppjwa.cn/gtrctmdgps.html

[T44] Perl：条件
来源：http://hz.shanyushiyangtech.top/gtcunhcpin.html

if ($a > 0) { print "正"; }
来源：http://hz.jqgfzy.top/gtosndmeyv.html

[T45] Perl：数组遍历
来源：http://hz.jinyuanbaomall.cn/gtbsnwlbrs.html

for my $x (@arr) { print $x; }
来源：http://hz.vqdsnc.cn/gtsiewipch.html

[T46] Perl：哈希操作
来源：http://hz.xuanzx.com/gtenhgrdlp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.havefunace.top/gtkmvpmfhh.html

[T47] Perl：正则捕获
来源：http://hz.redwolf501.top/gthxhkccmc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.vqdsnc.cn/gtsbxenppj.html

[T48] Perl：正则替换
来源：http://hz.sxryk.cn/gtgyknonsz.html

$s =~ s/old/new/g;
来源：http://hz.ywan-chungtsiang.top/gtexzghjwz.html

[T49] Perl：函数
来源：http://hz.yj20258888.top/gtsttzkuja.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.cucudq.cn/gtwzawqafi.html

[T50] Perl：逐行读文件
来源：http://hz.xylfe.cn/gtdtjaaqtb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.kuanghao11.cn/gtlzuyrphl.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.quarkkingdee.top/gtsxrkbstf.html

[T51] Scala：Hello World
来源：http://hz.c1oappe.top/gtbqabqzca.html

println("Hello")
来源：http://hz.hnqzz.top/gtypzmwrpv.html

[T52] Scala：变量
来源：http://hz.havefunace.top/gtjaqhuemz.html

val a = 1;  var b = 2
来源：http://hz.guannengcc.top/gtgwmsbqsq.html

[T53] Scala：字符串插值
来源：http://hz.shangyingyoupin.top/gtzfwyenib.html

s"值: $b"
来源：http://hz.hammf.cn/gthhhdsred.html

[T54] Scala：集合映射
来源：http://hz.ywan-chungtsiang.top/gtgjhmjwkl.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.dianchejie.cn/gtjvqbppmw.html

[T55] Scala：集合过滤
来源：http://hz.cdnleiting.top/gtfpuopcnp.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.dashuyun.cn/gtujbmbcyj.html

[T56] Scala：样例类
来源：http://hz.dashuyun.cn/gtzdpfxmqu.html

case class User(name: String, age: Int)
来源：http://hz.shangyingyoupin.top/gtbwlndplv.html

[T57] Scala：模式匹配
来源：http://hz.shanyushiyangkeji.top/gtpfpiuyct.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.snrcjt.cn/gtocmwptcq.html

[T58] Scala：函数定义
来源：http://hz.9152youxi.cn/gthxwbkhro.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.hywenlv.cn/gtuzaoxlkf.html

[T59] Scala：循环
来源：http://hz.bjfxy.top/gtnshijsvm.html

for (i <- 1 to 10) println(i)
来源：http://hz.tianlin.xyz/gtvonpyjjt.html

[T60] Scala：折叠
来源：http://hz.yvedp.cn/gtojwridip.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yonumen.top/gtzlikarll.html

================================================================================
来源：http://hz.daxiang520.top/gtrlzhreks.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jqgufenzy.top/gttdnmqqyx.html

================================================================================
来源：http://hz.hysaishi.cn/gtejcnxcxd.html

[U01] Py：创建虚拟环境
来源：http://hz.ybcxt.top/gtobkltdaw.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.nanxinkj.top/gtkmbsykvv.html

[U02] Py：导出 / 安装依赖
来源：http://hz.dianchejie.cn/gtlvseuofk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.xylfe.cn/gtbcszlhvb.html

[U03] Py：加载 .env 配置
来源：http://hz.zhongyouzk.top/gtlwamsotx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.316326.xyz/gtjxeuvbxg.html

[U04] Py：变量调试打印
来源：http://hz.yongpay.top/gthpejwcyk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.daxiang520.top/gtodjjszba.html

[U05] Py：列表去重且保序
来源：http://hz.redwolf501.top/gtopklxuid.html

list(dict.fromkeys(arr))
来源：http://hz.guannengcc.top/gtzrstwvof.html

[U06] Py：合并两个字典
来源：http://hz.jinqigufen.top/gtfndlpohk.html

{**a, **b}
来源：http://hz.ydjk.org.cn/gtchboebtg.html

[U07] Py：反转字典键值
来源：http://hz.hywenlv.cn/gthiqjnyyl.html

{v: k for k, v in d.items()}
来源：http://hz.jiagoushi.top/gtdbpjmoua.html

[U08] Py：展平二维列表
来源：http://hz.guowangkeji.top/gtqhagsaml.html

[y for x in nested for y in x]
来源：http://hz.nanxuanxn.top/gtvxcyhnma.html

[U09] Py：字典取最大值的键
来源：http://hz.shanyushiyangkeji.top/gtoettvukq.html

max(d, key=d.get)
来源：http://hz.shangyingyoupin.top/gtdzqrhsdn.html

[U10] Py：按值排序字典
来源：http://hz.jinghuilouyu.cn/gtcfutayrs.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.gotoacloud.top/gthwnwueip.html

[U11] Py：生成器表达式
来源：http://hz.xuetiantiany.cn/gttfrtalcz.html

(x * 2 for x in arr)
来源：http://hz.sweek.top/gttedtxsoe.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.aibaodan.cn/gtmukezsaf.html

Counter(arr).most_common(3)
来源：http://hz.nwbrower.top/gtphdhfljm.html

[U13] Py：固定长度队列
来源：http://hz.yanxiufei.cn/gtkucxwhza.html

deque(maxlen=10)
来源：http://hz.hfpthk.cn/gtxldcovvo.html

[U14] Py：分组收集到列表
来源：http://hz.jiagoushi.top/gtzixlqous.html

defaultdict(list)
来源：http://hz.nanxuanxn.top/gtmzkcmjqd.html

[U15] Py：高精度计时
来源：http://hz.sweek.top/gtaacaykjt.html

t = time.perf_counter()
来源：http://hz.gotoacloud.top/gtfjkxloqy.html

[U16] Py：命令行参数解析
来源：http://hz.tanke756.top/gtophwihjk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.iojbl.cn/gtldxuxfae.html

[U17] Py：初始化日志
来源：http://hz.nanxuanxn.top/gtdxzsgoab.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.shanyushiyangkeji.top/gtkvhrybjb.html

[U18] Py：预编译正则
来源：http://hz.yuanzhike.top/gtnhcnjufy.html

pat = re.compile(r"\d+")
来源：http://hz.yangfankeji.com/gtpvkbnjbp.html

[U19] Py：正则替换带回调
来源：http://hz.hywenlv.cn/gtkiyjtcsu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.xylfe.cn/gtkpiihxwu.html

[U20] Py：缓存函数结果
来源：http://hz.xuanzx.com/gtxjjlcbqb.html

@functools.lru_cache(maxsize=None)
来源：http://hz.tian-w.cn/gtbcrdfxlo.html

[U21] Py：自定义上下文管理器
来源：http://hz.ywan-chungtsiang.top/gtohyscqpx.html

@contextlib.contextmanager
来源：http://hz.jqgfzy.top/gtlppovtte.html

[U22] Py：矩阵转置
来源：http://hz.jyoumei.cn/gtatbacqsq.html

list(zip(*m))
来源：http://hz.haohaochexian.top/gtbofrtnqj.html

[U23] Py：分块读取大文件
来源：http://hz.dashuyun.cn/gtwjtybfwy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yvedp.cn/gtljiraanr.html

[U24] Py：路径操作
来源：http://hz.havefunace.top/gtypcovcuz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.jlsjyb.cn/gtabxxquje.html

[U25] Py：CSV 按字典读
来源：http://hz.guannengcc.top/gtreeunziu.html

csv.DictReader(f)
来源：http://hz.jinghuilouyu.cn/gtkfrszdww.html

[U26] Py：并发下载
来源：http://hz.yuxming.cn/gtmpodszqx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.feifeiyinyue.top/gtxnkqnwia.html

[U27] Py：异步 HTTP
来源：http://hz.shangyingyoupin.top/gtsmnbskft.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.gogol.net.cn/gtxjyyhiwb.html

[U28] Py：类型别名
来源：http://hz.cashguo.top/gtjgxvzvpd.html

UserId = int
来源：http://hz.xingfuxueyuan.xyz/gtkbrcvzdr.html

[U29] Py：属性校验
来源：http://hz.yj20258888.top/gtkdhkfvyr.html

@property 与 @x.setter 配合
来源：http://hz.jiagoushi.top/gtjyhnlecl.html

[U30] Py：数据类
来源：http://hz.zhixingplan.top/gtajekxsmj.html

@dataclass(slots=True)
来源：http://hz.jinqigufen.top/gtjeqcsfms.html

[U31] Py：单测
来源：http://hz.fengsongda.top/gtbbutjcxp.html

python -m pytest -q
来源：http://hz.9152youxi.cn/gtfiibrbwg.html

[U32] Py：代码格式化
来源：http://hz.shangyingyoupin.top/gthlwkvwyy.html

ruff format . && ruff check --fix .
来源：http://hz.yj20258.top/gtejxcsars.html

[U33] Py：打包发布
来源：http://hz.yj20258.top/gtzpidzdvb.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.sufxvd.cn/gtvsqenlal.html

[U34] Py：判断编码
来源：http://hz.yueranfly.top/gtxkgpxrez.html

chardet.detect(raw)
来源：http://hz.cqqwz.cn/gtdowxazed.html

[U35] Py：发送邮件
来源：http://hz.jqgfzy.top/gtjgawlrvx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.ppjwa.cn/gtwbzyqebm.html

[U36] Py：定时任务
来源：http://hz.snrcjt.cn/gtfauarhxe.html

schedule.every(10).minutes.do(job)
来源：http://hz.fzhhl.top/gtziqfduko.html


<!-- 参考信息 -->