代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhoulong.xyz/gtxofjnigx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.aibaodan.cn/gtdnpmvndz.html

fclose(f);
来源：http://hz.zhoulong.xyz/gturccqxyd.html

[S12] C：写文件
来源：http://hz.jqgfzy.top/gtevvznxlc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.chenjidiqi.icu/gtqosobvrq.html

[S13] C：宏定义
来源：http://hz.ywan-chungtsiang.top/gtiuvdigjp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.tianlin.xyz/gtnapkvuhp.html

[S14] C：枚举
来源：http://hz.svipenyu.cn/gtzjsljpye.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zdqjudy.top/gtjnhyzrvx.html

[S15] C：类型转换
来源：http://hz.guannengcc.top/gtecwtbaen.html

(double) a / b
来源：http://hz.jinqigufen.top/gtowrkyzga.html

[S16] C：位操作置位
来源：http://hz.hammf.cn/gtmtbflbtp.html

x |= (1 << 3);
来源：http://hz.guannengcc.top/gtqofrppax.html

[S17] C：安全拼接字符串
来源：http://hz.ywan-chungtsiang.top/gtoxrdygak.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ydzc1.top/gtyrcxfzzj.html

[S18] C：命令行参数
来源：http://hz.cdnleiting.top/gtblkzgaie.html

int main(int argc, char **argv)
来源：http://hz.ppjwa.cn/gtqvjkznye.html

[S19] C：快速排序
来源：http://hz.ivvv.top/gtfutyoics.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shanyushiyangtech.top/gtfakrtivv.html

[S20] C：二分查找
来源：http://hz.gogol.net.cn/gtienudkjr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.xinyue.icu/gtbkfeukgl.html

[S21] C：字符类别判断
来源：http://hz.jinyuanbaomall.cn/gtxmxbdvzw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ehwqpu.com/gtwjkvwxdf.html

[S22] C：字符串转数字
来源：http://hz.jinqigfzy.top/gtrgtojcrq.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ydjk.org.cn/gtnymtsopt.html

[S23] C：随机数
来源：http://hz.andypj.xyz/gtupdryfau.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hysaishi.cn/gtmrpypwef.html

[S24] C：获取本地时间
来源：http://hz.kuanghao11.cn/gtvylbmmmz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.sysykeji.top/gtztijnfti.html

[S25] C：内存拷贝
来源：http://hz.pycfn.com/gtmajslvsm.html

memcpy(dst, src, n);
来源：http://hz.kuanghao11.cn/gtdbqvxfok.html

[S26] C：内存清零
来源：http://hz.zhaomingkeji.xyz/gtehaquoga.html

memset(a, 0, sizeof a);
来源：http://hz.sufxvd.cn/gtijgjgaqc.html

[S27] C：定义常量
来源：http://hz.tianlin.xyz/gtwcihtphn.html

const double PI = 3.14159;
来源：http://hz.yuanzhike.top/gtfmjdevuz.html

[S28] C：静态变量
来源：http://hz.svipenyu.cn/gttnuuquua.html

static int counter = 0;
来源：http://hz.zhoulong.xyz/gtsspqfypm.html

[S29] C：变参函数
来源：http://hz.nanxuanxn.top/gtasywuobd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.pycfn.com/gtzbcmdvbt.html

[S30] C：头文件保护
来源：http://hz.nanxinkj.top/gtefvbvxva.html

#ifndef X_H
来源：http://hz.yueranfly.top/gtpinjhzcw.html

#define X_H
来源：http://hz.yanxiufei.cn/gtywavyses.html

#endif
来源：http://hz.chenlongwang.top/gtwflcjtir.html

[S31] C++：Hello World
来源：http://hz.xylfe.cn/gtmrmmpnti.html

#include <iostream>
来源：http://hz.c1oappe.top/gtlswtkiik.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.ybcxt.top/gteyqrhtdf.html

[S32] C++：字符串
来源：http://hz.tanke756.top/gteckurkfg.html

std::string s = "hi";  s += "!";
来源：http://hz.yanxiufei.cn/gtdhmeddgh.html

[S33] C++：vector 增删
来源：http://hz.daria6918.cn/gtgrepqase.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ybcxt.top/gtwpxxcpbf.html

[S34] C++：遍历 vector
来源：http://hz.pycfn.com/gtgcvprgqr.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.shanyushiyangtech.top/gtocqhzyrq.html

[S35] C++：map
来源：http://hz.hnqzz.top/gtbusawcbj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gogol.net.cn/gtqxhyuvwg.html

