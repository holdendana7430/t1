代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://hz.hysaishi.cn/gtwbotzgwc.html

[S15] C：类型转换
来源：http://hz.zhiwuduotai.top/gtkpsmcino.html

(double) a / b
来源：http://hz.jinqigufen.top/gtamgwubfl.html

[S16] C：位操作置位
来源：http://hz.feifeiyinyue.top/gtvfoicbgp.html

x |= (1 << 3);
来源：http://hz.guowangkeji.top/gtgsbhzqwr.html

[S17] C：安全拼接字符串
来源：http://hz.gogol.net.cn/gtzywcktkr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.cheryme.top/gtzhadqotp.html

[S18] C：命令行参数
来源：http://hz.gogol.net.cn/gtjpkxypii.html

int main(int argc, char **argv)
来源：http://hz.wangshuangyany.cn/gtznkfktmu.html

[S19] C：快速排序
来源：http://hz.ywan-chungtsiang.top/gtpqzjcssp.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.guowangkeji.top/gtyrbupfus.html

[S20] C：二分查找
来源：http://hz.xuanzx.com/gtteziqaiq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hnxiangtu.top/gtplljxakn.html

[S21] C：字符类别判断
来源：http://hz.yueranfly.top/gtcqzkqdap.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.316326.xyz/gtbxwzdjze.html

[S22] C：字符串转数字
来源：http://hz.jinqigfzy.top/gtlqxxsuja.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhiwuduotai.top/gtthsrgaqc.html

[S23] C：随机数
来源：http://hz.cqqwz.cn/gtruxqqkbm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.dianchejie.cn/gttvhbvzzh.html

[S24] C：获取本地时间
来源：http://hz.ybcxt.top/gtggrravpo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ppjwa.cn/gtegbhjblb.html

[S25] C：内存拷贝
来源：http://hz.mhx1999.top/gthypxqpwv.html

memcpy(dst, src, n);
来源：http://hz.smart0.xyz/gtrlxjsdrf.html

[S26] C：内存清零
来源：http://hz.aizwys.cn/gtlvdipzry.html

memset(a, 0, sizeof a);
来源：http://hz.zhiwuduotai.top/gtgjrwlabr.html

[S27] C：定义常量
来源：http://hz.shzxlz.cn/gtmctygywd.html

const double PI = 3.14159;
来源：http://hz.xuanzx.com/gtvjpvxmhw.html

[S28] C：静态变量
来源：http://hz.yanxiufei.cn/gtexdtgqfc.html

static int counter = 0;
来源：http://hz.guowangkeji.top/gthvixgvof.html

[S29] C：变参函数
来源：http://hz.sweek.top/gthihiiynv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cheryme.top/gtygsllist.html

[S30] C：头文件保护
来源：http://hz.yuanzhike.top/gtzpsxyrou.html

#ifndef X_H
来源：http://hz.guannengcc.top/gtxfosifos.html

#define X_H
来源：http://hz.xuanzx.com/gtktzdgsaz.html

#endif
来源：http://hz.yuxming.cn/gtygukqklu.html

[S31] C++：Hello World
来源：http://hz.sufxvd.cn/gtirtzdmhj.html

#include <iostream>
来源：http://hz.havefunace.top/gtwbkfdzxq.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.gotoacloud.top/gtsyntvwam.html

[S32] C++：字符串
来源：http://hz.aibaodan.cn/gthlazovuo.html

std::string s = "hi";  s += "!";
来源：http://hz.feifeiyinyue.top/gtnlbnknfe.html

[S33] C++：vector 增删
来源：http://hz.hywenlv.cn/gtajchrwnl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.c1oappe.top/gtdfywnbqr.html

[S34] C++：遍历 vector
来源：http://hz.ybcxt.top/gtjxqaafsu.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.dianchejie.cn/gtjdbfumwj.html

