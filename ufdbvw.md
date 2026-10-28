代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://hz.cqqwz.cn/gtxsnzjhao.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.52xcode.cn/gtruoklhba.html

fclose(f);
来源：http://hz.9152youxi.cn/gtndntshwl.html

[S12] C：写文件
来源：http://hz.zhixingplan.top/gtmdhwkzvo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.daxiang520.top/gtbrfnlzwp.html

[S13] C：宏定义
来源：http://hz.gaohongyu789.top/gtxciadals.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zycfv.cn/gtwdwbtgvm.html

[S14] C：枚举
来源：http://hz.jyoumei.cn/gttpebjflw.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yj20258.top/gttgsnfmxx.html

[S15] C：类型转换
来源：http://hz.jinqigufen.top/gtiqnpwsbz.html

(double) a / b
来源：http://hz.yj202588.top/gtulmntzdy.html

[S16] C：位操作置位
来源：http://hz.haohaochexian.top/gtvkaoerth.html

x |= (1 << 3);
来源：http://hz.yangfankeji.com/gtciabcrbj.html

[S17] C：安全拼接字符串
来源：http://hz.cucudq.cn/gtdjkwhoct.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.chenlongwang.top/gtwooyiuef.html

[S18] C：命令行参数
来源：http://hz.dianchejie.cn/gtuxpvvhwd.html

int main(int argc, char **argv)
来源：http://hz.zhoulong.xyz/gtvjyudyzp.html

[S19] C：快速排序
来源：http://hz.yj20258888.top/gtcxrjqcxz.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jinyuanbaomall.cn/gtzhwvxfhf.html

[S20] C：二分查找
来源：http://hz.hywenlv.cn/gtlnxohati.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.gotoacloud.top/gtwuhxpett.html

[S21] C：字符类别判断
来源：http://hz.pengpengdd.cyou/gtqzefhzeq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ywan-chungtsiang.top/gtoqnsmyqu.html

[S22] C：字符串转数字
来源：http://hz.haohaochexian.top/gtunlaxsmk.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jianghu66.top/gtrllyebkr.html

[S23] C：随机数
来源：http://hz.zhixingplan.top/gtwyygymip.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.daxiang520.top/gtjhhrnwyg.html

[S24] C：获取本地时间
来源：http://hz.ydzc1.top/gtlzrpknee.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yuanzhike.top/gtbxczkvww.html

[S25] C：内存拷贝
来源：http://hz.tian-w.cn/gtamvmzfxq.html

memcpy(dst, src, n);
来源：http://hz.ydjk.org.cn/gtulexhbbm.html

[S26] C：内存清零
来源：http://hz.316326.xyz/gtqkhwocvm.html

memset(a, 0, sizeof a);
来源：http://hz.yangfankeji.com/gtktgdvsgi.html

[S27] C：定义常量
来源：http://hz.jinghuilouyu.cn/gteboczypj.html

const double PI = 3.14159;
来源：http://hz.shzxlz.cn/gtcpxyvpuo.html

[S28] C：静态变量
来源：http://hz.nwbrower.top/gtwfkhfizw.html

static int counter = 0;
来源：http://hz.jinqigufen.top/gtkehvwogb.html

[S29] C：变参函数
来源：http://hz.jlsjyb.cn/gtteqnlsal.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.guowangkeji.top/gtynotzjxa.html

[S30] C：头文件保护
来源：http://hz.fzhhl.top/gtpkqrfytz.html

#ifndef X_H
来源：http://hz.zycfv.cn/gtvhkhwmqj.html

#define X_H
来源：http://hz.ywan-chungtsiang.top/gtgouunxez.html

#endif
来源：http://hz.snrcjt.cn/gtomzsqhtx.html

[S31] C++：Hello World
来源：http://hz.jiagoushi.top/gtrknalmyd.html

