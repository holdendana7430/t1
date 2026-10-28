代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.cdnleiting.top/gtpqwfpnmv.html

[S13] C：宏定义
来源：http://hz.yanxiufei.cn/gtyjgpvmgx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.kuanghao11.cn/gtbffwlxcm.html

[S14] C：枚举
来源：http://hz.jinyuanbaomall.cn/gtmvyhnopz.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.gogol.net.cn/gtjpdsedvl.html

[S15] C：类型转换
来源：http://hz.yuxming.cn/gttqmronjk.html

(double) a / b
来源：http://hz.shuidangran.top/gtmtrezzka.html

[S16] C：位操作置位
来源：http://hz.nanxuanxn.top/gtgyutitfr.html

x |= (1 << 3);
来源：http://hz.jiagoushi.top/gtaivkoajk.html

[S17] C：安全拼接字符串
来源：http://hz.c1oappe.top/gtqrxzgzro.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yonumen.top/gtmmmzwkdz.html

[S18] C：命令行参数
来源：http://hz.yongpay.top/gtvqkfzodd.html

int main(int argc, char **argv)
来源：http://hz.sysykeji.top/gtevocxwqz.html

[S19] C：快速排序
来源：http://hz.52xcode.cn/gtxzrcqgzi.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hywenlv.cn/gttgjefptz.html

[S20] C：二分查找
来源：http://hz.jianghu66.top/gtkgglleqh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hysaishi.cn/gtxygoizyx.html

[S21] C：字符类别判断
来源：http://hz.cqqwz.cn/gtlagohwvv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yueranfly.top/gtqlpeliny.html

[S22] C：字符串转数字
来源：http://hz.yj202588.top/gthsbejigf.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yangfankeji.com/gtdkwyoipi.html

[S23] C：随机数
来源：http://hz.vqdsnc.cn/gtnmunbfaz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhiwuduotai.top/gtmjltjkvu.html

[S24] C：获取本地时间
来源：http://hz.cashguo.top/gtvofubknx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xuanzx.com/gtvfpzgbji.html

[S25] C：内存拷贝
来源：http://hz.zhijiandao.cn/gtwfuszoqc.html

memcpy(dst, src, n);
来源：http://hz.yuanzhike.top/gtakoxaqfo.html

[S26] C：内存清零
来源：http://hz.pengpengdd.cyou/gthemlyueb.html

memset(a, 0, sizeof a);
来源：http://hz.jlsjyb.cn/gtgbtsived.html

[S27] C：定义常量
来源：http://hz.nwbrower.top/gtykmecedz.html

const double PI = 3.14159;
来源：http://hz.svipenyu.cn/gtnkjrsckv.html

[S28] C：静态变量
来源：http://hz.yangfankeji.com/gtqgnmimje.html

static int counter = 0;
来源：http://hz.shanyushiyangkeji.top/gtjywimagh.html

[S29] C：变参函数
来源：http://hz.yuanzhike.top/gtwvvtlhhx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.iojbl.cn/gtztcrktma.html

[S30] C：头文件保护
来源：http://hz.316326.xyz/gtpwnngiyy.html

#ifndef X_H
来源：http://hz.ppjwa.cn/gtjkplsonr.html

#define X_H
来源：http://hz.cqqwz.cn/gtafxuwcxj.html

#endif
来源：http://hz.ydzc1.top/gtxnakimjd.html

[S31] C++：Hello World
来源：http://hz.aibaodan.cn/gtipvaxrhw.html

#include <iostream>
来源：http://hz.fzhhl.top/gtasyonixx.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.wangshuangyany.cn/gtjdhkljtb.html

[S32] C++：字符串
来源：http://hz.xuetiantiany.cn/gtqtcaymlc.html

std::string s = "hi";  s += "!";
来源：http://hz.dianchejie.cn/gtkygkkkvw.html

