代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.chenlongwang.top/gtiyafaonf.html

[S13] C：宏定义
来源：http://hz.gotoacloud.top/gtqrroxfyu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.tianlin.xyz/gtvgenjzfw.html

[S14] C：枚举
来源：http://hz.feifeiyinyue.top/gtsgcjnxzz.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.sxryk.cn/gtluhnpwyo.html

[S15] C：类型转换
来源：http://hz.haohaochexian.top/gtfxnltjsj.html

(double) a / b
来源：http://hz.wangdashe.top/gtzdcgknml.html

[S16] C：位操作置位
来源：http://hz.dashuyun.cn/gtgklwuqqc.html

x |= (1 << 3);
来源：http://hz.shuidangran.top/gtqaoubmvf.html

[S17] C：安全拼接字符串
来源：http://hz.yvedp.cn/gtjyxjvjgq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.shanyushiyangkeji.top/gtqlsucgvt.html

[S18] C：命令行参数
来源：http://hz.gaohongyu789.top/gtkroaoymi.html

int main(int argc, char **argv)
来源：http://hz.hammf.cn/gtylsvocez.html

[S19] C：快速排序
来源：http://hz.hysaishi.cn/gtjcrxnptr.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zdqjudy.top/gtqbdvitsy.html

[S20] C：二分查找
来源：http://hz.sweek.top/gteddhlizi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jyoumei.cn/gtakxsgpgt.html

[S21] C：字符类别判断
来源：http://hz.birdmap.top/gtbhcvbwro.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xinyue.icu/gtlvhuzdlq.html

[S22] C：字符串转数字
来源：http://hz.tanke756.top/gtyzdujfvf.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.0kj1m.cn/gttyfdfrke.html

[S23] C：随机数
来源：http://hz.fzhhl.top/gtzssudmkw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.fengsongda.top/gtwguieuvi.html

[S24] C：获取本地时间
来源：http://hz.zdqjudy.top/gtsrxjsfle.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.kuanghao11.cn/gtisjumehb.html

[S25] C：内存拷贝
来源：http://hz.jqgfzy.top/gtvxpqifvm.html

memcpy(dst, src, n);
来源：http://hz.jinqigfzy.top/gtnsgsqrnl.html

[S26] C：内存清零
来源：http://hz.yvedp.cn/gtatqxrabj.html

memset(a, 0, sizeof a);
来源：http://hz.jqgufenzy.top/gtcnnwkppz.html

[S27] C：定义常量
来源：http://hz.yj20258888.top/gtlajhggdl.html

const double PI = 3.14159;
来源：http://hz.smart0.xyz/gtregboaeq.html

[S28] C：静态变量
来源：http://hz.cqqwz.cn/gtcjfykmyt.html

static int counter = 0;
来源：http://hz.hammf.cn/gtmbtlcxms.html

[S29] C：变参函数
来源：http://hz.ivvv.top/gtcbpntguj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhaomingkeji.xyz/gtmszmiiym.html

[S30] C：头文件保护
来源：http://hz.aibaodan.cn/gtdizrclci.html

#ifndef X_H
来源：http://hz.yj20258888.top/gthcbyiryg.html

#define X_H
来源：http://hz.gogol.net.cn/gtahxnlkbe.html

#endif
来源：http://hz.jqgufenzy.top/gtjiwwteap.html

[S31] C++：Hello World
来源：http://hz.dianchejie.cn/gtdpoblkor.html

#include <iostream>
来源：http://hz.feifeiyinyue.top/gtavzqwudg.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.tianlin.xyz/gtpzukfodi.html

[S32] C++：字符串
来源：http://hz.yangfankeji.com/gtpaohquss.html

std::string s = "hi";  s += "!";
来源：http://hz.hnqzz.top/gtxbavvewy.html

[S33] C++：vector 增删
来源：http://hz.shangyingyoupin.top/gtvnempykf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zhixingplan.top/gtxfpykyxp.html

