代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hongshengwenyu.top/gtrmotqzrv.html

[S08] C：动态内存分配与释放
来源：http://hz.nanxuanxn.top/gtrjiefylg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.0kj1m.cn/gtkfkkksof.html

[S09] C：结构体定义与初始化
来源：http://hz.ydjk.org.cn/gtdqrkgvuf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.pycfn.com/gtwmibgsqq.html

[S10] C：指针与解引用
来源：http://hz.cdnleiting.top/gtzptbuzhm.html

int *p = &a;  *p = 5;
来源：http://hz.xylfe.cn/gtxqrgiusy.html

[S11] C：逐行读文件
来源：http://hz.zhongyouzk.top/gtoowuoona.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.kuanghao11.cn/gtikqmiypd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yueranfly.top/gtxlptdawf.html

fclose(f);
来源：http://hz.fengsongda.top/gtnpiqpxct.html

[S12] C：写文件
来源：http://hz.zhijiandao.cn/gtsqjgoavf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.chenjidiqi.icu/gtzaxxrgrd.html

[S13] C：宏定义
来源：http://hz.sysykeji.top/gtgfeousuo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.sysykeji.top/gtzshlcgml.html

[S14] C：枚举
来源：http://hz.sufxvd.cn/gtszytpoel.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.gogol.net.cn/gtsellsvmv.html

[S15] C：类型转换
来源：http://hz.cheryme.top/gtirjodktm.html

(double) a / b
来源：http://hz.sweek.top/gtgkfccjnq.html

[S16] C：位操作置位
来源：http://hz.jinyuanbaomall.cn/gtjxotpvkc.html

x |= (1 << 3);
来源：http://hz.zycfv.cn/gtenxgijfj.html

[S17] C：安全拼接字符串
来源：http://hz.tanke756.top/gtakhhmcdi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.hammf.cn/gtdqxmjqwj.html

[S18] C：命令行参数
来源：http://hz.zhijiandao.cn/gtagsqgbxw.html

int main(int argc, char **argv)
来源：http://hz.fzhhl.top/gthylkdkxz.html

[S19] C：快速排序
来源：http://hz.zhengqikj.top/gtkpyaygen.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.redwolf501.top/gtpgbjwdfr.html

[S20] C：二分查找
来源：http://hz.jiagoushi.top/gtfgjvncwi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.chenlongwang.top/gttzczuipv.html

[S21] C：字符类别判断
来源：http://hz.haohaochexian.top/gtcjgreyfi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.bjfxy.top/gthsunndwn.html

[S22] C：字符串转数字
来源：http://hz.sufxvd.cn/gtaabtjjvj.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jinghuilouyu.cn/gtqlmjslop.html

[S23] C：随机数
来源：http://hz.daxiang520.top/gtqgnqgsiq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yuxming.cn/gthfpkwrfj.html

[S24] C：获取本地时间
来源：http://hz.chenlongwang.top/gtufvdvukg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yanxiufei.cn/gtkblbapwx.html

[S25] C：内存拷贝
来源：http://hz.vqdsnc.cn/gtrcqdaogf.html

memcpy(dst, src, n);
来源：http://hz.iojbl.cn/gtgadtbbnb.html

[S26] C：内存清零
来源：http://hz.jqgufenzy.top/gtyumosvox.html

memset(a, 0, sizeof a);
来源：http://hz.daxiang520.top/gtojvurcer.html

[S27] C：定义常量
来源：http://hz.smart0.xyz/gtyqakjxns.html

const double PI = 3.14159;
来源：http://hz.havefunace.top/gtmqqqhyus.html

[S28] C：静态变量
来源：http://hz.sweek.top/gtbtsgamfc.html

static int counter = 0;
来源：http://hz.quarkkingdee.top/gtxmqggtjv.html

[S29] C：变参函数
来源：http://hz.zdqjudy.top/gtygbosmum.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhongyouzk.top/gtqripxueo.html

[S30] C：头文件保护
来源：http://hz.tianlin.xyz/gtkaubdjsb.html

#ifndef X_H
来源：http://hz.svipenyu.cn/gtydvxwlhx.html

#define X_H
来源：http://hz.zhongyouzk.top/gtcldwnfzb.html

#endif
来源：http://hz.ppjwa.cn/gtjtkpkdbb.html

[S31] C++：Hello World
来源：http://hz.wangdashe.top/gtjzpwrsln.html

#include <iostream>
来源：http://hz.zdqjudy.top/gtkeyayjpi.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xuanzx.com/gtnkgajabq.html