#include <iostream>
来源：http://hz.ybcxt.top/gtvmzfuxpo.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hongshengwenyu.top/gtorrenapq.html

[S32] C++：字符串
来源：http://hz.ywan-chungtsiang.top/gtfazofpng.html

std::string s = "hi";  s += "!";
来源：http://hz.aibaodan.cn/gtyrbylsyf.html

[S33] C++：vector 增删
来源：http://hz.sweek.top/gtsvlyrftq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ehwqpu.com/gtsaofbies.html

[S34] C++：遍历 vector
来源：http://hz.jiagoushi.top/gtwqktelgr.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xinyue.icu/gtkbgeqlal.html

[S35] C++：map
来源：http://hz.chenlongwang.top/gtdcgdisdy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shzxlz.cn/gtetxapgrz.html

[S36] C++：unordered_map
来源：http://hz.pycfn.com/gtpmkynowt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.svipenyu.cn/gtizqcjwzn.html

[S37] C++：set
来源：http://hz.hnqzz.top/gtsgnoyoyy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.aibaodan.cn/gtmfinisei.html

[S38] C++：排序
来源：http://hz.birdmap.top/gtorrqucor.html

std::sort(v.begin(), v.end());
来源：http://hz.xuanzx.com/gtmdrgiuaq.html

[S39] C++：自定义比较器排序
来源：http://hz.pengpengdd.cyou/gtdtactnoa.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.sufxvd.cn/gtfvlrhorx.html

[S40] C++：查找元素
来源：http://hz.yueranfly.top/gtwuyfrtsy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yj20258.top/gtgpsmmgxg.html

[S41] C++：类与构造函数
来源：http://hz.snrcjt.cn/gtuizlbvxa.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xingfuxueyuan.xyz/gtdrollayd.html

[S42] C++：继承与虚函数
来源：http://hz.sweek.top/gtiblumowt.html

class B : public Base { public: void f() override {} };
来源：http://hz.jqgfzy.top/gtgunfousf.html

[S43] C++：智能指针
来源：http://hz.sxryk.cn/gtunwyhdyf.html

auto p = std::make_unique<int>(5);
来源：http://hz.hfpthk.cn/gtjjgefwrh.html

[S44] C++：引用传参
来源：http://hz.zhijiandao.cn/gtghlfkslo.html

void inc(int &x) { ++x; }
来源：http://hz.xuetiantiany.cn/gtsztmjkce.html

[S45] C++：lambda
来源：http://hz.ehwqpu.com/gtvwzcojjl.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.shzxlz.cn/gtcbwlxuvg.html

[S46] C++：函数模板
来源：http://hz.andypj.xyz/gtwcrhruhw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.fengsongda.top/gtypfeanlp.html

[S47] C++：结构化绑定遍历
来源：http://hz.xziqi.cn/gtqlmiqqtl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.cdnleiting.top/gtpkkvbmev.html

[S48] C++：逐行读文件
来源：http://hz.yanxiufei.cn/gtsnqqbhmh.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yuanzhike.top/gtxjnmumuu.html

while (std::getline(in, line)) { }
来源：http://hz.andypj.xyz/gttvuibvsi.html

[S49] C++：写文件
来源：http://hz.yuanzhike.top/gtxwbxmjzg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ydzc1.top/gtbvbopajy.html

[S50] C++：格式化数字
来源：http://hz.jiagoushi.top/gtejcpswgn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhaomingkeji.xyz/gttjbsammw.html

[S51] C++：显式类型转换
来源：http://hz.wangdashe.top/gtblzhcvcl.html

static_cast<double>(a) / b
来源：http://hz.hywenlv.cn/gtjpyrsika.html

[S52] C++：const 与 noexcept
来源：http://hz.ivvv.top/gthjcrlgch.html

int size() const noexcept { return n_; }
来源：http://hz.wangdashe.top/gtmvnbgiqu.html

[S53] C++：移动语义
来源：http://hz.yonumen.top/gtphunabzz.html

