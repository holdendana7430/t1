代发 wailian999

strlen(s)
来源：http://hz.havefunace.top/gtrpvktwrx.html

[S06] C：字符串比较
来源：http://hz.tanke756.top/gtzqkosutn.html

strcmp(a, b) == 0
来源：http://hz.zhixingplan.top/gtahedysec.html

[S07] C：数组遍历求和
来源：http://hz.jiagoushi.top/gtfphsixpw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jinyuanbaomall.cn/gteuydrtlr.html

[S08] C：动态内存分配与释放
来源：http://hz.wangshuangyany.cn/gtntsxztfc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.dianchejie.cn/gteoeyywwu.html

[S09] C：结构体定义与初始化
来源：http://hz.tanke756.top/gtosolnklz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.shanyushiyangkeji.top/gtnldfpwia.html

[S10] C：指针与解引用
来源：http://hz.zhoulong.xyz/gtnmktaemm.html

int *p = &a;  *p = 5;
来源：http://hz.zhengqikj.top/gtezslqbne.html

[S11] C：逐行读文件
来源：http://hz.nanxinkj.top/gtfaqxlsdd.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.hnxiangtu.top/gtqqpxtezy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.andypj.xyz/gtrreusynr.html

fclose(f);
来源：http://hz.hywenlv.cn/gtlzlfjwat.html

[S12] C：写文件
来源：http://hz.daria6918.cn/gtbsphmfug.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ivvv.top/gtkvoqnpkq.html

[S13] C：宏定义
来源：http://hz.zhengqikj.top/gtjdcdjbbg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ydjk.org.cn/gtnlxehtdg.html

[S14] C：枚举
来源：http://hz.zhijiandao.cn/gtriolvwin.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhixingplan.top/gtcgwevazv.html

[S15] C：类型转换
来源：http://hz.tian-w.cn/gtvpzzkpvh.html

(double) a / b
来源：http://hz.chenzaomai.com/gtbgzpgwba.html

[S16] C：位操作置位
来源：http://hz.zhengqikj.top/gtuysyofqk.html

x |= (1 << 3);
来源：http://hz.hnxiangtu.top/gtxoemeskv.html

[S17] C：安全拼接字符串
来源：http://hz.bjfxy.top/gtxaswgufj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.iojbl.cn/gtposwsovv.html

[S18] C：命令行参数
来源：http://hz.havefunace.top/gtxqumoxcs.html

int main(int argc, char **argv)
来源：http://hz.hongshengwenyu.top/gtxnhqfqjq.html

[S19] C：快速排序
来源：http://hz.pengpengdd.cyou/gtjedkfcxm.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jqgufenzy.top/gtwuqylxrl.html

[S20] C：二分查找
来源：http://hz.svipenyu.cn/gtjvjxlfbr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ybcxt.top/gtyeowbkfa.html

[S21] C：字符类别判断
来源：http://hz.xinyue.icu/gterusfoqk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hfpthk.cn/gtfqoewzmd.html

[S22] C：字符串转数字
来源：http://hz.hongshengwenyu.top/gtcpzuuczm.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.wangdashe.top/gtqnkgkkjn.html

[S23] C：随机数
来源：http://hz.birdmap.top/gtpbidugfe.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.vqdsnc.cn/gtvubhoyzs.html

[S24] C：获取本地时间
来源：http://hz.dianchejie.cn/gtbiicmhba.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yj20258.top/gtcumucvdq.html

[S25] C：内存拷贝
来源：http://hz.jqgfzy.top/gthpbhcwnb.html

memcpy(dst, src, n);
来源：http://hz.zhoulong.xyz/gtayvewghe.html

[S26] C：内存清零
来源：http://hz.yangfankeji.com/gtjaglfcdo.html

memset(a, 0, sizeof a);
来源：http://hz.yanxiufei.cn/gtaitsbiwa.html

[S27] C：定义常量
来源：http://hz.feifeiyinyue.top/gtfbuxaevi.html

const double PI = 3.14159;
来源：http://hz.xinyue.icu/gttumfriti.html

[S28] C：静态变量
来源：http://hz.fengsongda.top/gtrljggbts.html

static int counter = 0;
来源：http://hz.chenlongwang.top/gtriyxbznj.html

[S29] C：变参函数
来源：http://hz.quarkkingdee.top/gttqsdhbys.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.shuidangran.top/gturblkciz.html

[S30] C：头文件保护
来源：http://hz.pengpengdd.cyou/gttcavhoho.html