[S32] C++：字符串
来源：http://hz.fengsongda.top/gtbivicbbk.html

std::string s = "hi";  s += "!";
来源：http://hz.0kj1m.cn/gtgwdybqbt.html

[S33] C++：vector 增删
来源：http://hz.dianchejie.cn/gtajukdgwf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yuxming.cn/gtegzyknjo.html

[S34] C++：遍历 vector
来源：http://hz.ywan-chungtsiang.top/gtcfvcagob.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jinqigfzy.top/gtjuzbpdos.html

[S35] C++：map
来源：http://hz.yj20258888.top/gtdhblwkpb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.birdmap.top/gtxecbyuhq.html

[S36] C++：unordered_map
来源：http://hz.gotoacloud.top/gtkicdjzvj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhixingplan.top/gtqxzpysvf.html

[S37] C++：set
来源：http://hz.sxryk.cn/gtarnpmaio.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.feifeiyinyue.top/gttrrzkkwg.html

[S38] C++：排序
来源：http://hz.daria6918.cn/gtlltlyqhm.html

std::sort(v.begin(), v.end());
来源：http://hz.ehwqpu.com/gtkjjqafyf.html

[S39] C++：自定义比较器排序
来源：http://hz.yanxiufei.cn/gtjvcscjjk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.guannengcc.top/gtqvxkbimm.html

[S40] C++：查找元素
来源：http://hz.xylfe.cn/gtnfngwauj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.shanyushiyangkeji.top/gtjhhepagl.html

[S41] C++：类与构造函数
来源：http://hz.shangyingyoupin.top/gtbtfmxekw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hnxiangtu.top/gtyxdavxnn.html

[S42] C++：继承与虚函数
来源：http://hz.vqdsnc.cn/gtbqhlypfs.html

class B : public Base { public: void f() override {} };
来源：http://hz.aibaodan.cn/gtqvebobjf.html

[S43] C++：智能指针
来源：http://hz.haohaochexian.top/gtmkdniymc.html

auto p = std::make_unique<int>(5);
来源：http://hz.pengpengdd.cyou/gtmigxxvwq.html

[S44] C++：引用传参
来源：http://hz.52xcode.cn/gtijzlyebm.html

void inc(int &x) { ++x; }
来源：http://hz.snrcjt.cn/gtjihezbwl.html

[S45] C++：lambda
来源：http://hz.ydjk.org.cn/gtibtpvwfy.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.nanxuanxn.top/gtpuitdgpw.html

[S46] C++：函数模板
来源：http://hz.c1oappe.top/gtktzpbprs.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.daxiang520.top/gtdmnqqber.html

[S47] C++：结构化绑定遍历
来源：http://hz.iojbl.cn/gtwpjimnrm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.cdnleiting.top/gtyronqoaa.html

[S48] C++：逐行读文件
来源：http://hz.yj20258.top/gtygkkjnis.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhixingplan.top/gtfknxuzoi.html

while (std::getline(in, line)) { }
来源：http://hz.shangyingyoupin.top/gtwfrcjgsv.html

[S49] C++：写文件
来源：http://hz.ywan-chungtsiang.top/gtnbitbore.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.wangshuangyany.cn/gtteeleohz.html

[S50] C++：格式化数字
来源：http://hz.cashguo.top/gtqhauhtww.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.shuidangran.top/gtkoejtpzx.html

[S51] C++：显式类型转换
来源：http://hz.daxiang520.top/gtqgjhyzlw.html

static_cast<double>(a) / b
来源：http://hz.yueranfly.top/gtzqnuotbv.html

[S52] C++：const 与 noexcept
来源：http://hz.shzxlz.cn/gtmliisnjt.html

int size() const noexcept { return n_; }
来源：http://hz.smart0.xyz/gtrxgczpjf.html

[S53] C++：移动语义
来源：http://hz.jlsjyb.cn/gtswhvamlg.html

std::vector<int> w = std::move(v);
来源：http://hz.yueranfly.top/gtvvpltgnj.html

[S54] C++：异常处理
来源：http://hz.ydjk.org.cn/gtidrhuvrv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yanxiufei.cn/gtxfrcltec.html

[S55] C++：结构化绑定
来源：http://hz.shuidangran.top/gtuflurzww.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yvedp.cn/gtaoymrpon.html

[S56] C++：optional
来源：http://hz.zhaomingkeji.xyz/gtakgakgqw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.pycfn.com/gtdadoqzyk.html