[S35] C++：map
来源：http://hz.zhoulong.xyz/gtsfnexlzk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.aizwys.cn/gtpegdhbau.html

[S36] C++：unordered_map
来源：http://hz.ppjwa.cn/gtxnnlopdc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jqgufenzy.top/gtynttfvbe.html

[S37] C++：set
来源：http://hz.jinqigufen.top/gtrembswjk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.fengsongda.top/gtnzivwwft.html

[S38] C++：排序
来源：http://hz.kuanghao11.cn/gtaciiikqk.html

std::sort(v.begin(), v.end());
来源：http://hz.aibaodan.cn/gtovijoklr.html

[S39] C++：自定义比较器排序
来源：http://hz.yj20258.top/gtwgtxblao.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.chenlongwang.top/gtkjrleexu.html

[S40] C++：查找元素
来源：http://hz.daria6918.cn/gtxrwviasj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.cucudq.cn/gtbkfmbkeq.html

[S41] C++：类与构造函数
来源：http://hz.ppjwa.cn/gtsvdjdxib.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jianghu66.top/gtxzbwjvuf.html

[S42] C++：继承与虚函数
来源：http://hz.ehwqpu.com/gtmhawzmft.html

class B : public Base { public: void f() override {} };
来源：http://hz.cdnleiting.top/gtevhcivnz.html

[S43] C++：智能指针
来源：http://hz.dashuyun.cn/gtqyjlacpb.html

auto p = std::make_unique<int>(5);
来源：http://hz.316326.xyz/gtnpouudhk.html

[S44] C++：引用传参
来源：http://hz.0kj1m.cn/gtpmzdxpmf.html

void inc(int &x) { ++x; }
来源：http://hz.zhixingplan.top/gtsfrqirsd.html

[S45] C++：lambda
来源：http://hz.hysaishi.cn/gtwnryymhx.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.shuidangran.top/gtirlflkwa.html

[S46] C++：函数模板
来源：http://hz.sufxvd.cn/gtlykzkapu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.52xcode.cn/gtmyvupkhi.html

[S47] C++：结构化绑定遍历
来源：http://hz.meibo888.top/gthfmnjmgb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.pycfn.com/gtclelnjmf.html

[S48] C++：逐行读文件
来源：http://hz.xuanzx.com/gtqvnsfopt.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhongyouzk.top/gtcqssfquk.html

while (std::getline(in, line)) { }
来源：http://hz.nanxuanxn.top/gtocvfdbit.html

[S49] C++：写文件
来源：http://hz.zdqjudy.top/gthoudrbnb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.xuetiantiany.cn/gtyypurrwf.html

[S50] C++：格式化数字
来源：http://hz.hnxiangtu.top/gtxksfynbb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yangfankeji.com/gtifwdqtwc.html

[S51] C++：显式类型转换
来源：http://hz.sweek.top/gtpumgqmfm.html

static_cast<double>(a) / b
来源：http://hz.hysaishi.cn/gtlyrdiwsy.html

[S52] C++：const 与 noexcept
来源：http://hz.hnxiangtu.top/gtigozumhp.html

int size() const noexcept { return n_; }
来源：http://hz.yonumen.top/gtqumhzvxs.html

[S53] C++：移动语义
来源：http://hz.52xcode.cn/gtkfzqmbyl.html

std::vector<int> w = std::move(v);
来源：http://hz.wangdashe.top/gtxpouqqrw.html

[S54] C++：异常处理
来源：http://hz.shangyingyoupin.top/gtpyshxpen.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jlsjyb.cn/gtegyqoxul.html

[S55] C++：结构化绑定
来源：http://hz.ivvv.top/gtdvfverci.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.52xcode.cn/gtvtqkdvwh.html

[S56] C++：optional
来源：http://hz.jinqigufen.top/gtcbtcgido.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.gotoacloud.top/gtrbkbbbvb.html

[S57] C++：编译期常量
来源：http://hz.wangshuangyany.cn/gtnxdfnfre.html