[S36] C++：unordered_map
来源：http://hz.yj20258888.top/gtmcbrgjic.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xuanzx.com/gtyeujpmbu.html

[S37] C++：set
来源：http://hz.snrcjt.cn/gtriedyyav.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jlsjyb.cn/gtbhtghjcs.html

[S38] C++：排序
来源：http://hz.wangdashe.top/gthnwqurzx.html

std::sort(v.begin(), v.end());
来源：http://hz.smart0.xyz/gtnxpvhydv.html

[S39] C++：自定义比较器排序
来源：http://hz.shuidangran.top/gtxeztrxix.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hnxiangtu.top/gtzlrxhwpt.html

[S40] C++：查找元素
来源：http://hz.jinghuilouyu.cn/gtqxxmnsfx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.fengsongda.top/gtwhliehhx.html

[S41] C++：类与构造函数
来源：http://hz.ppjwa.cn/gtnfsmjzjd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhiwuduotai.top/gtrfzfzxcw.html

[S42] C++：继承与虚函数
来源：http://hz.daxiang520.top/gtgtogqvsi.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhoulong.xyz/gtejblaiio.html

[S43] C++：智能指针
来源：http://hz.yj20258888.top/gtwrwibmdd.html

auto p = std::make_unique<int>(5);
来源：http://hz.nanxinkj.top/gtugqlgpde.html

[S44] C++：引用传参
来源：http://hz.birdmap.top/gttskyjxls.html

void inc(int &x) { ++x; }
来源：http://hz.316326.xyz/gtpvrjyysm.html

[S45] C++：lambda
来源：http://hz.smart0.xyz/gtoyrqpgte.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.sufxvd.cn/gtrxgtqqpk.html

[S46] C++：函数模板
来源：http://hz.ywan-chungtsiang.top/gtdfskevjg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jyoumei.cn/gtzucqbgdy.html

[S47] C++：结构化绑定遍历
来源：http://hz.andypj.xyz/gttmtrhuiy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.nanxuanxn.top/gtwvqcghjg.html

[S48] C++：逐行读文件
来源：http://hz.pycfn.com/gtpqtihins.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.gogol.net.cn/gtirmeimqb.html

while (std::getline(in, line)) { }
来源：http://hz.daxiang520.top/gttpczvrvr.html

[S49] C++：写文件
来源：http://hz.tianlin.xyz/gtzqetkhow.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yuxming.cn/gtazibqsnb.html

[S50] C++：格式化数字
来源：http://hz.jinghuilouyu.cn/gtgyvzfotf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yvedp.cn/gtxvauwcow.html

[S51] C++：显式类型转换
来源：http://hz.chenjidiqi.icu/gtompninim.html

static_cast<double>(a) / b
来源：http://hz.tanke756.top/gtsxzusaqr.html

[S52] C++：const 与 noexcept
来源：http://hz.52xcode.cn/gtzqltsrer.html

int size() const noexcept { return n_; }
来源：http://hz.fzhhl.top/gtbokubgnh.html

[S53] C++：移动语义
来源：http://hz.jqgfzy.top/gttalppavr.html

std::vector<int> w = std::move(v);
来源：http://hz.ppjwa.cn/gtiakgpubf.html

[S54] C++：异常处理
来源：http://hz.meibo888.top/gtxyhrzshp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.sysykeji.top/gttzpfvmru.html

[S55] C++：结构化绑定
来源：http://hz.xuetiantiany.cn/gturjzgdgg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.tian-w.cn/gtumpqrmgt.html

[S56] C++：optional
来源：http://hz.0kj1m.cn/gtsaxmkxce.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhaomingkeji.xyz/gtkpykbyee.html

[S57] C++：编译期常量
来源：http://hz.shanyushiyangkeji.top/gthsocipwh.html

constexpr int N = 10;
来源：http://hz.zhengqikj.top/gtsrcdllkb.html

[S58] C++：命名空间
来源：http://hz.meibo888.top/gtusbhtijv.html

namespace ns { int f() { return 1; } }
来源：http://hz.sweek.top/gtirwdvdtc.html

[S59] C++：静态断言
来源：http://hz.9152youxi.cn/gtntbeydur.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jinqigfzy.top/gtmmlhrymu.html

[S60] C++：遍历并删除元素
来源：http://hz.cqqwz.cn/gtdnmvyclm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yuxming.cn/gtwchaqouw.html