[S57] C++：编译期常量
来源：http://hz.yvedp.cn/gtmzvczree.html

constexpr int N = 10;
来源：http://hz.nanxinkj.top/gtxpfixofs.html

[S58] C++：命名空间
来源：http://hz.shuidangran.top/gtihyoybfj.html

namespace ns { int f() { return 1; } }
来源：http://hz.jinqigfzy.top/gtrvgqjmxq.html

[S59] C++：静态断言
来源：http://hz.fengsongda.top/gturicsmmd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zhijiandao.cn/gtgdvqgxhl.html

[S60] C++：遍历并删除元素
来源：http://hz.meibo888.top/gtfnrsokns.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.ehwqpu.com/gtpvqjmltk.html

================================================================================
来源：http://hz.guowangkeji.top/gtsapyczbb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jianghu66.top/gtaahazzhu.html

================================================================================
来源：http://hz.jlsjyb.cn/gtzstmeyhs.html

[T01] Kotlin：Hello World
来源：http://hz.52xcode.cn/gtqvfxkmfe.html

println("Hello")
来源：http://hz.cqqwz.cn/gtgxktmuwm.html

[T02] Kotlin：变量
来源：http://hz.sxryk.cn/gtyiefvjvx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.bjfxy.top/gtqljzajhz.html

[T03] Kotlin：字符串模板
来源：http://hz.cashguo.top/gtwrkvzmen.html

"值: $b"
来源：http://hz.yongpay.top/gtosvmgizd.html

[T04] Kotlin：空安全
来源：http://hz.jinyuanbaomall.cn/gthzfqbhai.html

val n: String? = null;  n?.length
来源：http://hz.guowangkeji.top/gtlwiunmbr.html

[T05] Kotlin：when 表达式
来源：http://hz.hnxiangtu.top/gtnddbifmo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.guowangkeji.top/gtzzqbdpqo.html

[T06] Kotlin：集合映射
来源：http://hz.yongpay.top/gtixhetbjt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.xinyue.icu/gtcbwitbif.html

[T07] Kotlin：集合过滤
来源：http://hz.cucudq.cn/gtklemdqak.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yvedp.cn/gthmmknhxe.html

[T08] Kotlin：数据类
来源：http://hz.zdqjudy.top/gtzdrikevq.html

data class User(val name: String, val age: Int)
来源：http://hz.zhixingplan.top/gtougcquqq.html

[T09] Kotlin：扩展函数
来源：http://hz.jinqigfzy.top/gtjcwlpffz.html

fun String.exclaim() = this + "!"
来源：http://hz.cashguo.top/gtevfgdfom.html

[T10] Kotlin：默认参数
来源：http://hz.sysykeji.top/gtsruflgdr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yangfankeji.com/gtdmayrhmw.html

[T11] Kotlin：协程
来源：http://hz.yj202588.top/gtntaafnzr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.tianlin.xyz/gtvonwszqf.html

[T12] Kotlin：解构声明
来源：http://hz.shangyingyoupin.top/gtdzdwnvem.html

val (a, b) = Pair(1, 2)
来源：http://hz.zhiwuduotai.top/gtzvxfobzr.html

[T13] Kotlin：只读 Map
来源：http://hz.yj20258888.top/gtfjlliecq.html

val m = mapOf("a" to 1)
来源：http://hz.tianlin.xyz/gtetrearwe.html

[T14] Kotlin：循环
来源：http://hz.jyoumei.cn/gtsgtkwumn.html

for (i in 1..10) println(i)
来源：http://hz.shuidangran.top/gtnmqyjijd.html

[T15] Kotlin：接口
来源：http://hz.yj20258.top/gtqadmmkhm.html

interface Shape { fun area(): Double }
来源：http://hz.shzxlz.cn/gtpovxxwdh.html

[T16] Swift：Hello World
来源：http://hz.ppjwa.cn/gtuxbqaqns.html

print("Hello")
来源：http://hz.shzxlz.cn/gtasggefjo.html

[T17] Swift：变量与常量
来源：http://hz.zhixingplan.top/gtrzkrjyyo.html

var a = 1;  let b = 2
来源：http://hz.jianghu66.top/gtixdgfuox.html

[T18] Swift：字符串插值
来源：http://hz.daxiang520.top/gtocetyjiq.html

"值: \(b)"
来源：http://hz.aizwys.cn/gtxrhmvbef.html

[T19] Swift：可选绑定
来源：http://hz.haohaochexian.top/gtxgxkpuvk.html