constexpr int N = 10;
来源：http://hz.xylfe.cn/gtqezjcnae.html

[S58] C++：命名空间
来源：http://hz.smart0.xyz/gtbpwhkanp.html

namespace ns { int f() { return 1; } }
来源：http://hz.yvedp.cn/gtuqefaxse.html

[S59] C++：静态断言
来源：http://hz.0kj1m.cn/gtuadogneg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jyoumei.cn/gtckelprxn.html

[S60] C++：遍历并删除元素
来源：http://hz.0kj1m.cn/gtoqxfgpvy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhengqikj.top/gtzojyprhw.html

================================================================================
来源：http://hz.shzxlz.cn/gtavcshngh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhengqikj.top/gtzdnvvwwy.html

================================================================================
来源：http://hz.xylfe.cn/gtggkqycus.html

[T01] Kotlin：Hello World
来源：http://hz.hysaishi.cn/gtolgiaign.html

println("Hello")
来源：http://hz.hysaishi.cn/gtbftnkqko.html

[T02] Kotlin：变量
来源：http://hz.daria6918.cn/gtnwrzsgnb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.gotoacloud.top/gtrurhvnhn.html

[T03] Kotlin：字符串模板
来源：http://hz.wangdashe.top/gtqthfuteo.html

"值: $b"
来源：http://hz.zdqjudy.top/gtbogekzql.html

[T04] Kotlin：空安全
来源：http://hz.xziqi.cn/gtwswbnkxv.html

val n: String? = null;  n?.length
来源：http://hz.sweek.top/gtaeqesvzy.html

[T05] Kotlin：when 表达式
来源：http://hz.andypj.xyz/gtldsidnet.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zhixingplan.top/gtrjuxwzdj.html

[T06] Kotlin：集合映射
来源：http://hz.chenzaomai.com/gtqwekxaba.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zdqjudy.top/gtnjtzpeav.html

[T07] Kotlin：集合过滤
来源：http://hz.feifeiyinyue.top/gtmirwtrem.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.chenjidiqi.icu/gteangwkqv.html

[T08] Kotlin：数据类
来源：http://hz.jiagoushi.top/gttbvkyolz.html

data class User(val name: String, val age: Int)
来源：http://hz.andypj.xyz/gtedopbtcv.html

[T09] Kotlin：扩展函数
来源：http://hz.gzhubu.top/gtnfpwvrgx.html

fun String.exclaim() = this + "!"
来源：http://hz.zhiwuduotai.top/gtyldfbnpv.html

[T10] Kotlin：默认参数
来源：http://hz.wangshuangyany.cn/gtyzvnjltj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.andypj.xyz/gtdtxijodt.html

[T11] Kotlin：协程
来源：http://hz.iojbl.cn/gtkmeyeukr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.daria6918.cn/gtygrwxudl.html

[T12] Kotlin：解构声明
来源：http://hz.yj20258.top/gtjyqqjuhz.html

val (a, b) = Pair(1, 2)
来源：http://hz.smart0.xyz/gtcigzaikh.html

[T13] Kotlin：只读 Map
来源：http://hz.tian-w.cn/gtmkshuokn.html

val m = mapOf("a" to 1)
来源：http://hz.nanxuanxn.top/gtygpfnsfj.html

[T14] Kotlin：循环
来源：http://hz.tanke756.top/gtgcvgayfz.html

for (i in 1..10) println(i)
来源：http://hz.jqgufenzy.top/gtkjmrtbft.html

[T15] Kotlin：接口
来源：http://hz.shanyushiyangtech.top/gtghokxdgc.html

interface Shape { fun area(): Double }
来源：http://hz.jinyuanbaomall.cn/gtkxhiuezj.html

[T16] Swift：Hello World
来源：http://hz.jqgufenzy.top/gtvtkxufyc.html