================================================================================
来源：http://hz.sweek.top/gtrokcrzct.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhengqikj.top/gtrukwgpfj.html

================================================================================
来源：http://hz.zhengqikj.top/gtcbttyepy.html

[T01] Kotlin：Hello World
来源：http://hz.cqqwz.cn/gthnzzejji.html

println("Hello")
来源：http://hz.xingfuxueyuan.xyz/gtctesdkfy.html

[T02] Kotlin：变量
来源：http://hz.daxiang520.top/gtgqddxzjj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hnxiangtu.top/gtlrpkejcl.html

[T03] Kotlin：字符串模板
来源：http://hz.fzhhl.top/gtheyfpijp.html

"值: $b"
来源：http://hz.gzhubu.top/gtqqsivbtg.html

[T04] Kotlin：空安全
来源：http://hz.feifeiyinyue.top/gtiwwyzsie.html

val n: String? = null;  n?.length
来源：http://hz.hywenlv.cn/gttolpslqc.html

[T05] Kotlin：when 表达式
来源：http://hz.dashuyun.cn/gtuiegqcuc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jyoumei.cn/gtuimvxsgt.html

[T06] Kotlin：集合映射
来源：http://hz.cqqwz.cn/gtpinbteno.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.dianchejie.cn/gtxhwryklu.html

[T07] Kotlin：集合过滤
来源：http://hz.jinyuanbaomall.cn/gteacbpisc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hfpthk.cn/gtwrjiqccg.html

[T08] Kotlin：数据类
来源：http://hz.guowangkeji.top/gtsauydiiw.html

data class User(val name: String, val age: Int)
来源：http://hz.jlsjyb.cn/gtftvunclm.html

[T09] Kotlin：扩展函数
来源：http://hz.hammf.cn/gtrdaowddw.html

fun String.exclaim() = this + "!"
来源：http://hz.wangdashe.top/gttfxflhqo.html

[T10] Kotlin：默认参数
来源：http://hz.gotoacloud.top/gtobgagvnv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jlsjyb.cn/gthlvmignq.html

[T11] Kotlin：协程
来源：http://hz.fengsongda.top/gtesnaysxr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.redwolf501.top/gtecitrnbz.html

[T12] Kotlin：解构声明
来源：http://hz.xinyue.icu/gtjwfvyyia.html

val (a, b) = Pair(1, 2)
来源：http://hz.chenjidiqi.icu/gtosnmpjse.html

[T13] Kotlin：只读 Map
来源：http://hz.daria6918.cn/gtsogigjrk.html

val m = mapOf("a" to 1)
来源：http://hz.yuxming.cn/gtqqskfdnk.html

[T14] Kotlin：循环
来源：http://hz.dashuyun.cn/gtwwvydkdq.html

for (i in 1..10) println(i)
来源：http://hz.chenjidiqi.icu/gtkpmvactk.html

[T15] Kotlin：接口
来源：http://hz.aibaodan.cn/gtkxruhcze.html

interface Shape { fun area(): Double }
来源：http://hz.nanxuanxn.top/gtspkbwxbw.html

[T16] Swift：Hello World
来源：http://hz.snrcjt.cn/gtstmrqpqn.html

print("Hello")
来源：http://hz.tanke756.top/gtmciajcuc.html

[T17] Swift：变量与常量
来源：http://hz.jinqigfzy.top/gtujgyqelm.html

var a = 1;  let b = 2
来源：http://hz.yvedp.cn/gtizpswxfa.html

[T18] Swift：字符串插值
来源：http://hz.jinqigfzy.top/gtyngfuybf.html

"值: \(b)"
来源：http://hz.andypj.xyz/gtltqpzcny.html

[T19] Swift：可选绑定
来源：http://hz.cqqwz.cn/gtbsfdqkjr.html

if let n = opt { print(n) }
来源：http://hz.aibaodan.cn/gtwmdisekm.html

[T20] Swift：数组操作
来源：http://hz.andypj.xyz/gttzfepliw.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.havefunace.top/gtualpyjjz.html

[T21] Swift：遍历
来源：http://hz.vqdsnc.cn/gtahxnvxrq.html

for x in a { print(x) }
来源：http://hz.wangshuangyany.cn/gtaknwnvhw.html

[T22] Swift：字典
来源：http://hz.yueranfly.top/gtmtxcavyf.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jyoumei.cn/gtaklqzjrj.html

[T23] Swift：函数
来源：http://hz.tian-w.cn/gtwgpygyhe.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.fzhhl.top/gtqmxzqvkp.html

