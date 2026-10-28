代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yvedp.cn/gtvxqicxux.html

[S08] C：动态内存分配与释放
来源：http://hz.wangdashe.top/gtazpoxdmk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ehwqpu.com/gtuzymharm.html

[S09] C：结构体定义与初始化
来源：http://hz.zhengqikj.top/gtcryyiakj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.mhx1999.top/gtzbrrccxm.html

[S10] C：指针与解引用
来源：http://hz.yongpay.top/gtztwhaleu.html

int *p = &a;  *p = 5;
来源：http://hz.xuanzx.com/gtevjekbvh.html

[S11] C：逐行读文件
来源：http://hz.ppjwa.cn/gtvraphffd.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.vqdsnc.cn/gtliepiped.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.xuanzx.com/gthwwuvehq.html

fclose(f);
来源：http://hz.zhijiandao.cn/gtzofhsnbw.html

[S12] C：写文件
来源：http://hz.nanxuanxn.top/gtsnfhgsil.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hysaishi.cn/gtyrhfejoj.html

[S13] C：宏定义
来源：http://hz.feifeiyinyue.top/gtqqfqmfhg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.fengsongda.top/gteiczbyzu.html

[S14] C：枚举
来源：http://hz.jyoumei.cn/gtsvgadgqm.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.gotoacloud.top/gtimcomjwl.html

[S15] C：类型转换
来源：http://hz.xingfuxueyuan.xyz/gttnypymfi.html

(double) a / b
来源：http://hz.cdnleiting.top/gtmevavklc.html

[S16] C：位操作置位
来源：http://hz.xuanzx.com/gtjfpacrce.html

x |= (1 << 3);
来源：http://hz.jinqigufen.top/gtbfyauhda.html

[S17] C：安全拼接字符串
来源：http://hz.daxiang520.top/gtyajxsixg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xinyue.icu/gttrnpxoqh.html

[S18] C：命令行参数
来源：http://hz.sxryk.cn/gtmbgxtfpi.html

int main(int argc, char **argv)
来源：http://hz.zhoulong.xyz/gtgryrrbrn.html

[S19] C：快速排序
来源：http://hz.hnqzz.top/gtnldoahtt.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.sufxvd.cn/gtfmqeqnqi.html

[S20] C：二分查找
来源：http://hz.xingfuxueyuan.xyz/gtxbbbcwfd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yj20258888.top/gtavkzaqgk.html

[S21] C：字符类别判断
来源：http://hz.0kj1m.cn/gttcircjee.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ehwqpu.com/gtxydnjyln.html

[S22] C：字符串转数字
来源：http://hz.chenzaomai.com/gtomfkoklv.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yanxiufei.cn/gtitnaydmn.html

[S23] C：随机数
来源：http://hz.jinqigufen.top/gttgxuncac.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.shangyingyoupin.top/gtlhyaocuz.html

[S24] C：获取本地时间
来源：http://hz.jiagoushi.top/gtcfdyhtju.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ydjk.org.cn/gtwvjpnhxb.html

[S25] C：内存拷贝
来源：http://hz.cheryme.top/gtlnpgriin.html

memcpy(dst, src, n);
来源：http://hz.xinyue.icu/gtjcyhzzxj.html

[S26] C：内存清零
来源：http://hz.haohaochexian.top/gtqeoywhvg.html

memset(a, 0, sizeof a);
来源：http://hz.jiagoushi.top/gtrrgruutt.html

[S27] C：定义常量
来源：http://hz.nanxinkj.top/gtsfscmwwx.html

const double PI = 3.14159;
来源：http://hz.jyoumei.cn/gtbfzraoud.html

[S28] C：静态变量
来源：http://hz.cashguo.top/gtwtpfarvc.html

static int counter = 0;
来源：http://hz.nanxinkj.top/gtuzodcdvp.html

[S29] C：变参函数
来源：http://hz.jyoumei.cn/gtkhqksxxm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.fzhhl.top/gtaipecsvo.html

[S30] C：头文件保护
来源：http://hz.xuanzx.com/gtzzfztnto.html

#ifndef X_H
来源：http://hz.xinyue.icu/gtawfwnruy.html

#define X_H
来源：http://hz.chenlongwang.top/gtggdpegky.html

#endif
来源：http://hz.zycfv.cn/gtqzrfqbfh.html

[S31] C++：Hello World
来源：http://hz.quarkkingdee.top/gtpogeivhe.html

#include <iostream>
来源：http://hz.zycfv.cn/gtiueqvxyy.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yonumen.top/gteveyjfub.html