std::vector<int> w = std::move(v);
来源：http://hz.jqgufenzy.top/gtcrgbubdh.html

[S54] C++：异常处理
来源：http://hz.cqqwz.cn/gtaflbibmj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.nanxuanxn.top/gtjzfkgmfy.html

[S55] C++：结构化绑定
来源：http://hz.aizwys.cn/gtpdhcievc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.wangshuangyany.cn/gtziyzotyb.html

[S56] C++：optional
来源：http://hz.yj202588.top/gtpfcgfzjw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.fzhhl.top/gtbrgurglz.html

[S57] C++：编译期常量
来源：http://hz.hywenlv.cn/gthobofdcp.html

constexpr int N = 10;
来源：http://hz.hongshengwenyu.top/gtfnjjmvjt.html

[S58] C++：命名空间
来源：http://hz.ydzc1.top/gtztdrrikq.html

namespace ns { int f() { return 1; } }
来源：http://hz.jianghu66.top/gtwdlvdjhg.html

[S59] C++：静态断言
来源：http://hz.jinghuilouyu.cn/gtfejzdtfs.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.birdmap.top/gtxesulxjc.html

[S60] C++：遍历并删除元素
来源：http://hz.yj20258888.top/gtczoaaygf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.9152youxi.cn/gtueftyjuu.html

================================================================================
来源：http://hz.316326.xyz/gtlpqifpdv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.andypj.xyz/gttxkxregk.html

================================================================================
来源：http://hz.redwolf501.top/gtkiqaynbc.html

[T01] Kotlin：Hello World
来源：http://hz.yuxming.cn/gtlghvebcv.html

println("Hello")
来源：http://hz.yj20258.top/gtujvzmweg.html

[T02] Kotlin：变量
来源：http://hz.yuxming.cn/gtkpyozwoc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jiagoushi.top/gthkqirmrl.html

[T03] Kotlin：字符串模板
来源：http://hz.redwolf501.top/gtzvrtgxqz.html

"值: $b"
来源：http://hz.xuetiantiany.cn/gtsueowjku.html

[T04] Kotlin：空安全
来源：http://hz.bjfxy.top/gtyoctimnh.html

val n: String? = null;  n?.length
来源：http://hz.shangyingyoupin.top/gtxozburgu.html

[T05] Kotlin：when 表达式
来源：http://hz.jyoumei.cn/gtstxvcwal.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.chenlongwang.top/gtfeootxdx.html

[T06] Kotlin：集合映射
来源：http://hz.cqqwz.cn/gtzuguepao.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.dashuyun.cn/gtlhrzlgle.html

[T07] Kotlin：集合过滤
来源：http://hz.zhoulong.xyz/gtdjknymqr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xuanzx.com/gtabhhnxbz.html

[T08] Kotlin：数据类
来源：http://hz.kuanghao11.cn/gtlgweilsc.html

data class User(val name: String, val age: Int)
来源：http://hz.zhaomingkeji.xyz/gtewqgjgyb.html

[T09] Kotlin：扩展函数
来源：http://hz.tian-w.cn/gtwfwcxrfp.html

fun String.exclaim() = this + "!"
来源：http://hz.sufxvd.cn/gtdxqyluhx.html

[T10] Kotlin：默认参数
来源：http://hz.aizwys.cn/gtczjvsels.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ybcxt.top/gtyhyrbytq.html

[T11] Kotlin：协程
来源：http://hz.andypj.xyz/gtsrsyfloy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jqgfzy.top/gtbsszvtuz.html

[T12] Kotlin：解构声明
来源：http://hz.nanxuanxn.top/gtylldskld.html

val (a, b) = Pair(1, 2)
来源：http://hz.xziqi.cn/gtbskmyqce.html

[T13] Kotlin：只读 Map
来源：http://hz.chenjidiqi.icu/gtsfprquhm.html