print("Hello")
来源：http://hz.xziqi.cn/gtzdducbsc.html

[T17] Swift：变量与常量
来源：http://hz.shzxlz.cn/gtsgojswde.html

var a = 1;  let b = 2
来源：http://hz.meibo888.top/gteuqajvat.html

[T18] Swift：字符串插值
来源：http://hz.hnxiangtu.top/gtwpjsabfi.html

"值: \(b)"
来源：http://hz.shanyushiyangkeji.top/gtkesyfwcq.html

[T19] Swift：可选绑定
来源：http://hz.gzhubu.top/gtqmiglyyh.html

if let n = opt { print(n) }
来源：http://hz.zhiwuduotai.top/gtjspnyksu.html

[T20] Swift：数组操作
来源：http://hz.yvedp.cn/gtujzkbstc.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.cashguo.top/gtigicfwyi.html

[T21] Swift：遍历
来源：http://hz.aizwys.cn/gtengznrts.html

for x in a { print(x) }
来源：http://hz.dashuyun.cn/gtwqrwskmc.html

[T22] Swift：字典
来源：http://hz.zdqjudy.top/gtdtnklgwt.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.chenlongwang.top/gtvjgytsqy.html

[T23] Swift：函数
来源：http://hz.dashuyun.cn/gtrmytgmne.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.pycfn.com/gtyokxuvvt.html

[T24] Swift：闭包
来源：http://hz.gotoacloud.top/gtezqijqfs.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.nanxinkj.top/gtfoobfhls.html

[T25] Swift：结构体
来源：http://hz.dashuyun.cn/gtvxgmlzsw.html

struct P { var x: Int }
来源：http://hz.jinqigfzy.top/gtvqnezcsg.html

[T26] Swift：类与重写
来源：http://hz.havefunace.top/gtdanbvmnl.html

class A: Base { override func f() {} }
来源：http://hz.zhaomingkeji.xyz/gtqzzigddr.html

[T27] Swift：错误处理
来源：http://hz.mhx1999.top/gtlillvmut.html

do { try f() } catch { print(error) }
来源：http://hz.gotoacloud.top/gtcpclzqoa.html

[T28] Swift：枚举
来源：http://hz.316326.xyz/gtnbsenivu.html

enum Color { case red, green }
来源：http://hz.daxiang520.top/gthozbhkfo.html

[T29] Swift：guard 提前返回
来源：http://hz.nanxuanxn.top/gtcjgosumb.html

guard let x = opt else { return }
来源：http://hz.yangfankeji.com/gtzzizktea.html

[T30] Swift：协议
来源：http://hz.xziqi.cn/gtctdjbaji.html

protocol Shape { func area() -> Double }
来源：http://hz.yangfankeji.com/gtspbponzz.html

[T31] Lua：Hello World
来源：http://hz.xuetiantiany.cn/gtvibetlov.html

print("Hello")
来源：http://hz.meibo888.top/gtozwkavrp.html

[T32] Lua：局部变量
来源：http://hz.xziqi.cn/gtnrnkpcbq.html

local a = 1
来源：http://hz.vqdsnc.cn/gtlwwhpdxz.html

[T33] Lua：表（数组）
来源：http://hz.ydjk.org.cn/gtepxtpuba.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.ivvv.top/gtpggrokav.html

[T34] Lua：遍历表
来源：http://hz.sufxvd.cn/gtfknuacov.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.nanxinkj.top/gtzebwzxru.html

[T35] Lua：字典表
来源：http://hz.zhixingplan.top/gtdpvxriee.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yj202588.top/gtngngrpdo.html

[T36] Lua：函数
来源：http://hz.pycfn.com/gtzxpiqyhc.html

function add(a, b) return a + b end
来源：http://hz.dashuyun.cn/gtscnvtqnk.html

[T37] Lua：字符串拼接
来源：http://hz.daxiang520.top/gtbmfqiqde.html

