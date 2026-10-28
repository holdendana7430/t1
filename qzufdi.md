代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.cqqwz.cn/gtngbwpioi.html

[S13] C：宏定义
来源：http://hz.yonumen.top/gtzlcuovdj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.gogol.net.cn/gtqiyjvbwj.html

[S14] C：枚举
来源：http://hz.wangshuangyany.cn/gtnrrkduir.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.wangdashe.top/gtyuejtsdz.html

[S15] C：类型转换
来源：http://hz.zycfv.cn/gtwciesczx.html

(double) a / b
来源：http://hz.yanxiufei.cn/gtxlycrvpp.html

[S16] C：位操作置位
来源：http://hz.feifeiyinyue.top/gtvzxxkrzf.html

x |= (1 << 3);
来源：http://hz.jiagoushi.top/gtxdfzkdtj.html

[S17] C：安全拼接字符串
来源：http://hz.jyoumei.cn/gthoujmylz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jinyuanbaomall.cn/gtxavqiaqk.html

[S18] C：命令行参数
来源：http://hz.zhiwuduotai.top/gtygscafak.html

int main(int argc, char **argv)
来源：http://hz.chenzaomai.com/gtvrojzxbj.html

[S19] C：快速排序
来源：http://hz.pengpengdd.cyou/gtxqieusvk.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jiagoushi.top/gtnkdmonnk.html

[S20] C：二分查找
来源：http://hz.zhoulong.xyz/gtvlcxusop.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhongyouzk.top/gteoswmyle.html

[S21] C：字符类别判断
来源：http://hz.iojbl.cn/gtlclrphlt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.snrcjt.cn/gtmqizdxeu.html

[S22] C：字符串转数字
来源：http://hz.dashuyun.cn/gtmvkclnfk.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jlsjyb.cn/gtegaavovd.html

[S23] C：随机数
来源：http://hz.gogol.net.cn/gtbdxqxigp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.shzxlz.cn/gtptoubmzn.html

[S24] C：获取本地时间
来源：http://hz.snrcjt.cn/gtviydeoil.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.shangyingyoupin.top/gtesiaaqxf.html

[S25] C：内存拷贝
来源：http://hz.redwolf501.top/gteyiotgvx.html

memcpy(dst, src, n);
来源：http://hz.jinghuilouyu.cn/gtyvjtuyar.html

[S26] C：内存清零
来源：http://hz.zhongyouzk.top/gtnbgkfslx.html

memset(a, 0, sizeof a);
来源：http://hz.jinghuilouyu.cn/gtuawzgkrm.html

[S27] C：定义常量
来源：http://hz.xziqi.cn/gtpanosogl.html

const double PI = 3.14159;
来源：http://hz.shangyingyoupin.top/gtwsflzmlu.html

[S28] C：静态变量
来源：http://hz.sweek.top/gtiothamfc.html

static int counter = 0;
来源：http://hz.jqgfzy.top/gtlbzrufvz.html

[S29] C：变参函数
来源：http://hz.fengsongda.top/gtzucdtpct.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.sxryk.cn/gtyzkhrqpx.html

[S30] C：头文件保护
来源：http://hz.ywan-chungtsiang.top/gtwqmlllob.html

#ifndef X_H
来源：http://hz.yuanzhike.top/gtqakofovb.html

#define X_H
来源：http://hz.316326.xyz/gtqbqzdltv.html

#endif
来源：http://hz.redwolf501.top/gtstgmkoml.html

[S31] C++：Hello World
来源：http://hz.jinqigfzy.top/gtotscrmii.html

#include <iostream>
来源：http://hz.birdmap.top/gtinctnoij.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zycfv.cn/gtiidpdstl.html

[S32] C++：字符串
来源：http://hz.xuanzx.com/gtkphpkxvu.html

std::string s = "hi";  s += "!";
来源：http://hz.shangyingyoupin.top/gtroaethie.html