[T24] Swift：闭包
来源：http://hz.gogol.net.cn/gtggskwzaz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.fengsongda.top/gtsyhnteyj.html

[T25] Swift：结构体
来源：http://hz.aibaodan.cn/gttmbtllin.html

struct P { var x: Int }
来源：http://hz.wangshuangyany.cn/gtecgrncrz.html

[T26] Swift：类与重写
来源：http://hz.smart0.xyz/gtpksjynym.html

class A: Base { override func f() {} }
来源：http://hz.zhongyouzk.top/gtoinyhihw.html

[T27] Swift：错误处理
来源：http://hz.yanxiufei.cn/gtsxcusyxm.html

do { try f() } catch { print(error) }
来源：http://hz.snrcjt.cn/gtjdxmcxad.html

[T28] Swift：枚举
来源：http://hz.xingfuxueyuan.xyz/gtsfirjiwv.html

enum Color { case red, green }
来源：http://hz.meibo888.top/gtcibmdbti.html

[T29] Swift：guard 提前返回
来源：http://hz.c1oappe.top/gtupyiahwl.html

guard let x = opt else { return }
来源：http://hz.guowangkeji.top/gtqrijzgmo.html

[T30] Swift：协议
来源：http://hz.yongpay.top/gtdtxfdekm.html

protocol Shape { func area() -> Double }
来源：http://hz.tianlin.xyz/gtkfawkgkv.html

[T31] Lua：Hello World
来源：http://hz.316326.xyz/gtykzivzbg.html

print("Hello")
来源：http://hz.yuanzhike.top/gtnnumyhlk.html

[T32] Lua：局部变量
来源：http://hz.gaohongyu789.top/gtkpcadnla.html

local a = 1
来源：http://hz.gotoacloud.top/gtiwxigixm.html

[T33] Lua：表（数组）
来源：http://hz.wangdashe.top/gtnsmknchy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.iojbl.cn/gtsfictzkj.html

[T34] Lua：遍历表
来源：http://hz.ehwqpu.com/gtytlffewo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.9152youxi.cn/gtmmfzqnyq.html

[T35] Lua：字典表
来源：http://hz.yanxiufei.cn/gtwzgxathq.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yvedp.cn/gtdutupiva.html

[T36] Lua：函数
来源：http://hz.snrcjt.cn/gtsiadcprp.html

function add(a, b) return a + b end
来源：http://hz.jianghu66.top/gtriviqtqv.html

[T37] Lua：字符串拼接
来源：http://hz.0kj1m.cn/gtloyonjjs.html

"a" .. "b"
来源：http://hz.pycfn.com/gtpunonowr.html

[T38] Lua：条件
来源：http://hz.chenjidiqi.icu/gtpxeblsnx.html

if x > 0 then print("正") end
来源：http://hz.gzhubu.top/gtgicpnelf.html

[T39] Lua：模式匹配
来源：http://hz.shanyushiyangkeji.top/gtbeueixyl.html

string.find(s, "%d+")
来源：http://hz.jinghuilouyu.cn/gtbnrknnju.html

[T40] Lua：元表
来源：http://hz.nanxuanxn.top/gttembiwii.html

setmetatable({}, { __index = base })
来源：http://hz.cqqwz.cn/gtiwmeoqel.html

[T41] Perl：Hello World
来源：http://hz.yvedp.cn/gtutalaevf.html

print "Hello\n";
来源：http://hz.ybcxt.top/gtsntosxau.html

[T42] Perl：变量类型
来源：http://hz.dianchejie.cn/gtnnzeptzv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jyoumei.cn/gttrnafxir.html

[T43] Perl：字符串插值
来源：http://hz.zhijiandao.cn/gtforbfyow.html

"值: $a"
来源：http://hz.jianghu66.top/gtotiklksg.html

[T44] Perl：条件
来源：http://hz.jiagoushi.top/gtlovkryiw.html

if ($a > 0) { print "正"; }
来源：http://hz.mhx1999.top/gtkvajfmri.html

[T45] Perl：数组遍历
来源：http://hz.yj202588.top/gtjvlblcsr.html

for my $x (@arr) { print $x; }
来源：http://hz.pycfn.com/gthidgohha.html

[T46] Perl：哈希操作
来源：http://hz.jinyuanbaomall.cn/gtddbpmyvq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.dianchejie.cn/gtbbczqqjq.html

[T47] Perl：正则捕获
来源：http://hz.yongpay.top/gtaltoyxev.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.xingfuxueyuan.xyz/gtfkvybjhz.html