[S33] C++：vector 增删
来源：http://hz.c1oappe.top/gtikeshhwu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.chenlongwang.top/gtdaapuueh.html

[S34] C++：遍历 vector
来源：http://hz.hnqzz.top/gternftmrd.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ehwqpu.com/gttyofeepp.html

[S35] C++：map
来源：http://hz.dianchejie.cn/gtjwefutsc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.0kj1m.cn/gtlyitnypm.html

[S36] C++：unordered_map
来源：http://hz.fzhhl.top/gtlyssjosj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jiagoushi.top/gtljchbawd.html

[S37] C++：set
来源：http://hz.jinqigufen.top/gtmbkhyorw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ydjk.org.cn/gtxqbzfwja.html

[S38] C++：排序
来源：http://hz.hongshengwenyu.top/gtpjbhymse.html

std::sort(v.begin(), v.end());
来源：http://hz.gogol.net.cn/gthjdjhuyh.html

[S39] C++：自定义比较器排序
来源：http://hz.yonumen.top/gtcbblhjpp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yueranfly.top/gtmvatbaaw.html

[S40] C++：查找元素
来源：http://hz.birdmap.top/gtomijojua.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhixingplan.top/gtgncgifuq.html

[S41] C++：类与构造函数
来源：http://hz.yangfankeji.com/gtigbvtvaq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ydjk.org.cn/gtevnhtofc.html

[S42] C++：继承与虚函数
来源：http://hz.fengsongda.top/gtjfhbzfcu.html

class B : public Base { public: void f() override {} };
来源：http://hz.snrcjt.cn/gtsikhojna.html

[S43] C++：智能指针
来源：http://hz.meibo888.top/gtpfkacigm.html

auto p = std::make_unique<int>(5);
来源：http://hz.hammf.cn/gtjgqlqsgv.html

[S44] C++：引用传参
来源：http://hz.jlsjyb.cn/gtuvydodmi.html

void inc(int &x) { ++x; }
来源：http://hz.pengpengdd.cyou/gtqhcbvjtj.html

[S45] C++：lambda
来源：http://hz.ybcxt.top/gtwwpcvoba.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.aizwys.cn/gtgqavaimw.html

[S46] C++：函数模板
来源：http://hz.aizwys.cn/gtoykdtbzv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yvedp.cn/gtoqqqhnuj.html

[S47] C++：结构化绑定遍历
来源：http://hz.smart0.xyz/gtbpkwzpwc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.hysaishi.cn/gtngvwchfq.html

[S48] C++：逐行读文件
来源：http://hz.jlsjyb.cn/gtfekuojgp.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.mhx1999.top/gtbtiwxfvq.html

while (std::getline(in, line)) { }
来源：http://hz.jyoumei.cn/gtvonafooz.html

[S49] C++：写文件
来源：http://hz.sufxvd.cn/gtegirchrd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.chenjidiqi.icu/gtwkeagdcd.html

[S50] C++：格式化数字
来源：http://hz.ywan-chungtsiang.top/gtgxxopuyn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.xylfe.cn/gtpwnhotke.html

[S51] C++：显式类型转换
来源：http://hz.yangfankeji.com/gtiwndhcrv.html

static_cast<double>(a) / b
来源：http://hz.52xcode.cn/gtqciexxkr.html

[S52] C++：const 与 noexcept
来源：http://hz.yvedp.cn/gtaxvsrrnc.html

int size() const noexcept { return n_; }
来源：http://hz.haohaochexian.top/gtakjdnigy.html

[S53] C++：移动语义
来源：http://hz.haohaochexian.top/gtomjgazun.html

std::vector<int> w = std::move(v);
来源：http://hz.cucudq.cn/gtlfoyipzq.html

[S54] C++：异常处理
来源：http://hz.ywan-chungtsiang.top/gtkeflpdtw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.fengsongda.top/gtustslhjz.html