[S33] C++：vector 增删
来源：http://hz.ehwqpu.com/gtapuspetb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shuidangran.top/gtpgkcaron.html

[S34] C++：遍历 vector
来源：http://hz.yuxming.cn/gteplikkxj.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yvedp.cn/gtdhwzwskq.html

[S35] C++：map
来源：http://hz.ivvv.top/gtxopoqonw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nanxuanxn.top/gtogirkazx.html

[S36] C++：unordered_map
来源：http://hz.guannengcc.top/gtdarmukdq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yanxiufei.cn/gterncaclr.html

[S37] C++：set
来源：http://hz.ehwqpu.com/gtvkcgubqn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhijiandao.cn/gthpmkusgo.html

[S38] C++：排序
来源：http://hz.hnqzz.top/gtbolyuonc.html

std::sort(v.begin(), v.end());
来源：http://hz.sweek.top/gtoqvrytie.html

[S39] C++：自定义比较器排序
来源：http://hz.316326.xyz/gtflmffxwb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ywan-chungtsiang.top/gticcgafii.html

[S40] C++：查找元素
来源：http://hz.cheryme.top/gtqwuwxxis.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhaomingkeji.xyz/gtkiltqzzw.html

[S41] C++：类与构造函数
来源：http://hz.xingfuxueyuan.xyz/gtyvcrpmqk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhoulong.xyz/gtjukoharp.html

[S42] C++：继承与虚函数
来源：http://hz.fzhhl.top/gtscuppqzt.html

class B : public Base { public: void f() override {} };
来源：http://hz.shanyushiyangkeji.top/gtwipxltkg.html

[S43] C++：智能指针
来源：http://hz.ppjwa.cn/gthnmdrmdy.html

auto p = std::make_unique<int>(5);
来源：http://hz.jqgfzy.top/gtvivpdhnb.html

[S44] C++：引用传参
来源：http://hz.vqdsnc.cn/gttssqjovt.html

void inc(int &x) { ++x; }
来源：http://hz.c1oappe.top/gtnmpbxgdg.html

[S45] C++：lambda
来源：http://hz.pengpengdd.cyou/gttygxrwig.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.pycfn.com/gtskmcrqui.html

[S46] C++：函数模板
来源：http://hz.0kj1m.cn/gtiwngpqeb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.hnqzz.top/gthvcgqovg.html

[S47] C++：结构化绑定遍历
来源：http://hz.chenlongwang.top/gtybrgablx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.pycfn.com/gtppblyaaa.html

[S48] C++：逐行读文件
来源：http://hz.pengpengdd.cyou/gtpblbdfkx.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.dianchejie.cn/gtgkeqbkuj.html

while (std::getline(in, line)) { }
来源：http://hz.wangshuangyany.cn/gtumkveheh.html

[S49] C++：写文件
来源：http://hz.xuanzx.com/gtlicnhmwu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.0kj1m.cn/gtuaqciyft.html

[S50] C++：格式化数字
来源：http://hz.chenlongwang.top/gttuwozwwt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.chenzaomai.com/gtddylhbaq.html

[S51] C++：显式类型转换
来源：http://hz.jiagoushi.top/gtzfnfqexn.html

static_cast<double>(a) / b
来源：http://hz.svipenyu.cn/gteyivmpua.html

[S52] C++：const 与 noexcept
来源：http://hz.jqgfzy.top/gtshzlnzdm.html

int size() const noexcept { return n_; }
来源：http://hz.daria6918.cn/gtqapulmjh.html

[S53] C++：移动语义
来源：http://hz.snrcjt.cn/gtajetcitb.html

std::vector<int> w = std::move(v);
来源：http://hz.andypj.xyz/gtmuewshbh.html

[S54] C++：异常处理
来源：http://hz.jyoumei.cn/gtnzzbjfob.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jinghuilouyu.cn/gtwvqzkinh.html