[S34] C++：遍历 vector
来源：http://hz.zhengqikj.top/gtcxbthohu.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhengqikj.top/gtvzjaadeg.html

[S35] C++：map
来源：http://hz.sufxvd.cn/gtyirdmxqb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jlsjyb.cn/gthrblcbyi.html

[S36] C++：unordered_map
来源：http://hz.zhaomingkeji.xyz/gtnodytfsp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinqigufen.top/gtpanhrous.html

[S37] C++：set
来源：http://hz.bjfxy.top/gtjpeojujh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.smart0.xyz/gtjmzeszdy.html

[S38] C++：排序
来源：http://hz.hnqzz.top/gtijkbdmxt.html

std::sort(v.begin(), v.end());
来源：http://hz.guannengcc.top/gttrtjouit.html

[S39] C++：自定义比较器排序
来源：http://hz.vqdsnc.cn/gtgivahapv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhengqikj.top/gtrsndquwl.html

[S40] C++：查找元素
来源：http://hz.dashuyun.cn/gthsokaxyf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.cucudq.cn/gtrabmznte.html

[S41] C++：类与构造函数
来源：http://hz.jyoumei.cn/gtqwcydupf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hongshengwenyu.top/gtirabpost.html

[S42] C++：继承与虚函数
来源：http://hz.nanxinkj.top/gtmrgdpmpq.html

class B : public Base { public: void f() override {} };
来源：http://hz.nwbrower.top/gtpswevghd.html

[S43] C++：智能指针
来源：http://hz.zhoulong.xyz/gtgosjffdj.html

auto p = std::make_unique<int>(5);
来源：http://hz.cdnleiting.top/gtccwdzvmq.html

[S44] C++：引用传参
来源：http://hz.feifeiyinyue.top/gtdhgaaxgg.html

void inc(int &x) { ++x; }
来源：http://hz.yuxming.cn/gtweijbcvw.html

[S45] C++：lambda
来源：http://hz.zhiwuduotai.top/gtewjsxcio.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.sysykeji.top/gtmdjyyhqa.html

[S46] C++：函数模板
来源：http://hz.jinqigfzy.top/gtariqaefv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.tianlin.xyz/gtsbmpkzzb.html

[S47] C++：结构化绑定遍历
来源：http://hz.mhx1999.top/gtzhukeikq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.wangshuangyany.cn/gtjensjemi.html

[S48] C++：逐行读文件
来源：http://hz.zhongyouzk.top/gtyzttgcik.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.gzhubu.top/gtlbuhenlp.html

while (std::getline(in, line)) { }
来源：http://hz.nanxinkj.top/gtdpisggmm.html

[S49] C++：写文件
来源：http://hz.wangshuangyany.cn/gtnxtewysw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.quarkkingdee.top/gtbkplcipe.html

[S50] C++：格式化数字
来源：http://hz.wangdashe.top/gtfkxyrrln.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.tanke756.top/gtfecusugs.html

[S51] C++：显式类型转换
来源：http://hz.hfpthk.cn/gtpeaqczqq.html

static_cast<double>(a) / b
来源：http://hz.yuxming.cn/gtvqhhnckk.html

[S52] C++：const 与 noexcept
来源：http://hz.andypj.xyz/gtytplhtps.html

int size() const noexcept { return n_; }
来源：http://hz.pengpengdd.cyou/gtndwnbvhl.html

[S53] C++：移动语义
来源：http://hz.shzxlz.cn/gtsiqpfgle.html

std::vector<int> w = std::move(v);
来源：http://hz.daria6918.cn/gtrciiwuma.html

[S54] C++：异常处理
来源：http://hz.wangdashe.top/gtcdhedgvn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.svipenyu.cn/gtzpbuewdy.html

[S55] C++：结构化绑定
来源：http://hz.sweek.top/gtnyiuecbv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jianghu66.top/gtxerqhspk.html