[S32] C++：字符串
来源：http://hz.ywan-chungtsiang.top/gtqsqijbfb.html

std::string s = "hi";  s += "!";
来源：http://hz.shuidangran.top/gtxvmuhitv.html

[S33] C++：vector 增删
来源：http://hz.yuanzhike.top/gtxmmpdrtu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jqgufenzy.top/gtfvenvzjm.html

[S34] C++：遍历 vector
来源：http://hz.jinghuilouyu.cn/gtbcddsxet.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yongpay.top/gtmgsesssp.html

[S35] C++：map
来源：http://hz.nwbrower.top/gtcpkdjptf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.quarkkingdee.top/gtymqhayem.html

[S36] C++：unordered_map
来源：http://hz.svipenyu.cn/gtwqsoabhi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.52xcode.cn/gtelfuygxj.html

[S37] C++：set
来源：http://hz.jqgufenzy.top/gtgwktplpu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jinqigfzy.top/gtxqexceds.html

[S38] C++：排序
来源：http://hz.gaohongyu789.top/gtqxvkjril.html

std::sort(v.begin(), v.end());
来源：http://hz.chenlongwang.top/gtirfwxwup.html

[S39] C++：自定义比较器排序
来源：http://hz.bjfxy.top/gtfhqbfifq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.sysykeji.top/gtudswvcfi.html

[S40] C++：查找元素
来源：http://hz.c1oappe.top/gtsoqvntey.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hywenlv.cn/gtzrmpialk.html

[S41] C++：类与构造函数
来源：http://hz.nanxinkj.top/gtvhlbqqlf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hammf.cn/gtvisejadx.html

[S42] C++：继承与虚函数
来源：http://hz.zhaomingkeji.xyz/gtztmazvyz.html

class B : public Base { public: void f() override {} };
来源：http://hz.gzhubu.top/gtsxfxdhcy.html

[S43] C++：智能指针
来源：http://hz.ybcxt.top/gtumkblrmz.html

auto p = std::make_unique<int>(5);
来源：http://hz.cheryme.top/gteqkghccj.html

[S44] C++：引用传参
来源：http://hz.zhiwuduotai.top/gtmycotbnl.html

void inc(int &x) { ++x; }
来源：http://hz.tian-w.cn/gtfhuvomks.html

[S45] C++：lambda
来源：http://hz.smart0.xyz/gtrstygskq.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xingfuxueyuan.xyz/gtyiewhocb.html

[S46] C++：函数模板
来源：http://hz.bjfxy.top/gtmapxyost.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yj20258888.top/gtcbexavnb.html

[S47] C++：结构化绑定遍历
来源：http://hz.hnqzz.top/gtpdpozdav.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.nanxuanxn.top/gtpgbmyzph.html

[S48] C++：逐行读文件
来源：http://hz.kuanghao11.cn/gtkgfdpzmi.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.ydzc1.top/gtrrfbmsvb.html

while (std::getline(in, line)) { }
来源：http://hz.jqgufenzy.top/gtnucvaluk.html

[S49] C++：写文件
来源：http://hz.chenjidiqi.icu/gttkcxfmbe.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.cdnleiting.top/gtqrpotmqq.html

[S50] C++：格式化数字
来源：http://hz.mhx1999.top/gtszojlycq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yj20258.top/gtjizisgua.html

[S51] C++：显式类型转换
来源：http://hz.yj202588.top/gtjmybqqsq.html

static_cast<double>(a) / b
来源：http://hz.aizwys.cn/gteduypprt.html

[S52] C++：const 与 noexcept
来源：http://hz.zhiwuduotai.top/gtwztgpvnh.html

int size() const noexcept { return n_; }
来源：http://hz.nwbrower.top/gtuezflkxc.html

[S53] C++：移动语义
来源：http://hz.zdqjudy.top/gtlfiidfum.html

std::vector<int> w = std::move(v);
来源：http://hz.nwbrower.top/gtrzkmxdrx.html

[S54] C++：异常处理
来源：http://hz.hongshengwenyu.top/gtftlsqaxg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.nanxinkj.top/gtsnzqceua.html

[S55] C++：结构化绑定
来源：http://hz.316326.xyz/gtdqvzczlk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.sysykeji.top/gtmimijcyx.html

[S56] C++：optional
来源：http://hz.jqgfzy.top/gtnvbpaoqw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yuanzhike.top/gtmtgjyuyy.html