val m = mapOf("a" to 1)
来源：http://hz.bjfxy.top/gtgagfsonn.html

[T14] Kotlin：循环
来源：http://hz.jinghuilouyu.cn/gtndhfncpz.html

for (i in 1..10) println(i)
来源：http://hz.zhixingplan.top/gthyjqxrjb.html

[T15] Kotlin：接口
来源：http://hz.xylfe.cn/gtpgostjjy.html

interface Shape { fun area(): Double }
来源：http://hz.zhoulong.xyz/gtkugdrafs.html

[T16] Swift：Hello World
来源：http://hz.ppjwa.cn/gtrthzcdhz.html

print("Hello")
来源：http://hz.tianlin.xyz/gtdnsllyll.html

[T17] Swift：变量与常量
来源：http://hz.hnxiangtu.top/gtakxsvoul.html

var a = 1;  let b = 2
来源：http://hz.aibaodan.cn/gtwgyyksdg.html

[T18] Swift：字符串插值
来源：http://hz.dianchejie.cn/gttxetwiof.html

"值: \(b)"
来源：http://hz.tian-w.cn/gtjcilejdc.html

[T19] Swift：可选绑定
来源：http://hz.wangdashe.top/gtnepsgnxp.html

if let n = opt { print(n) }
来源：http://hz.hywenlv.cn/gtomwqkpzi.html

[T20] Swift：数组操作
来源：http://hz.shzxlz.cn/gtropadxpc.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jianghu66.top/gtnljdxlji.html

[T21] Swift：遍历
来源：http://hz.ppjwa.cn/gtbwrlqvkf.html

for x in a { print(x) }
来源：http://hz.hammf.cn/gtrwnezfgd.html

[T22] Swift：字典
来源：http://hz.zhijiandao.cn/gtskuhqrcf.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.nanxinkj.top/gtxyqqfxsi.html

[T23] Swift：函数
来源：http://hz.ydzc1.top/gtguodijyp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ybcxt.top/gtdjhksmqv.html

[T24] Swift：闭包
来源：http://hz.yongpay.top/gtojqlurwm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jiagoushi.top/gtguviyytw.html

[T25] Swift：结构体
来源：http://hz.ydzc1.top/gtjulyazbz.html

struct P { var x: Int }
来源：http://hz.52xcode.cn/gtiquamcnh.html

[T26] Swift：类与重写
来源：http://hz.316326.xyz/gttgiaaanx.html

class A: Base { override func f() {} }
来源：http://hz.guannengcc.top/gtnhdjnhcx.html

[T27] Swift：错误处理
来源：http://hz.zdqjudy.top/gtvragkcoz.html

do { try f() } catch { print(error) }
来源：http://hz.jinqigfzy.top/gtnonbvcld.html

[T28] Swift：枚举
来源：http://hz.wangshuangyany.cn/gtifmhwdbz.html

enum Color { case red, green }
来源：http://hz.tianlin.xyz/gtsdurgwit.html

[T29] Swift：guard 提前返回
来源：http://hz.hywenlv.cn/gthfyoymhb.html

guard let x = opt else { return }
来源：http://hz.redwolf501.top/gtyxzkrwwm.html

[T30] Swift：协议
来源：http://hz.jyoumei.cn/gtocpdazsy.html

protocol Shape { func area() -> Double }
来源：http://hz.zhiwuduotai.top/gtbprflsrh.html

[T31] Lua：Hello World
来源：http://hz.yueranfly.top/gtepecsbno.html

print("Hello")
来源：http://hz.jinqigufen.top/gtdkpwnshm.html

[T32] Lua：局部变量
来源：http://hz.zhengqikj.top/gtwlwyqtri.html

local a = 1
来源：http://hz.tianlin.xyz/gtwxvpvetm.html

[T33] Lua：表（数组）
来源：http://hz.aibaodan.cn/gtleiwzawk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.sufxvd.cn/gtidqkodae.html