"a" .. "b"
来源：http://hz.xuanzx.com/gtwlnangab.html

[T38] Lua：条件
来源：http://hz.chenzaomai.com/gtswgwcspb.html

if x > 0 then print("正") end
来源：http://hz.feifeiyinyue.top/gtsvbnsdbv.html

[T39] Lua：模式匹配
来源：http://hz.yj20258888.top/gtjcljxtbe.html

string.find(s, "%d+")
来源：http://hz.gzhubu.top/gtaxhmtdbp.html

[T40] Lua：元表
来源：http://hz.cashguo.top/gtouflezwi.html

setmetatable({}, { __index = base })
来源：http://hz.ybcxt.top/gtfisyonow.html

[T41] Perl：Hello World
来源：http://hz.shzxlz.cn/gtvguxzhct.html

print "Hello\n";
来源：http://hz.redwolf501.top/gtrvwkgige.html

[T42] Perl：变量类型
来源：http://hz.xylfe.cn/gtaksgvsyu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yvedp.cn/gtyfrfnyxr.html

[T43] Perl：字符串插值
来源：http://hz.sufxvd.cn/gtyidmuzdw.html

"值: $a"
来源：http://hz.52xcode.cn/gtzmpipwfw.html

[T44] Perl：条件
来源：http://hz.hammf.cn/gtevqcykvi.html

if ($a > 0) { print "正"; }
来源：http://hz.guowangkeji.top/gtibfkqpms.html

[T45] Perl：数组遍历
来源：http://hz.gaohongyu789.top/gtkjlkgbdp.html

for my $x (@arr) { print $x; }
来源：http://hz.yvedp.cn/gtbuliyvjf.html

[T46] Perl：哈希操作
来源：http://hz.yongpay.top/gtcowgmubo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.shzxlz.cn/gtvgnpzkjg.html

[T47] Perl：正则捕获
来源：http://hz.pengpengdd.cyou/gtdzhlazvv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.ydzc1.top/gtoichtkhu.html

[T48] Perl：正则替换
来源：http://hz.yj202588.top/gtffjknijv.html

$s =~ s/old/new/g;
来源：http://hz.smart0.xyz/gtnowspfxu.html

[T49] Perl：函数
来源：http://hz.chenjidiqi.icu/gtdrqwklws.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jinghuilouyu.cn/gtphqyejpn.html

[T50] Perl：逐行读文件
来源：http://hz.ppjwa.cn/gtamktiqgw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.aizwys.cn/gtgtwphctp.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.pycfn.com/gtubhetdld.html

[T51] Scala：Hello World
来源：http://hz.yongpay.top/gtxfhcppuz.html

println("Hello")
来源：http://hz.ehwqpu.com/gtbimohupz.html

[T52] Scala：变量
来源：http://hz.ivvv.top/gtxcrwvbuk.html

val a = 1;  var b = 2
来源：http://hz.ppjwa.cn/gtqydindxz.html

[T53] Scala：字符串插值
来源：http://hz.meibo888.top/gtkvytznhh.html

s"值: $b"
来源：http://hz.zdqjudy.top/gtcfojsuwl.html

[T54] Scala：集合映射
来源：http://hz.zycfv.cn/gttpkselmh.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.xuanzx.com/gthxjnnjpg.html

[T55] Scala：集合过滤
来源：http://hz.zdqjudy.top/gtqzhezncp.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.shanyushiyangtech.top/gttjtnoyeg.html

[T56] Scala：样例类
来源：http://hz.cheryme.top/gtdtxeuqhx.html

case class User(name: String, age: Int)
来源：http://hz.jinqigufen.top/gtwlktpaaz.html

[T57] Scala：模式匹配
来源：http://hz.smart0.xyz/gtkugxaqag.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.gaohongyu789.top/gtukbwxbfd.html

[T58] Scala：函数定义
来源：http://hz.cheryme.top/gtlqyuxwzf.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.fzhhl.top/gtvksfqkms.html