#ifndef X_H
来源：http://hz.redwolf501.top/gtjifsxgby.html

#define X_H
来源：http://hz.hnqzz.top/gtiuddabft.html

#endif
来源：http://hz.yangfankeji.com/gtrsrfrfiw.html

[S31] C++：Hello World
来源：http://hz.kuanghao11.cn/gtuimqqkna.html

#include <iostream>
来源：http://hz.jianghu66.top/gtbfrvnuhc.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jianghu66.top/gtlxazaefg.html

[S32] C++：字符串
来源：http://hz.mhx1999.top/gtyrnuzezc.html

std::string s = "hi";  s += "!";
来源：http://hz.yongpay.top/gtjalbbigc.html

[S33] C++：vector 增删
来源：http://hz.hammf.cn/gtxjbyxrve.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.sufxvd.cn/gtekjbkrug.html

[S34] C++：遍历 vector
来源：http://hz.jinqigfzy.top/gthirvnixe.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.bjfxy.top/gtlmqlxnqu.html

[S35] C++：map
来源：http://hz.xziqi.cn/gtsaofrdcx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.chenzaomai.com/gtpzvabzei.html

[S36] C++：unordered_map
来源：http://hz.andypj.xyz/gtcskruwxf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhixingplan.top/gtyojuhlps.html

[S37] C++：set
来源：http://hz.shanyushiyangtech.top/gtjnyhwbrf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhaomingkeji.xyz/gtirewqszv.html

[S38] C++：排序
来源：http://hz.xuetiantiany.cn/gtyevsuuet.html

std::sort(v.begin(), v.end());
来源：http://hz.xingfuxueyuan.xyz/gtcqktjtsp.html

[S39] C++：自定义比较器排序
来源：http://hz.yuanzhike.top/gtmjvxvxqe.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ydzc1.top/gtorqqvmyy.html

[S40] C++：查找元素
来源：http://hz.aizwys.cn/gtmlywwkci.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yangfankeji.com/gtqwgofzav.html

[S41] C++：类与构造函数
来源：http://hz.meibo888.top/gtfgfuzuvw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jinqigufen.top/gtchdythrn.html

[S42] C++：继承与虚函数
来源：http://hz.kuanghao11.cn/gtgwwjrmyl.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhixingplan.top/gtncpepiju.html

[S43] C++：智能指针
来源：http://hz.ybcxt.top/gtxwmasmou.html

auto p = std::make_unique<int>(5);
来源：http://hz.9152youxi.cn/gtkrtzscdc.html

[S44] C++：引用传参
来源：http://hz.yj20258888.top/gtbniupcoe.html

void inc(int &x) { ++x; }
来源：http://hz.chenjidiqi.icu/gttkvvyqwn.html

[S45] C++：lambda
来源：http://hz.wangshuangyany.cn/gtodwmjeae.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.316326.xyz/gttprdoijn.html

[S46] C++：函数模板
来源：http://hz.jyoumei.cn/gtwsgnwugm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jinyuanbaomall.cn/gtaggmkjvy.html

[S47] C++：结构化绑定遍历
来源：http://hz.havefunace.top/gtuuhqcefe.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.xinyue.icu/gtfaadtivp.html

[S48] C++：逐行读文件
来源：http://hz.c1oappe.top/gtxnphufri.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.hysaishi.cn/gtsdsyqqwz.html

while (std::getline(in, line)) { }
来源：http://hz.havefunace.top/gtpnlxgkbt.html

[S49] C++：写文件
来源：http://hz.ehwqpu.com/gtrpeukkxz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.vqdsnc.cn/gtnnyvdkmh.html

[S50] C++：格式化数字
来源：http://hz.quarkkingdee.top/gthutkvvgu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jqgfzy.top/gtxurzgrdg.html

[S51] C++：显式类型转换
来源：http://hz.nanxinkj.top/gtfxuypxtj.html

static_cast<double>(a) / b
来源：http://hz.ydzc1.top/gtnkyqrusb.html

[S52] C++：const 与 noexcept
来源：http://hz.hfpthk.cn/gteqsdfxmj.html

int size() const noexcept { return n_; }
来源：http://hz.jinqigufen.top/gtdnomorde.html

[S53] C++：移动语义
来源：http://hz.gogol.net.cn/gtakxbdbqz.html

std::vector<int> w = std::move(v);
来源：http://hz.aizwys.cn/gtdgbyislr.html