[S55] C++：结构化绑定
来源：http://hz.jqgfzy.top/gtzdjdcbru.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.gogol.net.cn/gtamsflytk.html

[S56] C++：optional
来源：http://hz.hnqzz.top/gtopdcnhll.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.ywan-chungtsiang.top/gttanxuesg.html

[S57] C++：编译期常量
来源：http://hz.sysykeji.top/gtdyzbwqci.html

constexpr int N = 10;
来源：http://hz.hongshengwenyu.top/gtmlwvocxp.html

[S58] C++：命名空间
来源：http://hz.hammf.cn/gtoqmvkykv.html

namespace ns { int f() { return 1; } }
来源：http://hz.ydjk.org.cn/gtchlsfcrc.html

[S59] C++：静态断言
来源：http://hz.dashuyun.cn/gtavussdae.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.tianlin.xyz/gtknmwbudn.html

[S60] C++：遍历并删除元素
来源：http://hz.tianlin.xyz/gtawtorfna.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.vqdsnc.cn/gtwidzhoja.html

================================================================================
来源：http://hz.jyoumei.cn/gtsonvqlng.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.gogol.net.cn/gtcybrhjts.html

================================================================================
来源：http://hz.hysaishi.cn/gtvlgupjpl.html

[T01] Kotlin：Hello World
来源：http://hz.daria6918.cn/gtnycqmsta.html

println("Hello")
来源：http://hz.xinyue.icu/gtjalllakh.html

[T02] Kotlin：变量
来源：http://hz.yonumen.top/gtgovsfcoz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.mhx1999.top/gtbmpubdxr.html

[T03] Kotlin：字符串模板
来源：http://hz.hammf.cn/gtbggusbwy.html

"值: $b"
来源：http://hz.chenzaomai.com/gtpjlbddik.html

[T04] Kotlin：空安全
来源：http://hz.zhijiandao.cn/gtcgrvkmxg.html

val n: String? = null;  n?.length
来源：http://hz.ivvv.top/gtigrurbes.html

[T05] Kotlin：when 表达式
来源：http://hz.xingfuxueyuan.xyz/gtgesgdvnw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.svipenyu.cn/gtnaftktsf.html

[T06] Kotlin：集合映射
来源：http://hz.sxryk.cn/gtbzosejee.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.snrcjt.cn/gtmrcnwetz.html

[T07] Kotlin：集合过滤
来源：http://hz.hfpthk.cn/gthgzeqoca.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.tanke756.top/gtlcfxakcz.html

[T08] Kotlin：数据类
来源：http://hz.svipenyu.cn/gtxctocinx.html

data class User(val name: String, val age: Int)
来源：http://hz.xinyue.icu/gtpxvrropx.html

[T09] Kotlin：扩展函数
来源：http://hz.tianlin.xyz/gtbevtmpbb.html

fun String.exclaim() = this + "!"
来源：http://hz.sxryk.cn/gtxkmcoynu.html

[T10] Kotlin：默认参数
来源：http://hz.ehwqpu.com/gthrsxkkff.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jinqigfzy.top/gtrctafdyl.html

[T11] Kotlin：协程
来源：http://hz.jyoumei.cn/gtuiwokzhj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.hnxiangtu.top/gttahemqpc.html

[T12] Kotlin：解构声明
来源：http://hz.nanxuanxn.top/gthyqpxxrt.html

val (a, b) = Pair(1, 2)
来源：http://hz.tianlin.xyz/gtngvcnegz.html

[T13] Kotlin：只读 Map
来源：http://hz.shuidangran.top/gtwiniasot.html

val m = mapOf("a" to 1)
来源：http://hz.daxiang520.top/gtslxuewjt.html

[T14] Kotlin：循环
来源：http://hz.zhoulong.xyz/gtdevmcokz.html

for (i in 1..10) println(i)
来源：http://hz.wangshuangyany.cn/gtawbzxuue.html