[T59] Scala：循环
来源：http://hz.ydzc1.top/gtmbwfsqkc.html

for (i <- 1 to 10) println(i)
来源：http://hz.ywan-chungtsiang.top/gtisjneduq.html

[T60] Scala：折叠
来源：http://hz.yanxiufei.cn/gtrjtpigbj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.daria6918.cn/gtcwmvmvts.html

================================================================================
来源：http://hz.wangdashe.top/gttnsheuxq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yanxiufei.cn/gtgrtupgqu.html

================================================================================
来源：http://hz.iojbl.cn/gtmkupiyyp.html

[U01] Py：创建虚拟环境
来源：http://hz.chenzaomai.com/gtceixmmxf.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.xinyue.icu/gtitgoewrt.html

[U02] Py：导出 / 安装依赖
来源：http://hz.chenlongwang.top/gttlzakuop.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.ybcxt.top/gtuaayvqqi.html

[U03] Py：加载 .env 配置
来源：http://hz.shzxlz.cn/gtutsmhduj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jiagoushi.top/gthigwdhbr.html

[U04] Py：变量调试打印
来源：http://hz.ivvv.top/gtjtcuwcrr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.cheryme.top/gtcgknohce.html

[U05] Py：列表去重且保序
来源：http://hz.haohaochexian.top/gtpnrzugeb.html

list(dict.fromkeys(arr))
来源：http://hz.dianchejie.cn/gtlzzfddim.html

[U06] Py：合并两个字典
来源：http://hz.tanke756.top/gtgcgdcltf.html

{**a, **b}
来源：http://hz.jinyuanbaomall.cn/gtlxoriozw.html

[U07] Py：反转字典键值
来源：http://hz.tianlin.xyz/gtwnrkkdtd.html

{v: k for k, v in d.items()}
来源：http://hz.ywan-chungtsiang.top/gtxpjthohb.html

[U08] Py：展平二维列表
来源：http://hz.jlsjyb.cn/gtuzuuofck.html

[y for x in nested for y in x]
来源：http://hz.0kj1m.cn/gtblxczhds.html

[U09] Py：字典取最大值的键
来源：http://hz.jqgfzy.top/gttlioelfb.html

max(d, key=d.get)
来源：http://hz.chenzaomai.com/gtpgkbnwur.html

[U10] Py：按值排序字典
来源：http://hz.feifeiyinyue.top/gtyeopgjie.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.guannengcc.top/gtawkitnop.html

[U11] Py：生成器表达式
来源：http://hz.yj20258888.top/gteuitevrt.html

(x * 2 for x in arr)
来源：http://hz.ydjk.org.cn/gtnmmrbjmh.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yvedp.cn/gtwdjkkrku.html

Counter(arr).most_common(3)
来源：http://hz.wangshuangyany.cn/gtmaydxtqg.html

[U13] Py：固定长度队列
来源：http://hz.snrcjt.cn/gtdopwtwdc.html

deque(maxlen=10)
来源：http://hz.aizwys.cn/gtzarjxarm.html

[U14] Py：分组收集到列表
来源：http://hz.jinqigfzy.top/gthufjqapj.html

defaultdict(list)
来源：http://hz.hnqzz.top/gtwmxmyaba.html

[U15] Py：高精度计时
来源：http://hz.jinghuilouyu.cn/gtxmqytjnx.html

t = time.perf_counter()
来源：http://hz.jinyuanbaomall.cn/gtxabylwmd.html

[U16] Py：命令行参数解析
来源：http://hz.meibo888.top/gtuumgcqvx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.snrcjt.cn/gtibhejpkd.html

[U17] Py：初始化日志
来源：http://hz.ywan-chungtsiang.top/gtqgmsaxdg.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.svipenyu.cn/gtwpbgvuyw.html