[S54] C++：异常处理
来源：http://hz.gaohongyu789.top/gttoxotkot.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.andypj.xyz/gtzzsymwnz.html

[S55] C++：结构化绑定
来源：http://hz.wangdashe.top/gtolciqwpr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.ivvv.top/gtrczzusbj.html

[S56] C++：optional
来源：http://hz.xuetiantiany.cn/gtqkbntdpv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yj202588.top/gtkstkkeca.html

[S57] C++：编译期常量
来源：http://hz.sxryk.cn/gtcboexcwv.html

constexpr int N = 10;
来源：http://hz.jianghu66.top/gtaxclluvj.html

[S58] C++：命名空间
来源：http://hz.jinghuilouyu.cn/gtrjujglpe.html

namespace ns { int f() { return 1; } }
来源：http://hz.daria6918.cn/gtdbptowiz.html

[S59] C++：静态断言
来源：http://hz.bjfxy.top/gtckouzzeg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.cashguo.top/gtzikykclz.html

[S60] C++：遍历并删除元素
来源：http://hz.sweek.top/gtmbfmnsfe.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.cashguo.top/gtigwxwjtl.html

================================================================================
来源：http://hz.ydzc1.top/gtczroggdf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.pycfn.com/gtluocptzo.html

================================================================================
来源：http://hz.ybcxt.top/gtcqwcgify.html

[T01] Kotlin：Hello World
来源：http://hz.yj20258.top/gtrybxfzxe.html

println("Hello")
来源：http://hz.shanyushiyangkeji.top/gtdbuyoyqf.html

[T02] Kotlin：变量
来源：http://hz.wangdashe.top/gthhfekyhc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhaomingkeji.xyz/gtuhemvgkb.html

[T03] Kotlin：字符串模板
来源：http://hz.hfpthk.cn/gtrdrcjvrp.html

"值: $b"
来源：http://hz.cqqwz.cn/gtdtqhjtkk.html

[T04] Kotlin：空安全
来源：http://hz.hongshengwenyu.top/gtzehthxhz.html

val n: String? = null;  n?.length
来源：http://hz.mhx1999.top/gthyyaobdy.html

[T05] Kotlin：when 表达式
来源：http://hz.shanyushiyangkeji.top/gtkktaltix.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.tian-w.cn/gtngmqemro.html

[T06] Kotlin：集合映射
来源：http://hz.xylfe.cn/gtwnugfnud.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.dashuyun.cn/gtwpeoyvtg.html

[T07] Kotlin：集合过滤
来源：http://hz.ehwqpu.com/gtvuqhrcrw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.ydjk.org.cn/gtiqxirlfc.html

[T08] Kotlin：数据类
来源：http://hz.daxiang520.top/gtagcabznr.html

data class User(val name: String, val age: Int)
来源：http://hz.tanke756.top/gtzgbhfizy.html

[T09] Kotlin：扩展函数
来源：http://hz.yongpay.top/gtceoybmai.html

fun String.exclaim() = this + "!"
来源：http://hz.gotoacloud.top/gtefubfmmc.html

[T10] Kotlin：默认参数
来源：http://hz.ywan-chungtsiang.top/gtfxpahmea.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ehwqpu.com/gtltnmppqm.html

[T11] Kotlin：协程
来源：http://hz.nanxinkj.top/gtzbuivwtt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.sxryk.cn/gtcmrzdmdd.html

[T12] Kotlin：解构声明
来源：http://hz.cashguo.top/gtbsxgipbq.html

val (a, b) = Pair(1, 2)
来源：http://hz.zycfv.cn/gtpbzcsmps.html

[T13] Kotlin：只读 Map
来源：http://hz.sysykeji.top/gtgpnmbapi.html

val m = mapOf("a" to 1)
来源：http://hz.sxryk.cn/gtdesgaeji.html

[T14] Kotlin：循环
来源：http://hz.nanxinkj.top/gtikjalbug.html

for (i in 1..10) println(i)
来源：http://hz.ehwqpu.com/gtrftkgtxp.html

[T15] Kotlin：接口
来源：http://hz.vqdsnc.cn/gtqpkrmuds.html

interface Shape { fun area(): Double }
来源：http://hz.tanke756.top/gtcvlquddx.html

[T16] Swift：Hello World
来源：http://hz.52xcode.cn/gtziriyhll.html

print("Hello")
来源：http://hz.snrcjt.cn/gthefaoify.html

[T17] Swift：变量与常量
来源：http://hz.hfpthk.cn/gtvtluhrij.html