[S56] C++：optional
来源：http://hz.jinyuanbaomall.cn/gthusggapv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.shuidangran.top/gtjzgldodi.html

[S57] C++：编译期常量
来源：http://hz.zhongyouzk.top/gtbialfdak.html

constexpr int N = 10;
来源：http://hz.daxiang520.top/gtpcntuwkr.html

[S58] C++：命名空间
来源：http://hz.kuanghao11.cn/gtfblfmpso.html

namespace ns { int f() { return 1; } }
来源：http://hz.jqgfzy.top/gthlakksfn.html

[S59] C++：静态断言
来源：http://hz.wangshuangyany.cn/gtxdyzljhh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.svipenyu.cn/gtcbshloap.html

[S60] C++：遍历并删除元素
来源：http://hz.cheryme.top/gtpibjydwz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.tanke756.top/gtcqqndyau.html

================================================================================
来源：http://hz.sufxvd.cn/gtlplskqhe.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yvedp.cn/gtywweudii.html

================================================================================
来源：http://hz.zhixingplan.top/gtmzlyndoc.html

[T01] Kotlin：Hello World
来源：http://hz.daxiang520.top/gtdciubzeb.html

println("Hello")
来源：http://hz.wangshuangyany.cn/gtwkdknidr.html

[T02] Kotlin：变量
来源：http://hz.vqdsnc.cn/gtjwwabwgr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.cucudq.cn/gtubnobddt.html

[T03] Kotlin：字符串模板
来源：http://hz.hnqzz.top/gtqfpfhfoa.html

"值: $b"
来源：http://hz.hongshengwenyu.top/gtjwjqliru.html

[T04] Kotlin：空安全
来源：http://hz.iojbl.cn/gtrfzemyoq.html

val n: String? = null;  n?.length
来源：http://hz.andypj.xyz/gtjyhifsol.html

[T05] Kotlin：when 表达式
来源：http://hz.nanxinkj.top/gtkyitbexe.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.tanke756.top/gtbcxlwhvb.html

[T06] Kotlin：集合映射
来源：http://hz.0kj1m.cn/gttaaqyyxk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.cheryme.top/gtacjlodqt.html

[T07] Kotlin：集合过滤
来源：http://hz.c1oappe.top/gtwofjhxci.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhijiandao.cn/gtyamjjavb.html

[T08] Kotlin：数据类
来源：http://hz.chenlongwang.top/gtygxwtfww.html

data class User(val name: String, val age: Int)
来源：http://hz.pycfn.com/gtsbjyxcra.html

[T09] Kotlin：扩展函数
来源：http://hz.ydzc1.top/gtsjujpnob.html

fun String.exclaim() = this + "!"
来源：http://hz.tianlin.xyz/gtjaugitfm.html

[T10] Kotlin：默认参数
来源：http://hz.ybcxt.top/gtcjxgormb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.cashguo.top/gtlegneedu.html

[T11] Kotlin：协程
来源：http://hz.zhixingplan.top/gtgcfmpfnn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.aibaodan.cn/gtwpvuxycb.html

[T12] Kotlin：解构声明
来源：http://hz.cheryme.top/gtikkgrwgy.html

val (a, b) = Pair(1, 2)
来源：http://hz.zhixingplan.top/gtacfxpexf.html

[T13] Kotlin：只读 Map
来源：http://hz.svipenyu.cn/gtgpdwzvvf.html

val m = mapOf("a" to 1)
来源：http://hz.sweek.top/gtjlvcootg.html

[T14] Kotlin：循环
来源：http://hz.jinqigfzy.top/gtbzorfrgk.html

for (i in 1..10) println(i)
来源：http://hz.daria6918.cn/gtfsfryqqg.html

[T15] Kotlin：接口
来源：http://hz.hnxiangtu.top/gtyizyzxqq.html