[S55] C++：结构化绑定
来源：http://hz.yongpay.top/gtzmfkrrvb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.pycfn.com/gtmdzqwhal.html

[S56] C++：optional
来源：http://hz.0kj1m.cn/gtkwhpdvvk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.snrcjt.cn/gtzmcbtdxq.html

[S57] C++：编译期常量
来源：http://hz.nwbrower.top/gtpxbftxrr.html

constexpr int N = 10;
来源：http://hz.ivvv.top/gtrfifldub.html

[S58] C++：命名空间
来源：http://hz.andypj.xyz/gtlxkhwvnf.html

namespace ns { int f() { return 1; } }
来源：http://hz.ehwqpu.com/gtfgjvcbrv.html

[S59] C++：静态断言
来源：http://hz.gaohongyu789.top/gtpofffdss.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.chenzaomai.com/gtzzlkudej.html

[S60] C++：遍历并删除元素
来源：http://hz.cashguo.top/gtpsruswhp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.daria6918.cn/gtcfrcdjkd.html

================================================================================
来源：http://hz.tianlin.xyz/gtijyojdbb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.iojbl.cn/gtjmcopmfe.html

================================================================================
来源：http://hz.zycfv.cn/gttnvdsveu.html

[T01] Kotlin：Hello World
来源：http://hz.havefunace.top/gtdiduarzi.html

println("Hello")
来源：http://hz.haohaochexian.top/gtawxwnsos.html

[T02] Kotlin：变量
来源：http://hz.tianlin.xyz/gtiaalnyzq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.nanxuanxn.top/gtslolahlb.html

[T03] Kotlin：字符串模板
来源：http://hz.shanyushiyangtech.top/gtbuhncprq.html

"值: $b"
来源：http://hz.cucudq.cn/gttagavmcs.html

[T04] Kotlin：空安全
来源：http://hz.zhijiandao.cn/gtcjqfwaao.html

val n: String? = null;  n?.length
来源：http://hz.ydzc1.top/gtalvtkgti.html

[T05] Kotlin：when 表达式
来源：http://hz.ehwqpu.com/gtljzlexbw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ivvv.top/gttotjhsii.html

[T06] Kotlin：集合映射
来源：http://hz.gaohongyu789.top/gtawdtcndk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhijiandao.cn/gtlvjrzswu.html

[T07] Kotlin：集合过滤
来源：http://hz.smart0.xyz/gtvylpzezc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.snrcjt.cn/gtekrckghz.html

[T08] Kotlin：数据类
来源：http://hz.jinghuilouyu.cn/gtvovtdqim.html

data class User(val name: String, val age: Int)
来源：http://hz.sufxvd.cn/gtnhbhsndf.html

[T09] Kotlin：扩展函数
来源：http://hz.kuanghao11.cn/gtbhqhfqac.html

fun String.exclaim() = this + "!"
来源：http://hz.aibaodan.cn/gtdiyzutbz.html

[T10] Kotlin：默认参数
来源：http://hz.nwbrower.top/gtlycqlfwc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yuxming.cn/gtlqmxzphv.html

[T11] Kotlin：协程
来源：http://hz.nanxuanxn.top/gtrlbcbwzg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.ehwqpu.com/gtgwgczbpt.html

[T12] Kotlin：解构声明
来源：http://hz.zhengqikj.top/gtodyohqgc.html

val (a, b) = Pair(1, 2)
来源：http://hz.chenlongwang.top/gtyvquwbpb.html

[T13] Kotlin：只读 Map
来源：http://hz.hywenlv.cn/gtfllqhgnn.html

val m = mapOf("a" to 1)
来源：http://hz.hnxiangtu.top/gttlespiwj.html

[T14] Kotlin：循环
来源：http://hz.hysaishi.cn/gtsewqnbpl.html

for (i in 1..10) println(i)
来源：http://hz.hysaishi.cn/gtagqtfndx.html