[T34] Lua：遍历表
来源：http://hz.cheryme.top/gtsvsdkzlb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.gzhubu.top/gtsbtpqvvk.html

[T35] Lua：字典表
来源：http://hz.yonumen.top/gtgwxqbzyg.html

local d = { a = 1 };  d.b = 2
来源：http://hz.birdmap.top/gtpmuqqypm.html

[T36] Lua：函数
来源：http://hz.jinyuanbaomall.cn/gtfisufsmr.html

function add(a, b) return a + b end
来源：http://hz.yuanzhike.top/gtyaksvtdh.html

[T37] Lua：字符串拼接
来源：http://hz.jqgfzy.top/gthoxxpsot.html

"a" .. "b"
来源：http://hz.chenlongwang.top/gtanyrvfdq.html

[T38] Lua：条件
来源：http://hz.yvedp.cn/gtwebxgdev.html

if x > 0 then print("正") end
来源：http://hz.jlsjyb.cn/gtldqleikh.html

[T39] Lua：模式匹配
来源：http://hz.hysaishi.cn/gtdalpxgiu.html

string.find(s, "%d+")
来源：http://hz.yj20258.top/gtnpfwcspg.html

[T40] Lua：元表
来源：http://hz.ppjwa.cn/gthuxkwltw.html

setmetatable({}, { __index = base })
来源：http://hz.chenlongwang.top/gtocrsnzug.html

[T41] Perl：Hello World
来源：http://hz.yj20258.top/gtpnpadyao.html

print "Hello\n";
来源：http://hz.yj202588.top/gtfyozzjwu.html

[T42] Perl：变量类型
来源：http://hz.jinqigfzy.top/gtwjnfkvgr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.ydjk.org.cn/gtaaobsdtk.html

[T43] Perl：字符串插值
来源：http://hz.cqqwz.cn/gtzpzxengk.html

"值: $a"
来源：http://hz.cucudq.cn/gtcsfmwptk.html

[T44] Perl：条件
来源：http://hz.daria6918.cn/gtsfzyxnnp.html

if ($a > 0) { print "正"; }
来源：http://hz.zhixingplan.top/gtnglnvroq.html

[T45] Perl：数组遍历
来源：http://hz.dianchejie.cn/gtkbztwtww.html

for my $x (@arr) { print $x; }
来源：http://hz.hammf.cn/gtapcjlxfm.html

[T46] Perl：哈希操作
来源：http://hz.andypj.xyz/gtbhiqldii.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zhongyouzk.top/gtiiualyyj.html

[T47] Perl：正则捕获
来源：http://hz.9152youxi.cn/gtvufvsiwc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.meibo888.top/gtwpmdzcyl.html

[T48] Perl：正则替换
来源：http://hz.snrcjt.cn/gtaxqnojoi.html

$s =~ s/old/new/g;
来源：http://hz.vqdsnc.cn/gtiewnzbzr.html

[T49] Perl：函数
来源：http://hz.c1oappe.top/gtrqkiscsf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.ywan-chungtsiang.top/gteythbmbc.html

[T50] Perl：逐行读文件
来源：http://hz.aizwys.cn/gtmulpfuvx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.shuidangran.top/gtckpstefn.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yuxming.cn/gtwkrbontg.html

[T51] Scala：Hello World
来源：http://hz.yj20258888.top/gtbtjjgvvo.html

println("Hello")
来源：http://hz.jyoumei.cn/gtfmasxkfx.html

[T52] Scala：变量
来源：http://hz.xylfe.cn/gtxkpwdbwz.html

val a = 1;  var b = 2
来源：http://hz.aizwys.cn/gtrhxdxdhs.html

[T53] Scala：字符串插值
来源：http://hz.feifeiyinyue.top/gtddljdzfr.html

s"值: $b"
来源：http://hz.wangshuangyany.cn/gtjqjzjlyq.html