[T15] Kotlin：接口
来源：http://hz.shuidangran.top/gtodkqgkvf.html

interface Shape { fun area(): Double }
来源：http://hz.ehwqpu.com/gtytwwfrxn.html

[T16] Swift：Hello World
来源：http://hz.dianchejie.cn/gtuhahungk.html

print("Hello")
来源：http://hz.xuanzx.com/gtyaaxaelq.html

[T17] Swift：变量与常量
来源：http://hz.shangyingyoupin.top/gtudmkupyg.html

var a = 1;  let b = 2
来源：http://hz.cashguo.top/gtnyicyxte.html

[T18] Swift：字符串插值
来源：http://hz.zdqjudy.top/gtcjazsbir.html

"值: \(b)"
来源：http://hz.smart0.xyz/gtulnpvdev.html

[T19] Swift：可选绑定
来源：http://hz.pycfn.com/gtznmvodnk.html

if let n = opt { print(n) }
来源：http://hz.yanxiufei.cn/gtczywbshg.html

[T20] Swift：数组操作
来源：http://hz.0kj1m.cn/gtthunyyrx.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.ehwqpu.com/gtlpudlwtl.html

[T21] Swift：遍历
来源：http://hz.jqgfzy.top/gtkxumqabf.html

for x in a { print(x) }
来源：http://hz.yongpay.top/gtzmgizpus.html

[T22] Swift：字典
来源：http://hz.hysaishi.cn/gtjgfrcwke.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yvedp.cn/gtlxuqpfdj.html

[T23] Swift：函数
来源：http://hz.zdqjudy.top/gtdzbxhfja.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.sysykeji.top/gtfpfwygqo.html

[T24] Swift：闭包
来源：http://hz.redwolf501.top/gtsiqmsjka.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.shzxlz.cn/gtngakhkmf.html

[T25] Swift：结构体
来源：http://hz.52xcode.cn/gtvywzonql.html

struct P { var x: Int }
来源：http://hz.jianghu66.top/gtrgoztijr.html

[T26] Swift：类与重写
来源：http://hz.wangshuangyany.cn/gtcsduxofp.html

class A: Base { override func f() {} }
来源：http://hz.nanxuanxn.top/gttklncjsz.html

[T27] Swift：错误处理
来源：http://hz.316326.xyz/gtibpsknon.html

do { try f() } catch { print(error) }
来源：http://hz.hfpthk.cn/gtivurlrnb.html

[T28] Swift：枚举
来源：http://hz.zhijiandao.cn/gtydfxjmmq.html

enum Color { case red, green }
来源：http://hz.gzhubu.top/gtbbgnqpff.html

[T29] Swift：guard 提前返回
来源：http://hz.dashuyun.cn/gthhygqxee.html

guard let x = opt else { return }
来源：http://hz.shuidangran.top/gtvzkxoonl.html

[T30] Swift：协议
来源：http://hz.hysaishi.cn/gttcwumoxi.html

protocol Shape { func area() -> Double }
来源：http://hz.pengpengdd.cyou/gtafkrbgho.html

[T31] Lua：Hello World
来源：http://hz.redwolf501.top/gtbsbzyesf.html

print("Hello")
来源：http://hz.shanyushiyangkeji.top/gtxettqtws.html

[T32] Lua：局部变量
来源：http://hz.ybcxt.top/gtgkrduvpo.html

local a = 1
来源：http://hz.sxryk.cn/gtilitrcha.html

[T33] Lua：表（数组）
来源：http://hz.c1oappe.top/gtkdpgxism.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.hnqzz.top/gtyrnerbgx.html

[T34] Lua：遍历表
来源：http://hz.xuanzx.com/gtkfciznjh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.redwolf501.top/gttbihobzu.html

[T35] Lua：字典表
来源：http://hz.zhijiandao.cn/gtjyzdfqsi.html

local d = { a = 1 };  d.b = 2
来源：http://hz.zhijiandao.cn/gtlzxprnre.html