[T15] Kotlin：接口
来源：http://hz.yonumen.top/gtuwckhnld.html

interface Shape { fun area(): Double }
来源：http://hz.hammf.cn/gtmwldmoal.html

[T16] Swift：Hello World
来源：http://hz.cucudq.cn/gtmduyklnv.html

print("Hello")
来源：http://hz.tianlin.xyz/gtronminmw.html

[T17] Swift：变量与常量
来源：http://hz.yanxiufei.cn/gtohbsivdv.html

var a = 1;  let b = 2
来源：http://hz.ydjk.org.cn/gtgsrdnfov.html

[T18] Swift：字符串插值
来源：http://hz.havefunace.top/gtwhuuxgno.html

"值: \(b)"
来源：http://hz.xuanzx.com/gtjgxymggw.html

[T19] Swift：可选绑定
来源：http://hz.sxryk.cn/gtuxxwybre.html

if let n = opt { print(n) }
来源：http://hz.tian-w.cn/gtkkhoptzf.html

[T20] Swift：数组操作
来源：http://hz.xinyue.icu/gtuwtdkwmp.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zhongyouzk.top/gttcvroutr.html

[T21] Swift：遍历
来源：http://hz.nanxuanxn.top/gtjabqvdjg.html

for x in a { print(x) }
来源：http://hz.aizwys.cn/gtmoayfphl.html

[T22] Swift：字典
来源：http://hz.tian-w.cn/gtzeqcvogp.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yuanzhike.top/gttevhjupr.html

[T23] Swift：函数
来源：http://hz.xziqi.cn/gtzkxlwkoq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jinghuilouyu.cn/gtpohaymal.html

[T24] Swift：闭包
来源：http://hz.chenlongwang.top/gtmujjnlvc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.hongshengwenyu.top/gtdgxbtlme.html

[T25] Swift：结构体
来源：http://hz.aizwys.cn/gttbzirqor.html

struct P { var x: Int }
来源：http://hz.tianlin.xyz/gtpiedjpxf.html

[T26] Swift：类与重写
来源：http://hz.aibaodan.cn/gttbitazyb.html

class A: Base { override func f() {} }
来源：http://hz.hnqzz.top/gtgyoxizjx.html

[T27] Swift：错误处理
来源：http://hz.dianchejie.cn/gtnlvlstxg.html

do { try f() } catch { print(error) }
来源：http://hz.ywan-chungtsiang.top/gtfyllifmr.html

[T28] Swift：枚举
来源：http://hz.hnqzz.top/gtjmaoxcfd.html

enum Color { case red, green }
来源：http://hz.gogol.net.cn/gtfmsrlhbm.html

[T29] Swift：guard 提前返回
来源：http://hz.vqdsnc.cn/gtnncqqwjr.html

guard let x = opt else { return }
来源：http://hz.jqgufenzy.top/gthjtfjljp.html

[T30] Swift：协议
来源：http://hz.svipenyu.cn/gtzsfuchzq.html

protocol Shape { func area() -> Double }
来源：http://hz.zhiwuduotai.top/gticlxzwvi.html

[T31] Lua：Hello World
来源：http://hz.fengsongda.top/gtwxausdjs.html

print("Hello")
来源：http://hz.wangdashe.top/gtnfyoypeg.html

[T32] Lua：局部变量
来源：http://hz.gotoacloud.top/gtgohufktt.html

local a = 1
来源：http://hz.zhaomingkeji.xyz/gtfcfazmul.html

[T33] Lua：表（数组）
来源：http://hz.dashuyun.cn/gtqiupunea.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yuanzhike.top/gtnrrhkjws.html

[T34] Lua：遍历表
来源：http://hz.0kj1m.cn/gtqczjwgoe.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jinqigufen.top/gtmxkqdlqf.html

[T35] Lua：字典表
来源：http://hz.jiagoushi.top/gtmmwouhhq.html