if let n = opt { print(n) }
来源：http://hz.snrcjt.cn/gthhabikkw.html

[T20] Swift：数组操作
来源：http://hz.pycfn.com/gthxmrkfxu.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.xingfuxueyuan.xyz/gtxwvcvnau.html

[T21] Swift：遍历
来源：http://hz.tanke756.top/gtvcrcymkt.html

for x in a { print(x) }
来源：http://hz.chenlongwang.top/gtobsuuchy.html

[T22] Swift：字典
来源：http://hz.jqgufenzy.top/gtdgjolfew.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.svipenyu.cn/gteuqnvood.html

[T23] Swift：函数
来源：http://hz.9152youxi.cn/gtlwwevtgb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jqgfzy.top/gtqnlmmzbx.html

[T24] Swift：闭包
来源：http://hz.316326.xyz/gtsojjxjsy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yueranfly.top/gthqjfnjmi.html

[T25] Swift：结构体
来源：http://hz.xziqi.cn/gtfrzypxpe.html

struct P { var x: Int }
来源：http://hz.zhoulong.xyz/gtinbwoyyu.html

[T26] Swift：类与重写
来源：http://hz.wangdashe.top/gtxieyqxni.html

class A: Base { override func f() {} }
来源：http://hz.jinghuilouyu.cn/gthkfjzfpr.html

[T27] Swift：错误处理
来源：http://hz.jqgfzy.top/gtnwbljgjy.html

do { try f() } catch { print(error) }
来源：http://hz.yj202588.top/gtpanusgva.html

[T28] Swift：枚举
来源：http://hz.tanke756.top/gtffwakhai.html

enum Color { case red, green }
来源：http://hz.zhongyouzk.top/gtxvlbxbro.html

[T29] Swift：guard 提前返回
来源：http://hz.quarkkingdee.top/gtfapqeykb.html

guard let x = opt else { return }
来源：http://hz.zhengqikj.top/gtqpwecopd.html

[T30] Swift：协议
来源：http://hz.yuxming.cn/gtyiyksjfo.html

protocol Shape { func area() -> Double }
来源：http://hz.xinyue.icu/gtufciwded.html

[T31] Lua：Hello World
来源：http://hz.smart0.xyz/gttfctokny.html

print("Hello")
来源：http://hz.quarkkingdee.top/gtrtyzhhke.html

[T32] Lua：局部变量
来源：http://hz.yj202588.top/gtluuilzro.html

local a = 1
来源：http://hz.zhixingplan.top/gtahcvtiff.html

[T33] Lua：表（数组）
来源：http://hz.hammf.cn/gttdgabwoy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.xylfe.cn/gtxfkzxzbo.html

[T34] Lua：遍历表
来源：http://hz.iojbl.cn/gtgobbuymy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.kuanghao11.cn/gtzbafbbqh.html

[T35] Lua：字典表
来源：http://hz.316326.xyz/gtxejquiaj.html

local d = { a = 1 };  d.b = 2
来源：http://hz.sxryk.cn/gtfaifczgp.html

[T36] Lua：函数
来源：http://hz.gogol.net.cn/gtkluqbvbl.html

function add(a, b) return a + b end
来源：http://hz.ydjk.org.cn/gtrggqiabx.html

[T37] Lua：字符串拼接
来源：http://hz.vqdsnc.cn/gtgkdhomnz.html

"a" .. "b"
来源：http://hz.shzxlz.cn/gtakffpgga.html

[T38] Lua：条件
来源：http://hz.yj202588.top/gtzyokqgol.html

if x > 0 then print("正") end
来源：http://hz.andypj.xyz/gtibbtxiwk.html

[T39] Lua：模式匹配
来源：http://hz.dianchejie.cn/gtlbjwrpxn.html

string.find(s, "%d+")
来源：http://hz.sufxvd.cn/gtklqivtlr.html

[T40] Lua：元表
来源：http://hz.sweek.top/gtvhuykgwc.html

setmetatable({}, { __index = base })
来源：http://hz.dashuyun.cn/gthrtxvoep.html

[T41] Perl：Hello World
来源：http://hz.tianlin.xyz/gtbrzvidzq.html

print "Hello\n";
来源：http://hz.shanyushiyangtech.top/gtdeiielmr.html

[T42] Perl：变量类型
来源：http://hz.xylfe.cn/gtvavbxuds.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.gaohongyu789.top/gtufsanzya.html