[T36] Lua：函数
来源：http://hz.redwolf501.top/gtmptjtxpu.html

function add(a, b) return a + b end
来源：http://hz.zycfv.cn/gtrxkkkmgw.html

[T37] Lua：字符串拼接
来源：http://hz.sysykeji.top/gtcesflfjj.html

"a" .. "b"
来源：http://hz.iojbl.cn/gtliqryuoc.html

[T38] Lua：条件
来源：http://hz.cdnleiting.top/gtsdjykpzw.html

if x > 0 then print("正") end
来源：http://hz.guowangkeji.top/gtnvrspzen.html

[T39] Lua：模式匹配
来源：http://hz.daxiang520.top/gtjxnutnnj.html

string.find(s, "%d+")
来源：http://hz.hysaishi.cn/gtnrbhyqzw.html

[T40] Lua：元表
来源：http://hz.cqqwz.cn/gtwnceutkr.html

setmetatable({}, { __index = base })
来源：http://hz.hfpthk.cn/gtwnfuoyly.html

[T41] Perl：Hello World
来源：http://hz.quarkkingdee.top/gtxxvgiqly.html

print "Hello\n";
来源：http://hz.chenlongwang.top/gtnkjgyhxc.html

[T42] Perl：变量类型
来源：http://hz.ehwqpu.com/gtcmeqhrfd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.316326.xyz/gtahooftub.html

[T43] Perl：字符串插值
来源：http://hz.andypj.xyz/gtfaicqccl.html

"值: $a"
来源：http://hz.sweek.top/gtukmkktkp.html

[T44] Perl：条件
来源：http://hz.quarkkingdee.top/gttayydhii.html

if ($a > 0) { print "正"; }
来源：http://hz.svipenyu.cn/gtwuixifps.html

[T45] Perl：数组遍历
来源：http://hz.shuidangran.top/gtchrvgqxe.html

for my $x (@arr) { print $x; }
来源：http://hz.yueranfly.top/gtxlnsffuj.html

[T46] Perl：哈希操作
来源：http://hz.tianlin.xyz/gtwumswncc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jianghu66.top/gttlbzkmpc.html

[T47] Perl：正则捕获
来源：http://hz.haohaochexian.top/gtwhdhsjqf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.shanyushiyangkeji.top/gtggqfprpc.html

[T48] Perl：正则替换
来源：http://hz.hywenlv.cn/gtwuznxhml.html

$s =~ s/old/new/g;
来源：http://hz.zhiwuduotai.top/gtflsbnkiq.html

[T49] Perl：函数
来源：http://hz.xuetiantiany.cn/gtnknqabtd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.svipenyu.cn/gteaqchsuu.html

[T50] Perl：逐行读文件
来源：http://hz.yvedp.cn/gttlefdkyu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.hfpthk.cn/gtswssqpnm.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.ivvv.top/gtyfidfkmg.html

[T51] Scala：Hello World
来源：http://hz.fengsongda.top/gtnohxyyrf.html

println("Hello")
来源：http://hz.xziqi.cn/gtpjawjyje.html

[T52] Scala：变量
来源：http://hz.ydjk.org.cn/gtjxmmtled.html

val a = 1;  var b = 2
来源：http://hz.zdqjudy.top/gtaoooxiwk.html

[T53] Scala：字符串插值
来源：http://hz.cqqwz.cn/gtljscquim.html

s"值: $b"
来源：http://hz.zycfv.cn/gttjvayxiw.html

[T54] Scala：集合映射
来源：http://hz.fengsongda.top/gtofwqjxhb.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.dianchejie.cn/gtfngckaei.html

[T55] Scala：集合过滤
来源：http://hz.hysaishi.cn/gtfchrmfmv.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.wangdashe.top/gtfhpoloav.html

[T56] Scala：样例类
来源：http://hz.shanyushiyangkeji.top/gtfedkdhkz.html