[S57] C++：编译期常量
来源：http://hz.birdmap.top/gtprxrllqe.html

constexpr int N = 10;
来源：http://hz.wangdashe.top/gtfehbbiiy.html

[S58] C++：命名空间
来源：http://hz.tianlin.xyz/gtlrlyrmum.html

namespace ns { int f() { return 1; } }
来源：http://hz.jinqigufen.top/gtwuscmuzl.html

[S59] C++：静态断言
来源：http://hz.shangyingyoupin.top/gtwvmfdikx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xylfe.cn/gtgfmzuthy.html

[S60] C++：遍历并删除元素
来源：http://hz.sufxvd.cn/gtjllfchbr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.aizwys.cn/gtshufqflz.html

================================================================================
来源：http://hz.andypj.xyz/gtyyhwxdab.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shanyushiyangkeji.top/gtlyrzkulm.html

================================================================================
来源：http://hz.daria6918.cn/gtpldazoqj.html

[T01] Kotlin：Hello World
来源：http://hz.zhoulong.xyz/gtrpusljel.html

println("Hello")
来源：http://hz.feifeiyinyue.top/gtmlhabbla.html

[T02] Kotlin：变量
来源：http://hz.zhijiandao.cn/gtjeauxvcg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.9152youxi.cn/gtmmlnrziz.html

[T03] Kotlin：字符串模板
来源：http://hz.dashuyun.cn/gtdtkzmlzz.html

"值: $b"
来源：http://hz.jinqigufen.top/gtfkdrvlod.html

[T04] Kotlin：空安全
来源：http://hz.0kj1m.cn/gtpsknozpy.html

val n: String? = null;  n?.length
来源：http://hz.fengsongda.top/gtzefdjjuf.html

[T05] Kotlin：when 表达式
来源：http://hz.jinghuilouyu.cn/gtwehflwbl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.wangshuangyany.cn/gtjoqwlube.html

[T06] Kotlin：集合映射
来源：http://hz.shangyingyoupin.top/gtndyateyn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.pycfn.com/gtsgfqicic.html

[T07] Kotlin：集合过滤
来源：http://hz.9152youxi.cn/gtqfgqyjqw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.sysykeji.top/gtecnlbmzl.html

[T08] Kotlin：数据类
来源：http://hz.fzhhl.top/gthnecsiog.html

data class User(val name: String, val age: Int)
来源：http://hz.vqdsnc.cn/gtlnxpvixe.html

[T09] Kotlin：扩展函数
来源：http://hz.chenjidiqi.icu/gtjlubodaq.html

fun String.exclaim() = this + "!"
来源：http://hz.pengpengdd.cyou/gtvbmztzki.html

[T10] Kotlin：默认参数
来源：http://hz.yj202588.top/gtqeiuhavy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.snrcjt.cn/gttszxykih.html

[T11] Kotlin：协程
来源：http://hz.svipenyu.cn/gtgbdnlipq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yj20258.top/gtyeldnfkr.html

[T12] Kotlin：解构声明
来源：http://hz.c1oappe.top/gtpygxycye.html

val (a, b) = Pair(1, 2)
来源：http://hz.zycfv.cn/gtfxifluwy.html

[T13] Kotlin：只读 Map
来源：http://hz.jqgfzy.top/gtqumuyhtb.html

val m = mapOf("a" to 1)
来源：http://hz.wangshuangyany.cn/gtpvecnpce.html

[T14] Kotlin：循环
来源：http://hz.yonumen.top/gtrezzuhgm.html

for (i in 1..10) println(i)
来源：http://hz.bjfxy.top/gtgueskyll.html

[T15] Kotlin：接口
来源：http://hz.nwbrower.top/gtofftfmdd.html

interface Shape { fun area(): Double }
来源：http://hz.yuxming.cn/gtruloulwe.html

[T16] Swift：Hello World
来源：http://hz.daria6918.cn/gtfpnvnuiv.html

print("Hello")
来源：http://hz.yj20258888.top/gtopuijtts.html

[T17] Swift：变量与常量
来源：http://hz.hammf.cn/gtprpfgwfy.html

var a = 1;  let b = 2
来源：http://hz.xziqi.cn/gtqqquncna.html

[T18] Swift：字符串插值
来源：http://hz.shangyingyoupin.top/gtmhpdqald.html

"值: \(b)"
来源：http://hz.fzhhl.top/gtbzcygmib.html

[T19] Swift：可选绑定
来源：http://hz.mhx1999.top/gtwkgcblyn.html