[T43] Perl：字符串插值
来源：http://hz.xuetiantiany.cn/gttgzwitiw.html

"值: $a"
来源：http://hz.guowangkeji.top/gterkyawtd.html

[T44] Perl：条件
来源：http://hz.jinqigufen.top/gtlrfmthfc.html

if ($a > 0) { print "正"; }
来源：http://hz.andypj.xyz/gtvqahvgda.html

[T45] Perl：数组遍历
来源：http://hz.zhiwuduotai.top/gtdepurpot.html

for my $x (@arr) { print $x; }
来源：http://hz.yongpay.top/gthyizxopv.html

[T46] Perl：哈希操作
来源：http://hz.zhixingplan.top/gtoejxsgly.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.hfpthk.cn/gttmobgscz.html

[T47] Perl：正则捕获
来源：http://hz.mhx1999.top/gtgxtdllye.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.zycfv.cn/gtdmdmkukf.html

[T48] Perl：正则替换
来源：http://hz.sxryk.cn/gtwimtlick.html

$s =~ s/old/new/g;
来源：http://hz.jinghuilouyu.cn/gtdmztnnfl.html

[T49] Perl：函数
来源：http://hz.cqqwz.cn/gtykmepyye.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jlsjyb.cn/gtqvjigtjf.html

[T50] Perl：逐行读文件
来源：http://hz.snrcjt.cn/gtgjtaikqf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.sweek.top/gtjfkuaozl.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jinqigfzy.top/gthcvcllgq.html

[T51] Scala：Hello World
来源：http://hz.shuidangran.top/gtejdceohw.html

println("Hello")
来源：http://hz.zhijiandao.cn/gtvchnmubc.html

[T52] Scala：变量
来源：http://hz.zhiwuduotai.top/gttqcovulb.html

val a = 1;  var b = 2
来源：http://hz.zhijiandao.cn/gtnrqubzsg.html

[T53] Scala：字符串插值
来源：http://hz.shuidangran.top/gtxooluhes.html

s"值: $b"
来源：http://hz.zhoulong.xyz/gtyjgxkdxb.html

[T54] Scala：集合映射
来源：http://hz.sysykeji.top/gtojxovjoo.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.jinqigfzy.top/gtlbowynco.html

[T55] Scala：集合过滤
来源：http://hz.nanxinkj.top/gtabeahidh.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.tanke756.top/gtoxvcfegv.html

[T56] Scala：样例类
来源：http://hz.xziqi.cn/gtisabmlzj.html

case class User(name: String, age: Int)
来源：http://hz.quarkkingdee.top/gtrqaazchf.html

[T57] Scala：模式匹配
来源：http://hz.52xcode.cn/gtzbvltpdn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.ywan-chungtsiang.top/gtezqdftxo.html

[T58] Scala：函数定义
来源：http://hz.yj202588.top/gthpyxgyaw.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.xuetiantiany.cn/gtipxhlilt.html

[T59] Scala：循环
来源：http://hz.sysykeji.top/gtgpancrvh.html

for (i <- 1 to 10) println(i)
来源：http://hz.hammf.cn/gtayhoyjxk.html

[T60] Scala：折叠
来源：http://hz.pycfn.com/gthowyhuzj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.cheryme.top/gtlwcblzlg.html

================================================================================
来源：http://hz.zhijiandao.cn/gtqrmbgoys.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yanxiufei.cn/gtqjiovnta.html

================================================================================
来源：http://hz.cheryme.top/gtrtruxuvv.html

[U01] Py：创建虚拟环境
来源：http://hz.guannengcc.top/gtfpihqppz.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yongpay.top/gtoniqjsaf.html

[U02] Py：导出 / 安装依赖
来源：http://hz.sxryk.cn/gthwvsehmk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yuanzhike.top/gtneqsglsc.html

[U03] Py：加载 .env 配置
来源：http://hz.jyoumei.cn/gtcxljbrap.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.nwbrower.top/gtauliqsgf.html

[U04] Py：变量调试打印
来源：http://hz.hammf.cn/gtgfvtyoan.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.meibo888.top/gtnphmkzwl.html

[U05] Py：列表去重且保序
来源：http://hz.yangfankeji.com/gtehdfwcnv.html

list(dict.fromkeys(arr))
来源：http://hz.birdmap.top/gtqzxrywke.html

[U06] Py：合并两个字典
来源：http://hz.pengpengdd.cyou/gtktfkehcq.html

{**a, **b}
来源：http://hz.ppjwa.cn/gtaxpbotkm.html