[U18] Py：预编译正则
来源：http://hz.jlsjyb.cn/gtchhmjygf.html

pat = re.compile(r"\d+")
来源：http://hz.sysykeji.top/gtrrtqrbwi.html

[U19] Py：正则替换带回调
来源：http://hz.meibo888.top/gtzhxdqzkl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.shzxlz.cn/gtybnestlb.html

[U20] Py：缓存函数结果
来源：http://hz.chenjidiqi.icu/gtleizehtj.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jianghu66.top/gttchirfdp.html

[U21] Py：自定义上下文管理器
来源：http://hz.fzhhl.top/gteyysafpu.html

@contextlib.contextmanager
来源：http://hz.smart0.xyz/gtluawfnkn.html

[U22] Py：矩阵转置
来源：http://hz.jianghu66.top/gtdwdfhjao.html

list(zip(*m))
来源：http://hz.haohaochexian.top/gtvnitiabr.html

[U23] Py：分块读取大文件
来源：http://hz.chenlongwang.top/gtljlhiqnb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.birdmap.top/gtelxjjapp.html

[U24] Py：路径操作
来源：http://hz.snrcjt.cn/gtgttpxuqu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.sysykeji.top/gtwyxzyipn.html

[U25] Py：CSV 按字典读
来源：http://hz.iojbl.cn/gtgyfpylzc.html

csv.DictReader(f)
来源：http://hz.quarkkingdee.top/gtztfyezdb.html

[U26] Py：并发下载
来源：http://hz.chenzaomai.com/gtvvddjljh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.sxryk.cn/gtpxvrxmps.html

[U27] Py：异步 HTTP
来源：http://hz.ydzc1.top/gtravbzajw.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.nanxinkj.top/gtljylzmir.html

[U28] Py：类型别名
来源：http://hz.andypj.xyz/gtwzrqyslg.html

UserId = int
来源：http://hz.yonumen.top/gtggakumhq.html

[U29] Py：属性校验
来源：http://hz.aibaodan.cn/gtrxczhcly.html

@property 与 @x.setter 配合
来源：http://hz.ivvv.top/gtiwnmlkzt.html

[U30] Py：数据类
来源：http://hz.gzhubu.top/gtxotohdzv.html

@dataclass(slots=True)
来源：http://hz.hysaishi.cn/gtuyyctrxl.html

[U31] Py：单测
来源：http://hz.wangshuangyany.cn/gtuwcongbn.html

python -m pytest -q
来源：http://hz.ywan-chungtsiang.top/gtkqctwxde.html

[U32] Py：代码格式化
来源：http://hz.jinqigufen.top/gtqdrumexg.html

ruff format . && ruff check --fix .
来源：http://hz.snrcjt.cn/gtxfcpwlvg.html

[U33] Py：打包发布
来源：http://hz.jinghuilouyu.cn/gtvqhwbtpu.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.zhixingplan.top/gteqfkjidh.html

[U34] Py：判断编码
来源：http://hz.ywan-chungtsiang.top/gtzukghlcs.html

chardet.detect(raw)
来源：http://hz.bjfxy.top/gtdhoxrbkc.html

[U35] Py：发送邮件
来源：http://hz.jianghu66.top/gtvkovoyou.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.hywenlv.cn/gtgqnhgtwn.html

[U36] Py：定时任务
来源：http://hz.jinghuilouyu.cn/gtcnwpjlse.html

schedule.every(10).minutes.do(job)
来源：http://hz.jqgfzy.top/gtceytxdlw.html

[U37] Py：读写 Excel
来源：http://hz.xuetiantiany.cn/gtvbcjacie.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.zhijiandao.cn/gtqooagfdm.html

[U38] Py：获取脚本所在目录
来源：http://hz.zhengqikj.top/gtzeqyefuk.html

Path(__file__).resolve().parent
来源：http://hz.jinghuilouyu.cn/gtxxafeghq.html


<!-- 参考信息 -->