local d = { a = 1 };  d.b = 2
来源：http://hz.andypj.xyz/gtdfuyczgf.html

[T36] Lua：函数
来源：http://hz.andypj.xyz/gtqhnzivdb.html

function add(a, b) return a + b end
来源：http://hz.jlsjyb.cn/gtzfnejyks.html

[T37] Lua：字符串拼接
来源：http://hz.mhx1999.top/gthadgblal.html

"a" .. "b"
来源：http://hz.jinyuanbaomall.cn/gttwqczvrr.html

[T38] Lua：条件
来源：http://hz.nanxuanxn.top/gtcwsiejii.html

if x > 0 then print("正") end
来源：http://hz.vqdsnc.cn/gtzdvddrsx.html

[T39] Lua：模式匹配
来源：http://hz.hnxiangtu.top/gtxqozgslz.html

string.find(s, "%d+")
来源：http://hz.zhoulong.xyz/gtlyxfrefq.html

[T40] Lua：元表
来源：http://hz.chenjidiqi.icu/gtkjijmhtm.html

setmetatable({}, { __index = base })
来源：http://hz.tanke756.top/gtrskqfndm.html

[T41] Perl：Hello World
来源：http://hz.guannengcc.top/gtqwbgjphc.html

print "Hello\n";
来源：http://hz.sysykeji.top/gtlmprjevq.html

[T42] Perl：变量类型
来源：http://hz.nanxinkj.top/gtnphqybta.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.cqqwz.cn/gtppdqxxgr.html

[T43] Perl：字符串插值
来源：http://hz.dianchejie.cn/gtbippdzbf.html

"值: $a"
来源：http://hz.xinyue.icu/gtirhrunnv.html

[T44] Perl：条件
来源：http://hz.zhixingplan.top/gtdpvevqpq.html

if ($a > 0) { print "正"; }
来源：http://hz.zdqjudy.top/gtrepystei.html

[T45] Perl：数组遍历
来源：http://hz.sysykeji.top/gtripugwrk.html

for my $x (@arr) { print $x; }
来源：http://hz.wangshuangyany.cn/gtpynbbndz.html

[T46] Perl：哈希操作
来源：http://hz.guannengcc.top/gtfzytitso.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.havefunace.top/gtgxlpusjl.html

[T47] Perl：正则捕获
来源：http://hz.aibaodan.cn/gtaedmfaco.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.wangshuangyany.cn/gtmieehnhw.html

[T48] Perl：正则替换
来源：http://hz.ppjwa.cn/gtjcolzctx.html

$s =~ s/old/new/g;
来源：http://hz.pycfn.com/gtnmerhxdl.html

[T49] Perl：函数
来源：http://hz.birdmap.top/gtaekcdswn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.gogol.net.cn/gtvxivnhkz.html

[T50] Perl：逐行读文件
来源：http://hz.xylfe.cn/gtzpxlfeor.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.cashguo.top/gtfcxaudsm.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.fzhhl.top/gtxdjwihff.html

[T51] Scala：Hello World
来源：http://hz.nanxuanxn.top/gtvcekvjsb.html

println("Hello")
来源：http://hz.nanxinkj.top/gtviivpqgy.html

[T52] Scala：变量
来源：http://hz.guannengcc.top/gtllsrfaix.html

val a = 1;  var b = 2
来源：http://hz.gaohongyu789.top/gtpfsjwgfq.html

[T53] Scala：字符串插值
来源：http://hz.aizwys.cn/gtsedykqlh.html

s"值: $b"
来源：http://hz.tianlin.xyz/gtzqocaudt.html

[T54] Scala：集合映射
来源：http://hz.wangdashe.top/gtzowvtmgh.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.hfpthk.cn/gtrzgxhvcd.html

[T55] Scala：集合过滤
来源：http://hz.bjfxy.top/gtlushxfzw.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jinyuanbaomall.cn/gtnogkbqvw.html