var a = 1;  let b = 2
来源：http://hz.sweek.top/gtcshopiib.html

[T18] Swift：字符串插值
来源：http://hz.andypj.xyz/gtcodgncns.html

"值: \(b)"
来源：http://hz.cucudq.cn/gtuevcrfmu.html

[T19] Swift：可选绑定
来源：http://hz.jianghu66.top/gtqgqrohqj.html

if let n = opt { print(n) }
来源：http://hz.zycfv.cn/gtfnfzdoco.html

[T20] Swift：数组操作
来源：http://hz.zhongyouzk.top/gtkqdpubhy.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.tanke756.top/gtkffvbvku.html

[T21] Swift：遍历
来源：http://hz.svipenyu.cn/gtsdqyjzth.html

for x in a { print(x) }
来源：http://hz.hnqzz.top/gtlbssnpzf.html

[T22] Swift：字典
来源：http://hz.tian-w.cn/gtszghcpgj.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jqgufenzy.top/gtwtogfqxd.html

[T23] Swift：函数
来源：http://hz.fengsongda.top/gtqkobodzr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zycfv.cn/gtusbfyvwx.html

[T24] Swift：闭包
来源：http://hz.guowangkeji.top/gtyyobkvbg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jlsjyb.cn/gtzgwmcmqc.html

[T25] Swift：结构体
来源：http://hz.yj20258.top/gtxyrpuill.html

struct P { var x: Int }
来源：http://hz.vqdsnc.cn/gtyagbmccm.html

[T26] Swift：类与重写
来源：http://hz.zycfv.cn/gteqjbthdn.html

class A: Base { override func f() {} }
来源：http://hz.hywenlv.cn/gtgmqqhpxw.html

[T27] Swift：错误处理
来源：http://hz.jyoumei.cn/gtcqgaoovd.html

do { try f() } catch { print(error) }
来源：http://hz.chenjidiqi.icu/gttruwkuvx.html

[T28] Swift：枚举
来源：http://hz.shanyushiyangtech.top/gtxifeltdi.html

enum Color { case red, green }
来源：http://hz.aizwys.cn/gtxuhjdocg.html

[T29] Swift：guard 提前返回
来源：http://hz.gotoacloud.top/gtbrbineds.html

guard let x = opt else { return }
来源：http://hz.shanyushiyangkeji.top/gttddmdadu.html

[T30] Swift：协议
来源：http://hz.yanxiufei.cn/gtlocgatbm.html

protocol Shape { func area() -> Double }
来源：http://hz.gzhubu.top/gtxvpinxse.html

[T31] Lua：Hello World
来源：http://hz.nanxuanxn.top/gtgwjddgsv.html

print("Hello")
来源：http://hz.pycfn.com/gtrljpbyjw.html

[T32] Lua：局部变量
来源：http://hz.xingfuxueyuan.xyz/gtoqwvgqoo.html

local a = 1
来源：http://hz.nanxinkj.top/gtwbcpiori.html

[T33] Lua：表（数组）
来源：http://hz.shuidangran.top/gtmcsazfhj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.ydjk.org.cn/gtzxgswidz.html

[T34] Lua：遍历表
来源：http://hz.birdmap.top/gtuqgptldk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.xuanzx.com/gtgijssnox.html

[T35] Lua：字典表
来源：http://hz.ivvv.top/gtwucrifxy.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yongpay.top/gtudymmocl.html

[T36] Lua：函数
来源：http://hz.sufxvd.cn/gtegfnqjxq.html

function add(a, b) return a + b end
来源：http://hz.smart0.xyz/gtyyxgxjcf.html

[T37] Lua：字符串拼接
来源：http://hz.havefunace.top/gtetqhagto.html

"a" .. "b"
来源：http://hz.bjfxy.top/gtocdfszln.html

[T38] Lua：条件
来源：http://hz.aibaodan.cn/gtddyjgjza.html

if x > 0 then print("正") end
来源：http://hz.zycfv.cn/gtyumkqdnk.html

[T39] Lua：模式匹配
来源：http://hz.wangshuangyany.cn/gtyuwxdfbt.html

string.find(s, "%d+")
来源：http://hz.yuxming.cn/gtgymqygdl.html

[T40] Lua：元表
来源：http://hz.guowangkeji.top/gtxqinafyk.html

setmetatable({}, { __index = base })
来源：http://hz.xuetiantiany.cn/gtyiqnqdaz.html