interface Shape { fun area(): Double }
来源：http://hz.aizwys.cn/gtaiufocmz.html

[T16] Swift：Hello World
来源：http://hz.shanyushiyangtech.top/gtocirkrxy.html

print("Hello")
来源：http://hz.redwolf501.top/gtkdskdrij.html

[T17] Swift：变量与常量
来源：http://hz.cucudq.cn/gtpbnsiseu.html

var a = 1;  let b = 2
来源：http://hz.jlsjyb.cn/gtzmfvzkji.html

[T18] Swift：字符串插值
来源：http://hz.jqgufenzy.top/gtckhuwqbp.html

"值: \(b)"
来源：http://hz.yuanzhike.top/gtlwtvcial.html

[T19] Swift：可选绑定
来源：http://hz.vqdsnc.cn/gtbgnitbgv.html

if let n = opt { print(n) }
来源：http://hz.yj202588.top/gthyhvpuin.html

[T20] Swift：数组操作
来源：http://hz.jinyuanbaomall.cn/gtaujcyspc.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.c1oappe.top/gttcveosyz.html

[T21] Swift：遍历
来源：http://hz.yvedp.cn/gtumamwymo.html

for x in a { print(x) }
来源：http://hz.yj202588.top/gtnhqmpqah.html

[T22] Swift：字典
来源：http://hz.hongshengwenyu.top/gtnrmsvlci.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.vqdsnc.cn/gtqodpnbmf.html

[T23] Swift：函数
来源：http://hz.zhongyouzk.top/gtjnxvrdpg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yuxming.cn/gtksyyrukd.html

[T24] Swift：闭包
来源：http://hz.yvedp.cn/gtarclzetj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.ydjk.org.cn/gthfliypff.html

[T25] Swift：结构体
来源：http://hz.shuidangran.top/gtnofdgcrh.html

struct P { var x: Int }
来源：http://hz.yangfankeji.com/gtczeawgnc.html

[T26] Swift：类与重写
来源：http://hz.ydzc1.top/gtdezfmxod.html

class A: Base { override func f() {} }
来源：http://hz.cucudq.cn/gtdvhlzvok.html

[T27] Swift：错误处理
来源：http://hz.smart0.xyz/gtegoefdva.html

do { try f() } catch { print(error) }
来源：http://hz.jinyuanbaomall.cn/gtntvzumik.html

[T28] Swift：枚举
来源：http://hz.jqgfzy.top/gtweqaxlii.html

enum Color { case red, green }
来源：http://hz.ydjk.org.cn/gtatfhgrsf.html

[T29] Swift：guard 提前返回
来源：http://hz.yuxming.cn/gtkdxchhmh.html

guard let x = opt else { return }
来源：http://hz.zhiwuduotai.top/gtjgvuidhc.html

[T30] Swift：协议
来源：http://hz.nwbrower.top/gtxoatyzjz.html

protocol Shape { func area() -> Double }
来源：http://hz.ywan-chungtsiang.top/gtwnivgjxd.html

[T31] Lua：Hello World
来源：http://hz.aizwys.cn/gtsfmrdexn.html

print("Hello")
来源：http://hz.zhiwuduotai.top/gtovycliii.html

[T32] Lua：局部变量
来源：http://hz.vqdsnc.cn/gtnjjrpfam.html

local a = 1
来源：http://hz.birdmap.top/gtgsdujrxj.html

[T33] Lua：表（数组）
来源：http://hz.cucudq.cn/gtdyuxoydp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.gaohongyu789.top/gtbzqtqwgw.html

[T34] Lua：遍历表
来源：http://hz.zhixingplan.top/gtcdepinta.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yj202588.top/gtwoarltkl.html

[T35] Lua：字典表
来源：http://hz.jinqigfzy.top/gtjgnbgtmw.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yangfankeji.com/gtvdnnrobe.html