[T54] Scala：集合映射
来源：http://hz.shangyingyoupin.top/gtpsugssjl.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.sysykeji.top/gtdovdzwgq.html

[T55] Scala：集合过滤
来源：http://hz.0kj1m.cn/gtfyigxjqy.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.ybcxt.top/gtefhsitcy.html

[T56] Scala：样例类
来源：http://hz.ppjwa.cn/gtgxgxuloy.html

case class User(name: String, age: Int)
来源：http://hz.hywenlv.cn/gtluzmrsye.html

[T57] Scala：模式匹配
来源：http://hz.zhixingplan.top/gtqjdomali.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.guannengcc.top/gtfqzunpvw.html

[T58] Scala：函数定义
来源：http://hz.shangyingyoupin.top/gtotpvhoez.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.shuidangran.top/gtebijahja.html

[T59] Scala：循环
来源：http://hz.havefunace.top/gtvdjvezfp.html

for (i <- 1 to 10) println(i)
来源：http://hz.gogol.net.cn/gtmnalywkv.html

[T60] Scala：折叠
来源：http://hz.yongpay.top/gtxmvxwzrf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hongshengwenyu.top/gtskmswmiq.html

================================================================================
来源：http://hz.xziqi.cn/gtfzsdgvkk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.316326.xyz/gtpehhwzvr.html

================================================================================
来源：http://hz.zhengqikj.top/gtixuafqlg.html

[U01] Py：创建虚拟环境
来源：http://hz.hammf.cn/gttlynpjwo.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.ywan-chungtsiang.top/gtdiwolhtk.html

[U02] Py：导出 / 安装依赖
来源：http://hz.hammf.cn/gtuzrhqiov.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yj202588.top/gtqzmimafy.html

[U03] Py：加载 .env 配置
来源：http://hz.hfpthk.cn/gtzfrfejdx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zycfv.cn/gtimahftik.html

[U04] Py：变量调试打印
来源：http://hz.ydzc1.top/gtrpiqfhsr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.gaohongyu789.top/gttvddcubi.html

[U05] Py：列表去重且保序
来源：http://hz.xuetiantiany.cn/gteuthnuyh.html

list(dict.fromkeys(arr))
来源：http://hz.hywenlv.cn/gtdrfgbcst.html

[U06] Py：合并两个字典
来源：http://hz.gotoacloud.top/gtbkiaixxk.html

{**a, **b}
来源：http://hz.gogol.net.cn/gtpaauutis.html

[U07] Py：反转字典键值
来源：http://hz.jyoumei.cn/gtfdlllwfv.html

{v: k for k, v in d.items()}
来源：http://hz.yj202588.top/gtjwsiqzgj.html

[U08] Py：展平二维列表
来源：http://hz.tian-w.cn/gtkjzibmip.html

[y for x in nested for y in x]
来源：http://hz.redwolf501.top/gtnbuorngx.html

[U09] Py：字典取最大值的键
来源：http://hz.cqqwz.cn/gtugvkbvnl.html

max(d, key=d.get)
来源：http://hz.jinghuilouyu.cn/gtmbxcqada.html

[U10] Py：按值排序字典
来源：http://hz.yj20258.top/gtptqqauhn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.cucudq.cn/gtmdvwtjro.html

[U11] Py：生成器表达式
来源：http://hz.yj20258888.top/gtzhrypomj.html

(x * 2 for x in arr)
来源：http://hz.mhx1999.top/gttxyqscki.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.cqqwz.cn/gtcocqmvuw.html

Counter(arr).most_common(3)
来源：http://hz.yj20258.top/gtnrinbwob.html

[U13] Py：固定长度队列
来源：http://hz.jinyuanbaomall.cn/gtcunfxprp.html

deque(maxlen=10)
来源：http://hz.ivvv.top/gtnhfupnwx.html