[T41] Perl：Hello World
来源：http://hz.pycfn.com/gtzbwzonvj.html

print "Hello\n";
来源：http://hz.tanke756.top/gtkajnmwrc.html

[T42] Perl：变量类型
来源：http://hz.yueranfly.top/gtameceonw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.aibaodan.cn/gtayhdlxce.html

[T43] Perl：字符串插值
来源：http://hz.gogol.net.cn/gtogoqzqfv.html

"值: $a"
来源：http://hz.pycfn.com/gtwbnyrjhu.html

[T44] Perl：条件
来源：http://hz.pengpengdd.cyou/gtislivwgo.html

if ($a > 0) { print "正"; }
来源：http://hz.aibaodan.cn/gtioacqcpe.html

[T45] Perl：数组遍历
来源：http://hz.yj202588.top/gtlaviuihd.html

for my $x (@arr) { print $x; }
来源：http://hz.hnqzz.top/gtrhzyadys.html

[T46] Perl：哈希操作
来源：http://hz.zhixingplan.top/gtqvozbach.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.shanyushiyangtech.top/gtbqijqily.html

[T47] Perl：正则捕获
来源：http://hz.hfpthk.cn/gtymozokkh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.mhx1999.top/gtkyolgzal.html

[T48] Perl：正则替换
来源：http://hz.redwolf501.top/gtohlgtqax.html

$s =~ s/old/new/g;
来源：http://hz.jinqigufen.top/gtaniggkde.html

[T49] Perl：函数
来源：http://hz.yvedp.cn/gtmgsjzzlr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.xingfuxueyuan.xyz/gtvmbidyco.html

[T50] Perl：逐行读文件
来源：http://hz.zycfv.cn/gtnqggjxjp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.hammf.cn/gtsjxeiqqh.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.pengpengdd.cyou/gtcsetuhlg.html

[T51] Scala：Hello World
来源：http://hz.tian-w.cn/gthhriberl.html

println("Hello")
来源：http://hz.yangfankeji.com/gtyesxqqsp.html

[T52] Scala：变量
来源：http://hz.bjfxy.top/gtiivjubop.html

val a = 1;  var b = 2
来源：http://hz.pycfn.com/gtkztojctc.html

[T53] Scala：字符串插值
来源：http://hz.hnqzz.top/gtgawspzwh.html

s"值: $b"
来源：http://hz.daxiang520.top/gtvjzquqpw.html

[T54] Scala：集合映射
来源：http://hz.zdqjudy.top/gtbjdlpwuj.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.fzhhl.top/gtyelikqcs.html

[T55] Scala：集合过滤
来源：http://hz.hysaishi.cn/gtitqvqakp.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.zhongyouzk.top/gtpyldfvyc.html

[T56] Scala：样例类
来源：http://hz.tianlin.xyz/gtbnnksgle.html

case class User(name: String, age: Int)
来源：http://hz.gotoacloud.top/gtsgaalsyw.html

[T57] Scala：模式匹配
来源：http://hz.zdqjudy.top/gtskpyaouj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.shuidangran.top/gtkgicbvrz.html

[T58] Scala：函数定义
来源：http://hz.smart0.xyz/gtwmmarmdq.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.guowangkeji.top/gttqvtljsg.html

[T59] Scala：循环
来源：http://hz.ydzc1.top/gtpgrmpnnz.html

for (i <- 1 to 10) println(i)
来源：http://hz.dianchejie.cn/gtcohghxtl.html

[T60] Scala：折叠
来源：http://hz.guannengcc.top/gtdjolxgld.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.shanyushiyangkeji.top/gthcdcgwzw.html

================================================================================
来源：http://hz.birdmap.top/gtjkoodest.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.cqqwz.cn/gtvphmhgjy.html

================================================================================
来源：http://hz.yongpay.top/gtcildytyz.html

[U01] Py：创建虚拟环境
来源：http://hz.dashuyun.cn/gtyzhiuhyi.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.jinghuilouyu.cn/gtpgszvsoh.html

[U02] Py：导出 / 安装依赖
来源：http://hz.chenzaomai.com/gtlzxtjvqh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.redwolf501.top/gtejmqugtm.html

[U03] Py：加载 .env 配置
来源：http://hz.wangdashe.top/gtndmqhwzk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.tanke756.top/gtujmyzuwg.html

[U04] Py：变量调试打印
来源：http://hz.meibo888.top/gtmrkgxdfu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.wangshuangyany.cn/gtcgveodsu.html