if let n = opt { print(n) }
来源：http://hz.yj20258888.top/gtwbjkmyra.html

[T20] Swift：数组操作
来源：http://hz.tanke756.top/gtvmknmmhz.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zdqjudy.top/gtmnfjcsle.html

[T21] Swift：遍历
来源：http://hz.chenjidiqi.icu/gtebzvuzbk.html

for x in a { print(x) }
来源：http://hz.kuanghao11.cn/gtihlemsgu.html

[T22] Swift：字典
来源：http://hz.jlsjyb.cn/gtxluhhjmy.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zhaomingkeji.xyz/gtfofjujap.html

[T23] Swift：函数
来源：http://hz.ydzc1.top/gtwruwyvsc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.tian-w.cn/gtckrnakjs.html

[T24] Swift：闭包
来源：http://hz.ydzc1.top/gtubkpukna.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhijiandao.cn/gthnovrwwt.html

[T25] Swift：结构体
来源：http://hz.redwolf501.top/gtxulqrihw.html

struct P { var x: Int }
来源：http://hz.shangyingyoupin.top/gtaxtliiho.html

[T26] Swift：类与重写
来源：http://hz.bjfxy.top/gtsvxxfeiy.html

class A: Base { override func f() {} }
来源：http://hz.cdnleiting.top/gtzpdautyc.html

[T27] Swift：错误处理
来源：http://hz.vqdsnc.cn/gtacyizlao.html

do { try f() } catch { print(error) }
来源：http://hz.9152youxi.cn/gtdqxhpsho.html

[T28] Swift：枚举
来源：http://hz.gogol.net.cn/gtiiquleiz.html

enum Color { case red, green }
来源：http://hz.9152youxi.cn/gtfpnjvpkg.html

[T29] Swift：guard 提前返回
来源：http://hz.redwolf501.top/gtykpwpvjh.html

guard let x = opt else { return }
来源：http://hz.pycfn.com/gtxmpytbwa.html

[T30] Swift：协议
来源：http://hz.zhongyouzk.top/gtmqxqgdhf.html

protocol Shape { func area() -> Double }
来源：http://hz.jyoumei.cn/gtotkhbzkp.html

[T31] Lua：Hello World
来源：http://hz.snrcjt.cn/gtdbwhuvfc.html

print("Hello")
来源：http://hz.yuxming.cn/gtiqcmzczt.html

[T32] Lua：局部变量
来源：http://hz.xuetiantiany.cn/gtbnoteysd.html

local a = 1
来源：http://hz.snrcjt.cn/gtmwmtcvzu.html

[T33] Lua：表（数组）
来源：http://hz.jlsjyb.cn/gtocwrwmge.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.nanxuanxn.top/gtxguplxip.html

[T34] Lua：遍历表
来源：http://hz.pycfn.com/gtptabqvyz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.ybcxt.top/gtvjyxklem.html

[T35] Lua：字典表
来源：http://hz.tianlin.xyz/gtokjzoelh.html

local d = { a = 1 };  d.b = 2
来源：http://hz.c1oappe.top/gtsfrtxabc.html

[T36] Lua：函数
来源：http://hz.ydzc1.top/gtvfcfibap.html

function add(a, b) return a + b end
来源：http://hz.nwbrower.top/gtgqunxylt.html

[T37] Lua：字符串拼接
来源：http://hz.zycfv.cn/gthhvtyaai.html

"a" .. "b"
来源：http://hz.birdmap.top/gtnprcjtqs.html

[T38] Lua：条件
来源：http://hz.zhaomingkeji.xyz/gtpahierzl.html

if x > 0 then print("正") end
来源：http://hz.ehwqpu.com/gtedytmejr.html

[T39] Lua：模式匹配
来源：http://hz.9152youxi.cn/gteehpgtbt.html

string.find(s, "%d+")
来源：http://hz.zhiwuduotai.top/gtidtugdvz.html

[T40] Lua：元表
来源：http://hz.jinqigufen.top/gtfsfzuwtj.html

setmetatable({}, { __index = base })
来源：http://hz.ydjk.org.cn/gtlfktclmd.html

[T41] Perl：Hello World
来源：http://hz.snrcjt.cn/gtebdkwvxf.html

print "Hello\n";
来源：http://hz.nwbrower.top/gtfcmcvhge.html

[T42] Perl：变量类型
来源：http://hz.pycfn.com/gtbvcorbvh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.hfpthk.cn/gtyvcbplzo.html

[T43] Perl：字符串插值
来源：http://hz.ywan-chungtsiang.top/gtlewivuaz.html