case class User(name: String, age: Int)
来源：http://hz.yuxming.cn/gtickyudhg.html

[T57] Scala：模式匹配
来源：http://hz.nanxuanxn.top/gtdpgtnbis.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.yanxiufei.cn/gtlxtztbjz.html

[T58] Scala：函数定义
来源：http://hz.tian-w.cn/gtwdljstju.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jqgufenzy.top/gtqgqsxvfj.html

[T59] Scala：循环
来源：http://hz.zhiwuduotai.top/gtxgxywzmi.html

for (i <- 1 to 10) println(i)
来源：http://hz.andypj.xyz/gtihcmfful.html

[T60] Scala：折叠
来源：http://hz.0kj1m.cn/gtvggyrzra.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.shanyushiyangtech.top/gtrinclnik.html

================================================================================
来源：http://hz.zhoulong.xyz/gtucxoldsp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.tanke756.top/gtnxkhngbr.html

================================================================================
来源：http://hz.chenzaomai.com/gtknslzbhx.html

[U01] Py：创建虚拟环境
来源：http://hz.yangfankeji.com/gtytujsbbh.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.xziqi.cn/gtgmkmowlm.html

[U02] Py：导出 / 安装依赖
来源：http://hz.zhixingplan.top/gtattdpjfu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.chenzaomai.com/gtqnrkcjau.html

[U03] Py：加载 .env 配置
来源：http://hz.hywenlv.cn/gtgutjfqdf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.daxiang520.top/gtripswfip.html

[U04] Py：变量调试打印
来源：http://hz.jinqigfzy.top/gtdervtrrl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.shuidangran.top/gtjkcvvtvg.html

[U05] Py：列表去重且保序
来源：http://hz.xuetiantiany.cn/gtropxjtfw.html

list(dict.fromkeys(arr))
来源：http://hz.yj20258.top/gtzgzggxsf.html

[U06] Py：合并两个字典
来源：http://hz.chenjidiqi.icu/gtawxvweiw.html

{**a, **b}
来源：http://hz.shzxlz.cn/gtfloluzjh.html

[U07] Py：反转字典键值
来源：http://hz.aizwys.cn/gtrubkexhj.html

{v: k for k, v in d.items()}
来源：http://hz.hongshengwenyu.top/gtdyjhygbi.html

[U08] Py：展平二维列表
来源：http://hz.iojbl.cn/gtvhnfxoud.html

[y for x in nested for y in x]
来源：http://hz.haohaochexian.top/gtayjajxqg.html

[U09] Py：字典取最大值的键
来源：http://hz.chenzaomai.com/gtwphhyciw.html

max(d, key=d.get)
来源：http://hz.sufxvd.cn/gttdiyvjov.html

[U10] Py：按值排序字典
来源：http://hz.ydzc1.top/gtvgrabjcm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.jyoumei.cn/gtekkezmnt.html

[U11] Py：生成器表达式
来源：http://hz.gotoacloud.top/gtdukeiiai.html

(x * 2 for x in arr)
来源：http://hz.jinqigufen.top/gtnizortvu.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yj20258888.top/gtlgzqzzee.html

Counter(arr).most_common(3)
来源：http://hz.cucudq.cn/gtflvzfydl.html

[U13] Py：固定长度队列
来源：http://hz.mhx1999.top/gtnjnirbbc.html

deque(maxlen=10)
来源：http://hz.zdqjudy.top/gtdczzsjhb.html

[U14] Py：分组收集到列表
来源：http://hz.fengsongda.top/gtztiegjmr.html

defaultdict(list)
来源：http://hz.gogol.net.cn/gtrywuyytw.html

[U15] Py：高精度计时
来源：http://hz.ppjwa.cn/gtcilboeek.html

t = time.perf_counter()
来源：http://hz.jinqigufen.top/gtyrkdzppf.html