[U05] Py：列表去重且保序
来源：http://hz.yonumen.top/gtkawzrkpd.html

list(dict.fromkeys(arr))
来源：http://hz.yj202588.top/gtllxssqvb.html

[U06] Py：合并两个字典
来源：http://hz.xziqi.cn/gtloldhsqx.html

{**a, **b}
来源：http://hz.ydzc1.top/gtkcikybir.html

[U07] Py：反转字典键值
来源：http://hz.tanke756.top/gtomehxcla.html

{v: k for k, v in d.items()}
来源：http://hz.yj202588.top/gtplosldzm.html

[U08] Py：展平二维列表
来源：http://hz.tian-w.cn/gthabcpnxq.html

[y for x in nested for y in x]
来源：http://hz.yuanzhike.top/gtasyzoktl.html

[U09] Py：字典取最大值的键
来源：http://hz.svipenyu.cn/gtsgyyjpmt.html

max(d, key=d.get)
来源：http://hz.zhiwuduotai.top/gtpafdzqkg.html

[U10] Py：按值排序字典
来源：http://hz.52xcode.cn/gtwhmseahp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.hammf.cn/gtcxwndthk.html

[U11] Py：生成器表达式
来源：http://hz.mhx1999.top/gtjbkvghjw.html

(x * 2 for x in arr)
来源：http://hz.cashguo.top/gtmysjprzy.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yj20258888.top/gtjqptwbqr.html

Counter(arr).most_common(3)
来源：http://hz.c1oappe.top/gtfjqlabnm.html

[U13] Py：固定长度队列
来源：http://hz.zhixingplan.top/gtazrfhdpb.html

deque(maxlen=10)
来源：http://hz.jqgufenzy.top/gtgzdkqhme.html

[U14] Py：分组收集到列表
来源：http://hz.dashuyun.cn/gtynfurjok.html

defaultdict(list)
来源：http://hz.yuxming.cn/gtxmhlpkkq.html

[U15] Py：高精度计时
来源：http://hz.yvedp.cn/gtqangidem.html

t = time.perf_counter()
来源：http://hz.jinqigufen.top/gtqmbwkmok.html

[U16] Py：命令行参数解析
来源：http://hz.zdqjudy.top/gtmrgnxwqp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.ydzc1.top/gtfpljtrog.html

[U17] Py：初始化日志
来源：http://hz.vqdsnc.cn/gtkabxncpo.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yangfankeji.com/gtnylpekao.html

[U18] Py：预编译正则
来源：http://hz.tanke756.top/gtfjjzqcbr.html

pat = re.compile(r"\d+")
来源：http://hz.aizwys.cn/gtivrbvzqr.html

[U19] Py：正则替换带回调
来源：http://hz.0kj1m.cn/gtnfzrsgzp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.wangdashe.top/gtpmazrknp.html

[U20] Py：缓存函数结果
来源：http://hz.havefunace.top/gtpsoamgem.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yanxiufei.cn/gtekntdlvc.html

[U21] Py：自定义上下文管理器
来源：http://hz.havefunace.top/gtvombqkoo.html

@contextlib.contextmanager
来源：http://hz.wangshuangyany.cn/gtzvhwjpbe.html

[U22] Py：矩阵转置
来源：http://hz.gaohongyu789.top/gtxlzdaudv.html

list(zip(*m))
来源：http://hz.sysykeji.top/gtnbuhjoug.html

[U23] Py：分块读取大文件
来源：http://hz.pycfn.com/gtndcigdas.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.ybcxt.top/gtmwradvkc.html

[U24] Py：路径操作
来源：http://hz.ybcxt.top/gtszgwlhfg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.dianchejie.cn/gtcxxlqxil.html

[U25] Py：CSV 按字典读
来源：http://hz.vqdsnc.cn/gteatnhtzp.html

csv.DictReader(f)
来源：http://hz.zhaomingkeji.xyz/gtefsuokvx.html

[U26] Py：并发下载
来源：http://hz.gogol.net.cn/gtmkdegbul.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.zhaomingkeji.xyz/gtjitlrzck.html

[U27] Py：异步 HTTP
来源：http://hz.sufxvd.cn/gthfrrmzen.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.cheryme.top/gtrenlazsg.html

[U28] Py：类型别名
来源：http://hz.gzhubu.top/gtrfdmhync.html

UserId = int
来源：http://hz.nanxuanxn.top/gtupdzfddk.html


<!-- 参考信息 -->