[T36] Lua：函数
来源：http://hz.jinghuilouyu.cn/gtgkkhgigm.html

function add(a, b) return a + b end
来源：http://hz.cashguo.top/gtcazcfiwf.html

[T37] Lua：字符串拼接
来源：http://hz.xylfe.cn/gtoycgqkmv.html

"a" .. "b"
来源：http://hz.sysykeji.top/gtntxohdpt.html

[T38] Lua：条件
来源：http://hz.ywan-chungtsiang.top/gtfyfkpcgi.html

if x > 0 then print("正") end
来源：http://hz.pycfn.com/gtbwvgxxzu.html

[T39] Lua：模式匹配
来源：http://hz.redwolf501.top/gtxviquddn.html

string.find(s, "%d+")
来源：http://hz.zhongyouzk.top/gtqmfopyki.html

[T40] Lua：元表
来源：http://hz.0kj1m.cn/gtrexdoknl.html

setmetatable({}, { __index = base })
来源：http://hz.hongshengwenyu.top/gthlqkyslf.html

[T41] Perl：Hello World
来源：http://hz.wangdashe.top/gtdqviyhlc.html

print "Hello\n";
来源：http://hz.zhaomingkeji.xyz/gtyeorwjzn.html

[T42] Perl：变量类型
来源：http://hz.chenzaomai.com/gtzizsvlmg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zhiwuduotai.top/gtodaalcrx.html

[T43] Perl：字符串插值
来源：http://hz.fengsongda.top/gtnrkgnqth.html

"值: $a"
来源：http://hz.jinghuilouyu.cn/gtyhiqbodf.html

[T44] Perl：条件
来源：http://hz.andypj.xyz/gtkacmbqnc.html

if ($a > 0) { print "正"; }
来源：http://hz.nanxuanxn.top/gtxqlfxyil.html

[T45] Perl：数组遍历
来源：http://hz.cheryme.top/gtpqkgsaza.html

for my $x (@arr) { print $x; }
来源：http://hz.52xcode.cn/gtxhdnuwlb.html

[T46] Perl：哈希操作
来源：http://hz.ywan-chungtsiang.top/gtaifdpluu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.fzhhl.top/gtfrrazpkt.html

[T47] Perl：正则捕获
来源：http://hz.chenlongwang.top/gtmishllnd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.cashguo.top/gtkwzsvbly.html

[T48] Perl：正则替换
来源：http://hz.yonumen.top/gthzgbonlv.html

$s =~ s/old/new/g;
来源：http://hz.zhaomingkeji.xyz/gtzuptjsoy.html

[T49] Perl：函数
来源：http://hz.gotoacloud.top/gtmivdrdzv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.ppjwa.cn/gtqelaqfnp.html

[T50] Perl：逐行读文件
来源：http://hz.sysykeji.top/gtlrcvdrku.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.ppjwa.cn/gttqdqswyu.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.zhiwuduotai.top/gtetdzyxdv.html

[T51] Scala：Hello World
来源：http://hz.gaohongyu789.top/gtelvxnhoy.html

println("Hello")
来源：http://hz.ydjk.org.cn/gtiwusloqw.html

[T52] Scala：变量
来源：http://hz.cheryme.top/gtbkozzawj.html

val a = 1;  var b = 2
来源：http://hz.chenjidiqi.icu/gtsireylzs.html

[T53] Scala：字符串插值
来源：http://hz.xinyue.icu/gtwslzeakz.html

s"值: $b"
来源：http://hz.0kj1m.cn/gttlrizcev.html

[T54] Scala：集合映射
来源：http://hz.quarkkingdee.top/gtfxpvlgvw.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.zhongyouzk.top/gthrzjvaij.html

[T55] Scala：集合过滤
来源：http://hz.meibo888.top/gtlkpqfuos.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.yonumen.top/gtvsfwsviv.html

[T56] Scala：样例类
来源：http://hz.yangfankeji.com/gtjhzlifxw.html