[U14] Py：分组收集到列表
来源：http://hz.jianghu66.top/gtomcryxgg.html

defaultdict(list)
来源：http://hz.gogol.net.cn/gtulqidcaq.html

[U15] Py：高精度计时
来源：http://hz.tianlin.xyz/gtpjcpawnp.html

t = time.perf_counter()
来源：http://hz.pycfn.com/gthbfexrqp.html

[U16] Py：命令行参数解析
来源：http://hz.hfpthk.cn/gtchxtxukc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.hongshengwenyu.top/gtrcupgapt.html

[U17] Py：初始化日志
来源：http://hz.hongshengwenyu.top/gttprbiamy.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.wangshuangyany.cn/gtmxwjxvcp.html

[U18] Py：预编译正则
来源：http://hz.hammf.cn/gtsbhkcwxb.html

pat = re.compile(r"\d+")
来源：http://hz.xylfe.cn/gtdevfckss.html

[U19] Py：正则替换带回调
来源：http://hz.jlsjyb.cn/gtpewfvvhf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.zhaomingkeji.xyz/gtkwyqpnyg.html

[U20] Py：缓存函数结果
来源：http://hz.xuetiantiany.cn/gtyyxzsvld.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zhijiandao.cn/gthcpglocw.html

[U21] Py：自定义上下文管理器
来源：http://hz.hongshengwenyu.top/gtcasvyysc.html

@contextlib.contextmanager
来源：http://hz.svipenyu.cn/gtdyfqomhr.html

[U22] Py：矩阵转置
来源：http://hz.jiagoushi.top/gteygacsis.html

list(zip(*m))
来源：http://hz.xylfe.cn/gtbsyfoski.html

[U23] Py：分块读取大文件
来源：http://hz.hywenlv.cn/gttgfhvxri.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.iojbl.cn/gtueunocil.html

[U24] Py：路径操作
来源：http://hz.shanyushiyangkeji.top/gtuwpfeofa.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.andypj.xyz/gtyibcpqke.html

[U25] Py：CSV 按字典读
来源：http://hz.yuxming.cn/gtaceobmkw.html

csv.DictReader(f)
来源：http://hz.shanyushiyangtech.top/gtevvejhqd.html

[U26] Py：并发下载
来源：http://hz.aizwys.cn/gtpiivfcww.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.ydjk.org.cn/gtnqzshmpw.html

[U27] Py：异步 HTTP
来源：http://hz.yj202588.top/gtwemlnuua.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.vqdsnc.cn/gtxvvavykv.html

[U28] Py：类型别名
来源：http://hz.fzhhl.top/gtnwkidvjl.html

UserId = int
来源：http://hz.c1oappe.top/gtwlksjjkh.html

[U29] Py：属性校验
来源：http://hz.shangyingyoupin.top/gtehmtcvid.html

@property 与 @x.setter 配合
来源：http://hz.dianchejie.cn/gtbmqvciji.html

[U30] Py：数据类
来源：http://hz.cucudq.cn/gtfmstrsyy.html

@dataclass(slots=True)
来源：http://hz.andypj.xyz/gtrvagziti.html

[U31] Py：单测
来源：http://hz.chenlongwang.top/gtsydvgxmd.html

python -m pytest -q
来源：http://hz.aizwys.cn/gtjoytooff.html

[U32] Py：代码格式化
来源：http://hz.jyoumei.cn/gteoionxrz.html

ruff format . && ruff check --fix .
来源：http://hz.sufxvd.cn/gtchxgitsy.html

[U33] Py：打包发布
来源：http://hz.hfpthk.cn/gtusokqzid.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.cdnleiting.top/gtjizerwuy.html

[U34] Py：判断编码
来源：http://hz.shuidangran.top/gtknmqznjj.html

chardet.detect(raw)
来源：http://hz.jiagoushi.top/gtnuekflzd.html


<!-- 参考信息 -->