"值: $a"
来源：http://hz.wangshuangyany.cn/gtbzozydyn.html

[T44] Perl：条件
来源：http://hz.andypj.xyz/gtjjsopdpf.html

if ($a > 0) { print "正"; }
来源：http://hz.yanxiufei.cn/gtrabmdmfb.html

[T45] Perl：数组遍历
来源：http://hz.zdqjudy.top/gtfvbzrmdk.html

for my $x (@arr) { print $x; }
来源：http://hz.shanyushiyangkeji.top/gtxcvbvhwh.html

[T46] Perl：哈希操作
来源：http://hz.zhoulong.xyz/gtbnypujko.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.c1oappe.top/gtefepnxwg.html

[T47] Perl：正则捕获
来源：http://hz.zdqjudy.top/gtzgfqmszj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.daxiang520.top/gtwgzenycv.html

[T48] Perl：正则替换
来源：http://hz.xingfuxueyuan.xyz/gtsslisefq.html

$s =~ s/old/new/g;
来源：http://hz.jqgfzy.top/gtkydwanae.html

[T49] Perl：函数
来源：http://hz.tianlin.xyz/gtximyeoxg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.hnxiangtu.top/gtfjslfpdo.html

[T50] Perl：逐行读文件
来源：http://hz.havefunace.top/gtwlvvoldu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jianghu66.top/gtasqjwrpl.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.ppjwa.cn/gtrxduyyxw.html

[T51] Scala：Hello World
来源：http://hz.cdnleiting.top/gtjzjhsqej.html

println("Hello")
来源：http://hz.wangdashe.top/gtpyzxoyhe.html

[T52] Scala：变量
来源：http://hz.hnqzz.top/gttzofopra.html

val a = 1;  var b = 2
来源：http://hz.zhiwuduotai.top/gtjsboxqth.html

[T53] Scala：字符串插值
来源：http://hz.zycfv.cn/gtzwhescgd.html

s"值: $b"
来源：http://hz.52xcode.cn/gtxnyvuqqz.html

[T54] Scala：集合映射
来源：http://hz.chenzaomai.com/gtfofpljpa.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.guowangkeji.top/gtoziwugav.html

[T55] Scala：集合过滤
来源：http://hz.zhixingplan.top/gtrufiqysz.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.cucudq.cn/gthrhshoug.html

[T56] Scala：样例类
来源：http://hz.yanxiufei.cn/gtgvpoqcbe.html

case class User(name: String, age: Int)
来源：http://hz.zhengqikj.top/gtxxjvljtv.html

[T57] Scala：模式匹配
来源：http://hz.andypj.xyz/gttlwyhwfu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.jlsjyb.cn/gtknimwskc.html

[T58] Scala：函数定义
来源：http://hz.cashguo.top/gtomplnpvl.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.dianchejie.cn/gtzhjyrkae.html

[T59] Scala：循环
来源：http://hz.cheryme.top/gtadnbkogh.html

for (i <- 1 to 10) println(i)
来源：http://hz.yuanzhike.top/gtvhdpcdst.html

[T60] Scala：折叠
来源：http://hz.9152youxi.cn/gtvdwiodus.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.aibaodan.cn/gtjmcgzken.html

================================================================================
来源：http://hz.guowangkeji.top/gtltbuetof.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.aizwys.cn/gtllwvvndo.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtcrtbvpnb.html

[U01] Py：创建虚拟环境
来源：http://hz.ehwqpu.com/gtkghngjdx.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.jinghuilouyu.cn/gtzcsohzun.html

[U02] Py：导出 / 安装依赖
来源：http://hz.snrcjt.cn/gtsnizyrfl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.vqdsnc.cn/gtdcdjcmnm.html

[U03] Py：加载 .env 配置
来源：http://hz.yonumen.top/gtnhwgomjx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yj20258888.top/gtdvbauium.html

[U04] Py：变量调试打印
来源：http://hz.daxiang520.top/gtbolorvij.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jiagoushi.top/gtmhjfprgc.html

[U05] Py：列表去重且保序
来源：http://hz.yj20258.top/gtjjkybhvm.html

list(dict.fromkeys(arr))
来源：http://hz.jiagoushi.top/gtyijuclox.html

[U06] Py：合并两个字典
来源：http://hz.guowangkeji.top/gtsskyczgx.html

{**a, **b}
来源：http://hz.cucudq.cn/gtonmoaegi.html

[U07] Py：反转字典键值
来源：http://hz.jinqigfzy.top/gteosdfxkh.html