[U16] Py：命令行参数解析
来源：http://hz.hnqzz.top/gtuwemmfej.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.mhx1999.top/gtjjclksds.html

[U17] Py：初始化日志
来源：http://hz.wangshuangyany.cn/gtrenuxsfo.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.jqgfzy.top/gtnnmczixy.html

[U18] Py：预编译正则
来源：http://hz.feifeiyinyue.top/gtctzdzsef.html

pat = re.compile(r"\d+")
来源：http://hz.gzhubu.top/gtquszlfmz.html

[U19] Py：正则替换带回调
来源：http://hz.xuanzx.com/gtmaoahwud.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.iojbl.cn/gteqcduqka.html

[U20] Py：缓存函数结果
来源：http://hz.ywan-chungtsiang.top/gtvhexoxyb.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jiagoushi.top/gteraueawl.html

[U21] Py：自定义上下文管理器
来源：http://hz.aizwys.cn/gtwocazzhl.html

@contextlib.contextmanager
来源：http://hz.xziqi.cn/gtbgivtkvs.html

[U22] Py：矩阵转置
来源：http://hz.jinqigfzy.top/gtxsfiqyxp.html

list(zip(*m))
来源：http://hz.xinyue.icu/gtjraijrtc.html

[U23] Py：分块读取大文件
来源：http://hz.kuanghao11.cn/gtuwphudng.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.xuetiantiany.cn/gtxgiwwpzk.html

[U24] Py：路径操作
来源：http://hz.hnxiangtu.top/gtxdkeutly.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.svipenyu.cn/gtopcadvub.html

[U25] Py：CSV 按字典读
来源：http://hz.shangyingyoupin.top/gtcidztuxs.html

csv.DictReader(f)
来源：http://hz.316326.xyz/gtdqrfxidv.html

[U26] Py：并发下载
来源：http://hz.pengpengdd.cyou/gtybxnklfp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.yonumen.top/gtqjrdclku.html

[U27] Py：异步 HTTP
来源：http://hz.ydjk.org.cn/gtxupczluw.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.gaohongyu789.top/gtalbxbegk.html

[U28] Py：类型别名
来源：http://hz.cucudq.cn/gthkmlebdg.html

UserId = int
来源：http://hz.xingfuxueyuan.xyz/gtahhlyybe.html

[U29] Py：属性校验
来源：http://hz.aibaodan.cn/gtbjhuwpvr.html

@property 与 @x.setter 配合
来源：http://hz.feifeiyinyue.top/gtcrkjcgrl.html

[U30] Py：数据类
来源：http://hz.xuetiantiany.cn/gtoojwtlad.html

@dataclass(slots=True)
来源：http://hz.hywenlv.cn/gtwgjkjbqr.html

[U31] Py：单测
来源：http://hz.wangshuangyany.cn/gttpzoajmr.html

python -m pytest -q
来源：http://hz.gaohongyu789.top/gtgbzppqkp.html

[U32] Py：代码格式化
来源：http://hz.sweek.top/gtxqwtaoud.html

ruff format . && ruff check --fix .
来源：http://hz.hfpthk.cn/gtzcdqzmhi.html

[U33] Py：打包发布
来源：http://hz.xylfe.cn/gtmpqcsren.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.vqdsnc.cn/gtiedfhxlv.html

[U34] Py：判断编码
来源：http://hz.cucudq.cn/gthfuqrfet.html

chardet.detect(raw)
来源：http://hz.xingfuxueyuan.xyz/gtsuwkzsrv.html

[U35] Py：发送邮件
来源：http://hz.gzhubu.top/gteuckuuln.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.sufxvd.cn/gtjgtclgby.html

[U36] Py：定时任务
来源：http://hz.316326.xyz/gtjxswjmnt.html

schedule.every(10).minutes.do(job)
来源：http://hz.chenjidiqi.icu/gtfckmrlns.html


<!-- 参考信息 -->