[T56] Scala：样例类
来源：http://hz.jqgfzy.top/gtcbvmnlkh.html

case class User(name: String, age: Int)
来源：http://hz.guowangkeji.top/gtszhhbcdv.html

[T57] Scala：模式匹配
来源：http://hz.yangfankeji.com/gtyixkqdog.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.sxryk.cn/gtpgvglyfc.html

[T58] Scala：函数定义
来源：http://hz.sxryk.cn/gtlaooynef.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zdqjudy.top/gtzdeglhbg.html

[T59] Scala：循环
来源：http://hz.birdmap.top/gtrajfdvpy.html

for (i <- 1 to 10) println(i)
来源：http://hz.andypj.xyz/gtkzavvvhz.html

[T60] Scala：折叠
来源：http://hz.gzhubu.top/gtkergzfqx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.aibaodan.cn/gtezskkoqi.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtxcewzrlx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhiwuduotai.top/gtruubfmql.html

================================================================================
来源：http://hz.jiagoushi.top/gtqtbxpfsb.html

[U01] Py：创建虚拟环境
来源：http://hz.wangdashe.top/gtokohzvwu.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.ppjwa.cn/gteyjmmkal.html

[U02] Py：导出 / 安装依赖
来源：http://hz.hysaishi.cn/gtzslblrhc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.0kj1m.cn/gtwpjnjejf.html

[U03] Py：加载 .env 配置
来源：http://hz.snrcjt.cn/gtprvtrjas.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zycfv.cn/gtscgoxpod.html

[U04] Py：变量调试打印
来源：http://hz.gotoacloud.top/gtlmegtcta.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.cqqwz.cn/gtjyjnkjst.html

[U05] Py：列表去重且保序
来源：http://hz.yvedp.cn/gtckyohapr.html

list(dict.fromkeys(arr))
来源：http://hz.hammf.cn/gtesswlltl.html

[U06] Py：合并两个字典
来源：http://hz.xuetiantiany.cn/gtdymvteiz.html

{**a, **b}
来源：http://hz.hfpthk.cn/gtepsyobzx.html

[U07] Py：反转字典键值
来源：http://hz.xuetiantiany.cn/gtmhkckicr.html

{v: k for k, v in d.items()}
来源：http://hz.aibaodan.cn/gtmskmpyvw.html

[U08] Py：展平二维列表
来源：http://hz.hongshengwenyu.top/gtqssxklvt.html

[y for x in nested for y in x]
来源：http://hz.zhiwuduotai.top/gtvcfolgly.html

[U09] Py：字典取最大值的键
来源：http://hz.vqdsnc.cn/gtarrtswkj.html

max(d, key=d.get)
来源：http://hz.zdqjudy.top/gtlzrqdgvs.html

[U10] Py：按值排序字典
来源：http://hz.quarkkingdee.top/gtkmpozlmn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.hysaishi.cn/gtyxaibnlm.html

[U11] Py：生成器表达式
来源：http://hz.hfpthk.cn/gtptltswyq.html

(x * 2 for x in arr)
来源：http://hz.gaohongyu789.top/gtruxfrviw.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.vqdsnc.cn/gtnwzrzcsm.html

Counter(arr).most_common(3)
来源：http://hz.pycfn.com/gtvhupcldc.html

[U13] Py：固定长度队列
来源：http://hz.tianlin.xyz/gtkstucatf.html

deque(maxlen=10)
来源：http://hz.smart0.xyz/gtngfnjhfv.html

[U14] Py：分组收集到列表
来源：http://hz.jiagoushi.top/gtftymktea.html

defaultdict(list)
来源：http://hz.yj20258888.top/gtbncoeggh.html

[U15] Py：高精度计时
来源：http://hz.jyoumei.cn/gtnxxmtxvd.html

t = time.perf_counter()
来源：http://hz.zhoulong.xyz/gtkvvdmwdl.html