[T48] Perl：正则替换
来源：http://hz.ydzc1.top/gtwkpkuybc.html

$s =~ s/old/new/g;
来源：http://hz.nanxinkj.top/gtwrkluulz.html

[T49] Perl：函数
来源：http://hz.xingfuxueyuan.xyz/gtckgspnot.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zycfv.cn/gtaaiatyqq.html

[T50] Perl：逐行读文件
来源：http://hz.hnqzz.top/gtkywdmvkq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.aizwys.cn/gttslkppin.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.zhengqikj.top/gtosltcfac.html

[T51] Scala：Hello World
来源：http://hz.cucudq.cn/gteqbomedd.html

println("Hello")
来源：http://hz.zhaomingkeji.xyz/gtlykhlkty.html

[T52] Scala：变量
来源：http://hz.yangfankeji.com/gtpomxznfp.html

val a = 1;  var b = 2
来源：http://hz.kuanghao11.cn/gthcunqtiq.html

[T53] Scala：字符串插值
来源：http://hz.daxiang520.top/gtvcnthrpo.html

s"值: $b"
来源：http://hz.yonumen.top/gtgqgbigpd.html

[T54] Scala：集合映射
来源：http://hz.jiagoushi.top/gtovazmbou.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.guowangkeji.top/gtcdufwysw.html

[T55] Scala：集合过滤
来源：http://hz.feifeiyinyue.top/gtvevfjxdl.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.gotoacloud.top/gtlqgicklv.html

[T56] Scala：样例类
来源：http://hz.fzhhl.top/gtnvjrxcni.html

case class User(name: String, age: Int)
来源：http://hz.sysykeji.top/gteriugzrn.html

[T57] Scala：模式匹配
来源：http://hz.haohaochexian.top/gtfqdbaiqt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.pycfn.com/gtmlnvwbdu.html

[T58] Scala：函数定义
来源：http://hz.zhijiandao.cn/gtldgizfsx.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.ybcxt.top/gtnwavgsvo.html

[T59] Scala：循环
来源：http://hz.jinghuilouyu.cn/gtvixrbscw.html

for (i <- 1 to 10) println(i)
来源：http://hz.jqgfzy.top/gtvscthitq.html

[T60] Scala：折叠
来源：http://hz.tanke756.top/gtlmutsnbw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.zycfv.cn/gtdbxcriwv.html

================================================================================
来源：http://hz.quarkkingdee.top/gtsuvbwtpr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.chenjidiqi.icu/gtamwsifdz.html

================================================================================
来源：http://hz.mhx1999.top/gtkzivoejv.html

[U01] Py：创建虚拟环境
来源：http://hz.hongshengwenyu.top/gtlnoqfegm.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.fengsongda.top/gtjkzsdcej.html

[U02] Py：导出 / 安装依赖
来源：http://hz.yj20258888.top/gtdaqbmrkf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jlsjyb.cn/gtewyfpliq.html

[U03] Py：加载 .env 配置
来源：http://hz.yj20258.top/gtexgvwhni.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yueranfly.top/gtnrcwkezz.html

[U04] Py：变量调试打印
来源：http://hz.svipenyu.cn/gteibsulzj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zhiwuduotai.top/gtlzywwjly.html

[U05] Py：列表去重且保序
来源：http://hz.yj20258.top/gtyghquget.html

list(dict.fromkeys(arr))
来源：http://hz.wangshuangyany.cn/gtpfxfjyeo.html

[U06] Py：合并两个字典
来源：http://hz.bjfxy.top/gthtidyley.html

{**a, **b}
来源：http://hz.sufxvd.cn/gthtmrhbrr.html

[U07] Py：反转字典键值
来源：http://hz.xylfe.cn/gtfhynnfmk.html

{v: k for k, v in d.items()}
来源：http://hz.0kj1m.cn/gtfqtilmat.html

[U08] Py：展平二维列表
来源：http://hz.jiagoushi.top/gtxljzsqlg.html

[y for x in nested for y in x]
来源：http://hz.xuanzx.com/gttyeitrnu.html

[U09] Py：字典取最大值的键
来源：http://hz.yongpay.top/gtzkkkdewz.html

max(d, key=d.get)
来源：http://hz.pycfn.com/gtwwasqxxr.html

[U10] Py：按值排序字典
来源：http://hz.hnxiangtu.top/gtoxlykvxc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.tian-w.cn/gtvdjubxcc.html