case class User(name: String, age: Int)
来源：http://hz.guannengcc.top/gtddivozdp.html

[T57] Scala：模式匹配
来源：http://hz.yj202588.top/gtciamijtf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.jlsjyb.cn/gttbgundyu.html

[T58] Scala：函数定义
来源：http://hz.zhiwuduotai.top/gtypcoggef.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.dashuyun.cn/gtwahqvvgh.html

[T59] Scala：循环
来源：http://hz.pycfn.com/gtqprknwqx.html

for (i <- 1 to 10) println(i)
来源：http://hz.shzxlz.cn/gtbepebesh.html

[T60] Scala：折叠
来源：http://hz.hywenlv.cn/gtolfxlyhg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yanxiufei.cn/gtxgxwdhnf.html

================================================================================
来源：http://hz.hnxiangtu.top/gtmkqotyow.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.bjfxy.top/gtnvobxazr.html

================================================================================
来源：http://hz.zycfv.cn/gtmlxvqnxu.html

[U01] Py：创建虚拟环境
来源：http://hz.hywenlv.cn/gtqskeoccl.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.wangshuangyany.cn/gtxsmifydn.html

[U02] Py：导出 / 安装依赖
来源：http://hz.zhongyouzk.top/gtixaiumih.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.tian-w.cn/gtocofwifa.html

[U03] Py：加载 .env 配置
来源：http://hz.zhixingplan.top/gtocpbgjfr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.gzhubu.top/gttosqtvbq.html

[U04] Py：变量调试打印
来源：http://hz.hfpthk.cn/gttuempffk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.havefunace.top/gtenmeimmg.html

[U05] Py：列表去重且保序
来源：http://hz.snrcjt.cn/gtwxksruxb.html

list(dict.fromkeys(arr))
来源：http://hz.316326.xyz/gtjwxhmxlo.html

[U06] Py：合并两个字典
来源：http://hz.cashguo.top/gtpaqvcync.html

{**a, **b}
来源：http://hz.tanke756.top/gtqwlegrti.html

[U07] Py：反转字典键值
来源：http://hz.zhongyouzk.top/gtstidievd.html

{v: k for k, v in d.items()}
来源：http://hz.0kj1m.cn/gtlqhbruau.html

[U08] Py：展平二维列表
来源：http://hz.xuetiantiany.cn/gttrscmhvl.html

[y for x in nested for y in x]
来源：http://hz.vqdsnc.cn/gtkmffrbry.html

[U09] Py：字典取最大值的键
来源：http://hz.xingfuxueyuan.xyz/gtrarygwvm.html

max(d, key=d.get)
来源：http://hz.yuanzhike.top/gtzyuslfbu.html

[U10] Py：按值排序字典
来源：http://hz.kuanghao11.cn/gtkqedoagw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.dashuyun.cn/gtteaqguzt.html

[U11] Py：生成器表达式
来源：http://hz.xuetiantiany.cn/gtfkeiofao.html

(x * 2 for x in arr)
来源：http://hz.tianlin.xyz/gteepydtff.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.fengsongda.top/gtjuryvmyk.html

Counter(arr).most_common(3)
来源：http://hz.havefunace.top/gtncrvpqox.html

[U13] Py：固定长度队列
来源：http://hz.wangshuangyany.cn/gtmyqahqaq.html

deque(maxlen=10)
来源：http://hz.ybcxt.top/gtjcyyscmz.html

[U14] Py：分组收集到列表
来源：http://hz.zhengqikj.top/gtaidcbbjt.html

defaultdict(list)
来源：http://hz.zhaomingkeji.xyz/gtmwvamaig.html

[U15] Py：高精度计时
来源：http://hz.yj20258888.top/gthdvcgvcx.html

t = time.perf_counter()
来源：http://hz.yuxming.cn/gttkaidrov.html