{v: k for k, v in d.items()}
来源：http://hz.gogol.net.cn/gtbgarkfmt.html

[U08] Py：展平二维列表
来源：http://hz.yuanzhike.top/gtotvoqqhz.html

[y for x in nested for y in x]
来源：http://hz.yuanzhike.top/gtpelctqzs.html

[U09] Py：字典取最大值的键
来源：http://hz.gzhubu.top/gtlxxxuold.html

max(d, key=d.get)
来源：http://hz.daria6918.cn/gtlpvgyggi.html

[U10] Py：按值排序字典
来源：http://hz.zdqjudy.top/gtiibjoiwv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.hnqzz.top/gtxjcdwtrh.html

[U11] Py：生成器表达式
来源：http://hz.xuetiantiany.cn/gthtvmigcq.html

(x * 2 for x in arr)
来源：http://hz.meibo888.top/gtezwjwtwr.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.cheryme.top/gtdkirmpde.html

Counter(arr).most_common(3)
来源：http://hz.ydjk.org.cn/gtbzgquvro.html

[U13] Py：固定长度队列
来源：http://hz.haohaochexian.top/gtnvmxpaqf.html

deque(maxlen=10)
来源：http://hz.iojbl.cn/gtciblrnih.html

[U14] Py：分组收集到列表
来源：http://hz.yj202588.top/gtcicrjarq.html

defaultdict(list)
来源：http://hz.svipenyu.cn/gtulmzbyiq.html

[U15] Py：高精度计时
来源：http://hz.jinqigufen.top/gtohqjoylg.html

t = time.perf_counter()
来源：http://hz.cqqwz.cn/gthjtqxedp.html

[U16] Py：命令行参数解析
来源：http://hz.yangfankeji.com/gtrsgfzyef.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.vqdsnc.cn/gtwvtyhjzd.html

[U17] Py：初始化日志
来源：http://hz.ydjk.org.cn/gtdvgosvyk.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.jianghu66.top/gtykwlgevy.html

[U18] Py：预编译正则
来源：http://hz.chenlongwang.top/gthibbbgpn.html

pat = re.compile(r"\d+")
来源：http://hz.hnqzz.top/gtfqmnltsg.html

[U19] Py：正则替换带回调
来源：http://hz.hnxiangtu.top/gtwsjsrcmn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.ehwqpu.com/gtkpofntnw.html

[U20] Py：缓存函数结果
来源：http://hz.zhongyouzk.top/gthpgzngmk.html

@functools.lru_cache(maxsize=None)
来源：http://hz.havefunace.top/gtvuqwqsag.html

[U21] Py：自定义上下文管理器
来源：http://hz.xylfe.cn/gtkvfwtkau.html

@contextlib.contextmanager
来源：http://hz.snrcjt.cn/gtxkzwipsm.html

[U22] Py：矩阵转置
来源：http://hz.ywan-chungtsiang.top/gtfgupmaoa.html

list(zip(*m))
来源：http://hz.snrcjt.cn/gtydcvydso.html

[U23] Py：分块读取大文件
来源：http://hz.52xcode.cn/gtstcnorjs.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.shuidangran.top/gttmxsoiin.html

[U24] Py：路径操作
来源：http://hz.cheryme.top/gtxqexgnih.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.hnqzz.top/gtejavbgza.html

[U25] Py：CSV 按字典读
来源：http://hz.mhx1999.top/gtsblqgnyf.html

csv.DictReader(f)
来源：http://hz.feifeiyinyue.top/gtcezdehhp.html

[U26] Py：并发下载
来源：http://hz.ppjwa.cn/gtxquzlqqs.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.xingfuxueyuan.xyz/gtjsgdrice.html

[U27] Py：异步 HTTP
来源：http://hz.wangdashe.top/gtdrzcjjqp.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.jinyuanbaomall.cn/gtflniggil.html

[U28] Py：类型别名
来源：http://hz.ivvv.top/gtkllthtsn.html

UserId = int
来源：http://hz.sysykeji.top/gtgzcbjari.html

[U29] Py：属性校验
来源：http://hz.gotoacloud.top/gtfexsbrec.html

@property 与 @x.setter 配合
来源：http://hz.shzxlz.cn/gtvhwtzfxt.html

[U30] Py：数据类
来源：http://hz.ydjk.org.cn/gtigvmycbr.html

@dataclass(slots=True)
来源：http://hz.yj20258888.top/gtimxaxuxf.html


<!-- 参考信息 -->