[U16] Py：命令行参数解析
来源：http://hz.vqdsnc.cn/gtqjyjznyn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.hysaishi.cn/gtcqaqwdii.html

[U17] Py：初始化日志
来源：http://hz.zdqjudy.top/gtrrnirpwh.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.zycfv.cn/gtzredzruj.html

[U18] Py：预编译正则
来源：http://hz.9152youxi.cn/gtaalribdo.html

pat = re.compile(r"\d+")
来源：http://hz.fengsongda.top/gtwzsbehll.html

[U19] Py：正则替换带回调
来源：http://hz.hammf.cn/gtpwhpejlg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.cheryme.top/gtkklypfub.html

[U20] Py：缓存函数结果
来源：http://hz.zhaomingkeji.xyz/gtiqssaoer.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zhixingplan.top/gtxeerfsha.html

[U21] Py：自定义上下文管理器
来源：http://hz.wangdashe.top/gttdxalkbl.html

@contextlib.contextmanager
来源：http://hz.sysykeji.top/gtfdunuzcf.html

[U22] Py：矩阵转置
来源：http://hz.vqdsnc.cn/gtcfwujcye.html

list(zip(*m))
来源：http://hz.zhijiandao.cn/gtqjgpvfru.html

[U23] Py：分块读取大文件
来源：http://hz.yj20258.top/gtdewkiaod.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.9152youxi.cn/gtvdxxmhkc.html

[U24] Py：路径操作
来源：http://hz.jianghu66.top/gtrjrisuea.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.zhixingplan.top/gtmahvhuwl.html

[U25] Py：CSV 按字典读
来源：http://hz.zhengqikj.top/gtskibvphk.html

csv.DictReader(f)
来源：http://hz.xuanzx.com/gtsjljqvqc.html

[U26] Py：并发下载
来源：http://hz.hongshengwenyu.top/gtwpsjuwka.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.zhoulong.xyz/gtlmskgtqj.html

[U27] Py：异步 HTTP
来源：http://hz.jianghu66.top/gtxpehqjbt.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.zycfv.cn/gthuqukmph.html

[U28] Py：类型别名
来源：http://hz.iojbl.cn/gtwikgjqhl.html

UserId = int
来源：http://hz.sxryk.cn/gtzlnyoiev.html

[U29] Py：属性校验
来源：http://hz.sysykeji.top/gtjmbfbbim.html

@property 与 @x.setter 配合
来源：http://hz.fzhhl.top/gtnoqoxbii.html

[U30] Py：数据类
来源：http://hz.guowangkeji.top/gtudzbantu.html

@dataclass(slots=True)
来源：http://hz.jinqigfzy.top/gtrfbvuzxu.html

[U31] Py：单测
来源：http://hz.chenjidiqi.icu/gtezdnlzgx.html

python -m pytest -q
来源：http://hz.shangyingyoupin.top/gtmjkxeqjz.html

[U32] Py：代码格式化
来源：http://hz.yueranfly.top/gtknhfvema.html

ruff format . && ruff check --fix .
来源：http://hz.ppjwa.cn/gtjyexccxj.html

[U33] Py：打包发布
来源：http://hz.316326.xyz/gteqttoxfr.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.wangdashe.top/gtjkntbnqj.html

[U34] Py：判断编码
来源：http://hz.shzxlz.cn/gtamihtird.html

chardet.detect(raw)
来源：http://hz.hammf.cn/gtxfpfzwed.html

[U35] Py：发送邮件
来源：http://hz.zhixingplan.top/gtsrmuuohi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.sxryk.cn/gtejepqjxt.html

[U36] Py：定时任务
来源：http://hz.cucudq.cn/gtoxhxaqnk.html

schedule.every(10).minutes.do(job)
来源：http://hz.tanke756.top/gtckathgnc.html


<!-- 参考信息 -->