[U16] Py：命令行参数解析
来源：http://hz.hammf.cn/gtnmogtdhx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.zhijiandao.cn/gteewyvwtt.html

[U17] Py：初始化日志
来源：http://hz.hammf.cn/gtftzvfcbx.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.shzxlz.cn/gtmtgqoeco.html

[U18] Py：预编译正则
来源：http://hz.zhaomingkeji.xyz/gtkrtlbbbe.html

pat = re.compile(r"\d+")
来源：http://hz.gogol.net.cn/gtlwvexgrd.html

[U19] Py：正则替换带回调
来源：http://hz.zhiwuduotai.top/gtldguzptk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.gotoacloud.top/gtytdragjx.html

[U20] Py：缓存函数结果
来源：http://hz.dianchejie.cn/gtqjbevgpz.html

@functools.lru_cache(maxsize=None)
来源：http://hz.shangyingyoupin.top/gtbcvxsoya.html

[U21] Py：自定义上下文管理器
来源：http://hz.jqgfzy.top/gtjqimlftb.html

@contextlib.contextmanager
来源：http://hz.zycfv.cn/gtlaoqjvde.html

[U22] Py：矩阵转置
来源：http://hz.jinghuilouyu.cn/gtyehmhocm.html

list(zip(*m))
来源：http://hz.zhixingplan.top/gtrovlbjip.html

[U23] Py：分块读取大文件
来源：http://hz.shuidangran.top/gtabkxflhp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.mhx1999.top/gtwdnwofbd.html

[U24] Py：路径操作
来源：http://hz.ehwqpu.com/gtnzxsqizw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.tanke756.top/gtgdhbnyum.html

[U25] Py：CSV 按字典读
来源：http://hz.hywenlv.cn/gtrttounoh.html

csv.DictReader(f)
来源：http://hz.cqqwz.cn/gtnxwxntib.html

[U26] Py：并发下载
来源：http://hz.zhixingplan.top/gtfsgiuqfj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.mhx1999.top/gtopurwfcp.html

[U27] Py：异步 HTTP
来源：http://hz.chenzaomai.com/gtlmedvzpj.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.jqgfzy.top/gtjjngkmhb.html

[U28] Py：类型别名
来源：http://hz.andypj.xyz/gtbbffdqfc.html

UserId = int
来源：http://hz.daxiang520.top/gtrkysixsy.html

[U29] Py：属性校验
来源：http://hz.fzhhl.top/gtpigsqicv.html

@property 与 @x.setter 配合
来源：http://hz.pengpengdd.cyou/gtwkakytbm.html

[U30] Py：数据类
来源：http://hz.sysykeji.top/gtcwyqrnxt.html

@dataclass(slots=True)
来源：http://hz.jqgufenzy.top/gtubfceigp.html

[U31] Py：单测
来源：http://hz.dashuyun.cn/gtvwunpwfl.html

python -m pytest -q
来源：http://hz.zhoulong.xyz/gtjcrugnjb.html

[U32] Py：代码格式化
来源：http://hz.sufxvd.cn/gtcmfzlprx.html

ruff format . && ruff check --fix .
来源：http://hz.daria6918.cn/gtulcgroil.html

[U33] Py：打包发布
来源：http://hz.iojbl.cn/gtjneackoe.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.ydjk.org.cn/gtpszxclmk.html

[U34] Py：判断编码
来源：http://hz.zhoulong.xyz/gtjpdgxobt.html

chardet.detect(raw)
来源：http://hz.xinyue.icu/gtcnmvcopr.html

[U35] Py：发送邮件
来源：http://hz.ydjk.org.cn/gtgsrrogjo.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.sweek.top/gtvhixweea.html

[U36] Py：定时任务
来源：http://hz.dashuyun.cn/gtjxhroweo.html

schedule.every(10).minutes.do(job)
来源：http://hz.tanke756.top/gtndzlhqng.html


<!-- 参考信息 -->