[U07] Py：反转字典键值
来源：http://hz.ydzc1.top/gtuleypzic.html

{v: k for k, v in d.items()}
来源：http://hz.jqgufenzy.top/gttncjmlwi.html

[U08] Py：展平二维列表
来源：http://hz.shanyushiyangkeji.top/gtdmjfomvc.html

[y for x in nested for y in x]
来源：http://hz.bjfxy.top/gtqpmbvtyk.html

[U09] Py：字典取最大值的键
来源：http://hz.andypj.xyz/gtsndrxlji.html

max(d, key=d.get)
来源：http://hz.zhijiandao.cn/gtwvimikrx.html

[U10] Py：按值排序字典
来源：http://hz.nanxinkj.top/gtyehfidwp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.jqgfzy.top/gtatosmtxp.html

[U11] Py：生成器表达式
来源：http://hz.dianchejie.cn/gtcfdawfgj.html

(x * 2 for x in arr)
来源：http://hz.nanxuanxn.top/gtgazlflpw.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.fengsongda.top/gtwkdosibv.html

Counter(arr).most_common(3)
来源：http://hz.meibo888.top/gtytdtgmsb.html

[U13] Py：固定长度队列
来源：http://hz.nwbrower.top/gttuooaarm.html

deque(maxlen=10)
来源：http://hz.sufxvd.cn/gtzokwhywh.html

[U14] Py：分组收集到列表
来源：http://hz.kuanghao11.cn/gtquekkqwh.html

defaultdict(list)
来源：http://hz.jinyuanbaomall.cn/gtfrmgzogu.html

[U15] Py：高精度计时
来源：http://hz.guowangkeji.top/gtynrkfrdq.html

t = time.perf_counter()
来源：http://hz.cheryme.top/gtvsjuffkv.html

[U16] Py：命令行参数解析
来源：http://hz.redwolf501.top/gtpgdautue.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.hnqzz.top/gtjptkcxyo.html

[U17] Py：初始化日志
来源：http://hz.aizwys.cn/gtxsvnhrct.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.kuanghao11.cn/gtneldgtsx.html

[U18] Py：预编译正则
来源：http://hz.jqgfzy.top/gthtydfroe.html

pat = re.compile(r"\d+")
来源：http://hz.zhengqikj.top/gtxxaznavq.html

[U19] Py：正则替换带回调
来源：http://hz.hnqzz.top/gtjedsspaz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.aibaodan.cn/gtocsztcnn.html

[U20] Py：缓存函数结果
来源：http://hz.jlsjyb.cn/gtmqdksatv.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jyoumei.cn/gtvkvxvdwl.html

[U21] Py：自定义上下文管理器
来源：http://hz.yueranfly.top/gtqkrnfkov.html

@contextlib.contextmanager
来源：http://hz.tanke756.top/gtryxtrblg.html

[U22] Py：矩阵转置
来源：http://hz.shanyushiyangkeji.top/gtftckeiwx.html

list(zip(*m))
来源：http://hz.mhx1999.top/gtnmikgqcs.html

[U23] Py：分块读取大文件
来源：http://hz.sxryk.cn/gtdfpusunu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.chenzaomai.com/gthrhctnkz.html

[U24] Py：路径操作
来源：http://hz.xziqi.cn/gtaidknolo.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.ivvv.top/gtytmvqkxn.html

[U25] Py：CSV 按字典读
来源：http://hz.jyoumei.cn/gtvrjctejp.html

csv.DictReader(f)
来源：http://hz.bjfxy.top/gtmryvrpie.html

[U26] Py：并发下载
来源：http://hz.0kj1m.cn/gtsczyklxn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.hnxiangtu.top/gtcfkxmifv.html

[U27] Py：异步 HTTP
来源：http://hz.ydzc1.top/gtdcemaqai.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.wangshuangyany.cn/gtdijkxtgn.html

[U28] Py：类型别名
来源：http://hz.gotoacloud.top/gtuozzbpiz.html

UserId = int
来源：http://hz.nanxuanxn.top/gtfqnzxeru.html

[U29] Py：属性校验
来源：http://hz.yj20258.top/gtximrsjik.html

@property 与 @x.setter 配合
来源：http://hz.9152youxi.cn/gtzbtzbsfl.html

[U30] Py：数据类
来源：http://hz.hywenlv.cn/gthpxkvvkg.html

@dataclass(slots=True)
来源：http://hz.ehwqpu.com/gtrjcrclbf.html


<!-- 参考信息 -->