[U11] Py：生成器表达式
来源：http://hz.yongpay.top/gtjhuuwfdk.html

(x * 2 for x in arr)
来源：http://hz.mhx1999.top/gtiailgbam.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.zhiwuduotai.top/gtnqjqotap.html

Counter(arr).most_common(3)
来源：http://hz.gaohongyu789.top/gtnwhqsnim.html

[U13] Py：固定长度队列
来源：http://hz.hammf.cn/gtwqhbduzn.html

deque(maxlen=10)
来源：http://hz.xingfuxueyuan.xyz/gtremslopr.html

[U14] Py：分组收集到列表
来源：http://hz.xinyue.icu/gtzcmitmof.html

defaultdict(list)
来源：http://hz.mhx1999.top/gtphbbrkve.html

[U15] Py：高精度计时
来源：http://hz.pycfn.com/gtaamildkp.html

t = time.perf_counter()
来源：http://hz.xylfe.cn/gtbuvvhajd.html

[U16] Py：命令行参数解析
来源：http://hz.jinghuilouyu.cn/gtskyiwlrw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.haohaochexian.top/gttqjwvldm.html

[U17] Py：初始化日志
来源：http://hz.xuanzx.com/gtcugunnnz.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.xziqi.cn/gtzabqjgyk.html

[U18] Py：预编译正则
来源：http://hz.yj20258888.top/gtsclxzedt.html

pat = re.compile(r"\d+")
来源：http://hz.yj202588.top/gtopcgwcnv.html

[U19] Py：正则替换带回调
来源：http://hz.dashuyun.cn/gttnnvtnme.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.gotoacloud.top/gtzovywhhf.html

[U20] Py：缓存函数结果
来源：http://hz.mhx1999.top/gtpprbxqbn.html

@functools.lru_cache(maxsize=None)
来源：http://hz.shuidangran.top/gtaoixagrj.html

[U21] Py：自定义上下文管理器
来源：http://hz.sweek.top/gtfxnlbphv.html

@contextlib.contextmanager
来源：http://hz.fzhhl.top/gtywtwkmqt.html

[U22] Py：矩阵转置
来源：http://hz.ivvv.top/gtzbodenuy.html

list(zip(*m))
来源：http://hz.hnqzz.top/gtjgzpvaol.html

[U23] Py：分块读取大文件
来源：http://hz.jqgufenzy.top/gtdgbxxobn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.c1oappe.top/gtwtroxdvk.html

[U24] Py：路径操作
来源：http://hz.shuidangran.top/gtprtzehon.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.andypj.xyz/gthhyqpjtj.html

[U25] Py：CSV 按字典读
来源：http://hz.xingfuxueyuan.xyz/gtsxtzwcge.html

csv.DictReader(f)
来源：http://hz.hongshengwenyu.top/gtpbqakcym.html

[U26] Py：并发下载
来源：http://hz.fzhhl.top/gtjfkytwfr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.hammf.cn/gtbjafisux.html

[U27] Py：异步 HTTP
来源：http://hz.cashguo.top/gtzsngfjoy.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.kuanghao11.cn/gtcoytfpha.html

[U28] Py：类型别名
来源：http://hz.pycfn.com/gtozffzhtn.html

UserId = int
来源：http://hz.chenzaomai.com/gtyrjzemjv.html

[U29] Py：属性校验
来源：http://hz.iojbl.cn/gthilouaue.html

@property 与 @x.setter 配合
来源：http://hz.jqgfzy.top/gtipimaxat.html

[U30] Py：数据类
来源：http://hz.cqqwz.cn/gtvdbtrdvu.html

@dataclass(slots=True)
来源：http://hz.yongpay.top/gtkouvcadw.html

[U31] Py：单测
来源：http://hz.jlsjyb.cn/gtsmsxthuq.html

python -m pytest -q
来源：http://hz.iojbl.cn/gthmpfyjzv.html

[U32] Py：代码格式化
来源：http://hz.zhengqikj.top/gtkbnucjtq.html

ruff format . && ruff check --fix .
来源：http://hz.gotoacloud.top/gtcfizbalp.html

[U33] Py：打包发布
来源：http://hz.guowangkeji.top/gtxsyqzful.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.gogol.net.cn/gtncsxqhwd.html

[U34] Py：判断编码
来源：http://hz.daria6918.cn/gtplidzjxi.html

chardet.detect(raw)
来源：http://hz.tian-w.cn/gtgqefnytr.html


<!-- 参考信息 -->