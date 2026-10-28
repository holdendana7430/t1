代发 wailian999

int main(int argc, char **argv)
来源：http://hz.snrcjt.cn/gtmneamott.html

[S19] C：快速排序
来源：http://hz.tian-w.cn/gtfgawmark.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yj20258888.top/gtxvgngikn.html

[S20] C：二分查找
来源：http://hz.ivvv.top/gteekmjsvq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.316326.xyz/gthbrioahw.html

[S21] C：字符类别判断
来源：http://hz.kuanghao11.cn/gtktuxyztu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hnxiangtu.top/gtqnxybkex.html

[S22] C：字符串转数字
来源：http://hz.xylfe.cn/gtwwzbfktb.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.svipenyu.cn/gtepzhycyf.html

[S23] C：随机数
来源：http://hz.kuanghao11.cn/gtdcwxamwj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.nanxuanxn.top/gtaxvrvivl.html

[S24] C：获取本地时间
来源：http://hz.haohaochexian.top/gtwypbnnnu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.9152youxi.cn/gtjfmjbcmh.html

[S25] C：内存拷贝
来源：http://hz.tian-w.cn/gtjlomntfp.html

memcpy(dst, src, n);
来源：http://hz.gogol.net.cn/gtvxpqslzo.html

[S26] C：内存清零
来源：http://hz.zdqjudy.top/gtretkjisw.html

memset(a, 0, sizeof a);
来源：http://hz.tanke756.top/gtxvcyucvd.html

[S27] C：定义常量
来源：http://hz.xingfuxueyuan.xyz/gtzothklhr.html

const double PI = 3.14159;
来源：http://hz.yuanzhike.top/gtnncfublz.html

[S28] C：静态变量
来源：http://hz.jinqigufen.top/gtitqsncfr.html

static int counter = 0;
来源：http://hz.redwolf501.top/gtcmqrokwy.html

[S29] C：变参函数
来源：http://hz.yueranfly.top/gtmdtfmcvt.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.pengpengdd.cyou/gtkqirwbqw.html

[S30] C：头文件保护
来源：http://hz.cqqwz.cn/gtbudgphlg.html

#ifndef X_H
来源：http://hz.ivvv.top/gtxwphwktt.html

#define X_H
来源：http://hz.jinqigfzy.top/gtcizrafok.html

#endif
来源：http://hz.gotoacloud.top/gtoywehtns.html

[S31] C++：Hello World
来源：http://hz.ivvv.top/gtnmelqfbq.html

#include <iostream>
来源：http://hz.snrcjt.cn/gtioyhomoa.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yvedp.cn/gtwrqdjxfu.html

[S32] C++：字符串
来源：http://hz.jianghu66.top/gtteepsczm.html

std::string s = "hi";  s += "!";
来源：http://hz.cucudq.cn/gtoehjpknt.html

[S33] C++：vector 增删
来源：http://hz.yvedp.cn/gtgsvylyuy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zdqjudy.top/gtbrgbrliz.html

[S34] C++：遍历 vector
来源：http://hz.pycfn.com/gtuucyfqdy.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xingfuxueyuan.xyz/gtzaontosu.html

[S35] C++：map
来源：http://hz.fengsongda.top/gtxeeukwfh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gzhubu.top/gtqojfzzij.html

[S36] C++：unordered_map
来源：http://hz.fzhhl.top/gtgqtgocbb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sweek.top/gtjiyywzzg.html

[S37] C++：set
来源：http://hz.haohaochexian.top/gtetkheele.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yueranfly.top/gtkxwvlsmb.html

[S38] C++：排序
来源：http://hz.jyoumei.cn/gtwwaxblwv.html

std::sort(v.begin(), v.end());
来源：http://hz.chenzaomai.com/gtfaherelg.html

[S39] C++：自定义比较器排序
来源：http://hz.hywenlv.cn/gtxzqhiaam.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.xziqi.cn/gtfffjknou.html

[S40] C++：查找元素
来源：http://hz.zhengqikj.top/gtdpypjgnc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hysaishi.cn/gtcgseknln.html

[S41] C++：类与构造函数
来源：http://hz.smart0.xyz/gtiizevhwq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.wangdashe.top/gttwohfpkr.html

[S42] C++：继承与虚函数
来源：http://hz.sxryk.cn/gtwlyeiywd.html

class B : public Base { public: void f() override {} };
来源：http://hz.birdmap.top/gtclwebvky.html

[S43] C++：智能指针
来源：http://hz.gzhubu.top/gtwozotjel.html

auto p = std::make_unique<int>(5);
来源：http://hz.tanke756.top/gtpgnjdijh.html

[S44] C++：引用传参
来源：http://hz.0kj1m.cn/gtltxpwcgb.html

void inc(int &x) { ++x; }
来源：http://hz.ydjk.org.cn/gtukmcpxvz.html

[S45] C++：lambda
来源：http://hz.hnxiangtu.top/gtwsepckqc.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ywan-chungtsiang.top/gtsnoaohqd.html

[S46] C++：函数模板
来源：http://hz.fengsongda.top/gtahfjoipa.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.sxryk.cn/gtjirbeksi.html

[S47] C++：结构化绑定遍历
来源：http://hz.feifeiyinyue.top/gtqsdkcdcm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.wangdashe.top/gtoachgwvr.html

[S48] C++：逐行读文件
来源：http://hz.nanxinkj.top/gtzzlvxihl.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.sysykeji.top/gtujwkyqdq.html

while (std::getline(in, line)) { }
来源：http://hz.birdmap.top/gthcinlemn.html

[S49] C++：写文件
来源：http://hz.sysykeji.top/gtnikhnggl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jinqigufen.top/gtwtdlzdyp.html

[S50] C++：格式化数字
来源：http://hz.dianchejie.cn/gtwzvyllwb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.tian-w.cn/gtysdwwrwe.html

[S51] C++：显式类型转换
来源：http://hz.hysaishi.cn/gtgksngrja.html

static_cast<double>(a) / b
来源：http://hz.aibaodan.cn/gtnulnuxuy.html

[S52] C++：const 与 noexcept
来源：http://hz.yj202588.top/gtquasuooa.html

int size() const noexcept { return n_; }
来源：http://hz.ywan-chungtsiang.top/gtdxfdxkyg.html

[S53] C++：移动语义
来源：http://hz.birdmap.top/gtdmrobzqe.html

std::vector<int> w = std::move(v);
来源：http://hz.shanyushiyangtech.top/gtnnrjikue.html

[S54] C++：异常处理
来源：http://hz.ehwqpu.com/gttisufdby.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ehwqpu.com/gtqoypkvui.html

[S55] C++：结构化绑定
来源：http://hz.yuxming.cn/gtrssmbqrk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.nanxuanxn.top/gtvnqrxupc.html

[S56] C++：optional
来源：http://hz.yj202588.top/gtsdpelfqi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.andypj.xyz/gtftysbmlt.html

[S57] C++：编译期常量
来源：http://hz.xinyue.icu/gtjbhgvtej.html

constexpr int N = 10;
来源：http://hz.jyoumei.cn/gtsipokmbc.html

[S58] C++：命名空间
来源：http://hz.gotoacloud.top/gtvukakbdi.html

namespace ns { int f() { return 1; } }
来源：http://hz.jqgufenzy.top/gtnkpuszec.html

[S59] C++：静态断言
来源：http://hz.mhx1999.top/gtdympnedx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.svipenyu.cn/gtwyflpkfj.html

[S60] C++：遍历并删除元素
来源：http://hz.aibaodan.cn/gtofovfqri.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yuxming.cn/gtdhevscmv.html

================================================================================
来源：http://hz.hammf.cn/gtbbloyunp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jinqigufen.top/gtsrqmjsbx.html

================================================================================
来源：http://hz.haohaochexian.top/gtfucomnyw.html

[T01] Kotlin：Hello World
来源：http://hz.cheryme.top/gtvgamdjjz.html

println("Hello")
来源：http://hz.jinqigufen.top/gtxjehbirh.html

[T02] Kotlin：变量
来源：http://hz.bjfxy.top/gtfmcipzsq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.daria6918.cn/gtxsrshguj.html

[T03] Kotlin：字符串模板
来源：http://hz.ivvv.top/gttsjlnelg.html

"值: $b"
来源：http://hz.jinyuanbaomall.cn/gtdnvsveoi.html

[T04] Kotlin：空安全
来源：http://hz.zhengqikj.top/gtxjnxizor.html

val n: String? = null;  n?.length
来源：http://hz.xuanzx.com/gtpuaptxoa.html

[T05] Kotlin：when 表达式
来源：http://hz.chenjidiqi.icu/gtzhjhqbuq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ydzc1.top/gtdolpawuu.html

[T06] Kotlin：集合映射
来源：http://hz.52xcode.cn/gtqcvwkxnw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.nanxinkj.top/gthgkoocyv.html

[T07] Kotlin：集合过滤
来源：http://hz.52xcode.cn/gtsuyhzcqr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.cheryme.top/gthgnpdeue.html

[T08] Kotlin：数据类
来源：http://hz.haohaochexian.top/gtqubxieql.html

data class User(val name: String, val age: Int)
来源：http://hz.pengpengdd.cyou/gtuijvyjhl.html

[T09] Kotlin：扩展函数
来源：http://hz.meibo888.top/gtjzuzkocw.html

fun String.exclaim() = this + "!"
来源：http://hz.ivvv.top/gteuetvbdm.html

[T10] Kotlin：默认参数
来源：http://hz.hongshengwenyu.top/gtqcnghbid.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jqgufenzy.top/gtcymyrepc.html

[T11] Kotlin：协程
来源：http://hz.gotoacloud.top/gtysauzjrm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.shangyingyoupin.top/gtguuxypgj.html

[T12] Kotlin：解构声明
来源：http://hz.tian-w.cn/gtbufshltm.html

val (a, b) = Pair(1, 2)
来源：http://hz.yj20258888.top/gtnqzgnoru.html

[T13] Kotlin：只读 Map
来源：http://hz.shuidangran.top/gtvuinpkze.html

val m = mapOf("a" to 1)
来源：http://hz.gaohongyu789.top/gtasjekear.html

[T14] Kotlin：循环
来源：http://hz.yueranfly.top/gtswmbdiue.html

for (i in 1..10) println(i)
来源：http://hz.ydjk.org.cn/gtygazjeph.html

[T15] Kotlin：接口
来源：http://hz.ivvv.top/gtcvkvzdlt.html

interface Shape { fun area(): Double }
来源：http://hz.jiagoushi.top/gtuxhyqboq.html

[T16] Swift：Hello World
来源：http://hz.haohaochexian.top/gtdvzsjqoz.html

print("Hello")
来源：http://hz.guowangkeji.top/gtsjebqkbj.html

[T17] Swift：变量与常量
来源：http://hz.ywan-chungtsiang.top/gtvwvyffqh.html

var a = 1;  let b = 2
来源：http://hz.snrcjt.cn/gtvsfsldmo.html

[T18] Swift：字符串插值
来源：http://hz.c1oappe.top/gtfuskvnze.html

"值: \(b)"
来源：http://hz.yvedp.cn/gtctkgmqrh.html

[T19] Swift：可选绑定
来源：http://hz.andypj.xyz/gtiqrxrmsh.html

if let n = opt { print(n) }
来源：http://hz.yueranfly.top/gtqipygmxk.html

[T20] Swift：数组操作
来源：http://hz.sysykeji.top/gtmhwuaazh.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.birdmap.top/gtoyqzessh.html

[T21] Swift：遍历
来源：http://hz.vqdsnc.cn/gtotpruvdx.html

for x in a { print(x) }
来源：http://hz.jinqigfzy.top/gtlwkipykc.html

[T22] Swift：字典
来源：http://hz.vqdsnc.cn/gtlpaynehu.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yueranfly.top/gtbqzyegfa.html

[T23] Swift：函数
来源：http://hz.gogol.net.cn/gtbnvpovev.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.hywenlv.cn/gtjhhibjza.html

[T24] Swift：闭包
来源：http://hz.nwbrower.top/gtqvideimo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.gogol.net.cn/gtffxnvoyk.html

[T25] Swift：结构体
来源：http://hz.tianlin.xyz/gthhltbdgo.html

struct P { var x: Int }
来源：http://hz.hysaishi.cn/gtqmurmytz.html

[T26] Swift：类与重写
来源：http://hz.zhixingplan.top/gtvrdgyecd.html

class A: Base { override func f() {} }
来源：http://hz.bjfxy.top/gttyvowgyk.html

[T27] Swift：错误处理
来源：http://hz.ywan-chungtsiang.top/gtudebcjza.html

do { try f() } catch { print(error) }
来源：http://hz.ivvv.top/gtfcwillol.html

[T28] Swift：枚举
来源：http://hz.yj202588.top/gtoilhttpy.html

enum Color { case red, green }
来源：http://hz.zhengqikj.top/gtzmljwoux.html

[T29] Swift：guard 提前返回
来源：http://hz.kuanghao11.cn/gttijmlazn.html

guard let x = opt else { return }
来源：http://hz.wangshuangyany.cn/gtjjuzrojo.html

[T30] Swift：协议
来源：http://hz.jlsjyb.cn/gtwdflplnd.html

protocol Shape { func area() -> Double }
来源：http://hz.aibaodan.cn/gtyoeiabvi.html

[T31] Lua：Hello World
来源：http://hz.hnxiangtu.top/gtkqzmbtzr.html

print("Hello")
来源：http://hz.0kj1m.cn/gtvzwahhzr.html

[T32] Lua：局部变量
来源：http://hz.xuanzx.com/gtjkjmkbsr.html

local a = 1
来源：http://hz.tianlin.xyz/gtplyjjtsh.html

[T33] Lua：表（数组）
来源：http://hz.nanxuanxn.top/gtmqvqwubf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.haohaochexian.top/gtbzyezixt.html

[T34] Lua：遍历表
来源：http://hz.fzhhl.top/gtljosofni.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.cdnleiting.top/gtjacpespb.html

[T35] Lua：字典表
来源：http://hz.jqgfzy.top/gtougtpnjn.html

local d = { a = 1 };  d.b = 2
来源：http://hz.gzhubu.top/gtqyzngyrn.html

[T36] Lua：函数
来源：http://hz.jinghuilouyu.cn/gtqbwmqlxq.html

function add(a, b) return a + b end
来源：http://hz.dianchejie.cn/gtyalhubwm.html

[T37] Lua：字符串拼接
来源：http://hz.guannengcc.top/gtghctfcwk.html

"a" .. "b"
来源：http://hz.ydjk.org.cn/gtpjuoksfz.html

[T38] Lua：条件
来源：http://hz.xingfuxueyuan.xyz/gtruzmcimp.html

if x > 0 then print("正") end
来源：http://hz.vqdsnc.cn/gtrsfqjzem.html

[T39] Lua：模式匹配
来源：http://hz.yuxming.cn/gtjoyipokr.html

string.find(s, "%d+")
来源：http://hz.zycfv.cn/gtytweujwa.html

[T40] Lua：元表
来源：http://hz.vqdsnc.cn/gtwulmgxfy.html

setmetatable({}, { __index = base })
来源：http://hz.jinghuilouyu.cn/gtpfdbprjd.html

[T41] Perl：Hello World
来源：http://hz.nwbrower.top/gtjistabzq.html

print "Hello\n";
来源：http://hz.yueranfly.top/gtdlsokhfd.html

[T42] Perl：变量类型
来源：http://hz.zhongyouzk.top/gtmcbedvho.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.feifeiyinyue.top/gtrqhxbbfc.html

[T43] Perl：字符串插值
来源：http://hz.yueranfly.top/gtlvqrdbnu.html

"值: $a"
来源：http://hz.jinyuanbaomall.cn/gtwrnhxrjw.html

[T44] Perl：条件
来源：http://hz.nanxinkj.top/gtkeuuqkyt.html

if ($a > 0) { print "正"; }
来源：http://hz.jqgufenzy.top/gtmbuiiuzy.html

[T45] Perl：数组遍历
来源：http://hz.yongpay.top/gtxcwjqbrh.html

for my $x (@arr) { print $x; }
来源：http://hz.wangdashe.top/gtdxihkwnn.html

[T46] Perl：哈希操作
来源：http://hz.zhengqikj.top/gtmitbszyw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.hysaishi.cn/gtsbjgllpd.html

[T47] Perl：正则捕获
来源：http://hz.meibo888.top/gtynjlxmjf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yanxiufei.cn/gtbvrtdcbb.html

[T48] Perl：正则替换
来源：http://hz.daxiang520.top/gtsfwzboay.html

$s =~ s/old/new/g;
来源：http://hz.jiagoushi.top/gthxuwudyy.html

[T49] Perl：函数
来源：http://hz.cheryme.top/gtgdhtiwge.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.bjfxy.top/gtliojpetb.html

[T50] Perl：逐行读文件
来源：http://hz.aizwys.cn/gtfytpuwdw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.zhixingplan.top/gtarattdat.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.meibo888.top/gtbyvkfher.html

[T51] Scala：Hello World
来源：http://hz.guannengcc.top/gtigucjled.html

println("Hello")
来源：http://hz.havefunace.top/gtqpqbshyx.html

[T52] Scala：变量
来源：http://hz.jianghu66.top/gteqxriphb.html

val a = 1;  var b = 2
来源：http://hz.zhaomingkeji.xyz/gtckzyfcxe.html

[T53] Scala：字符串插值
来源：http://hz.chenlongwang.top/gtuhnsenxj.html

s"值: $b"
来源：http://hz.vqdsnc.cn/gtusloctmi.html

[T54] Scala：集合映射
来源：http://hz.xuanzx.com/gthfuctbhr.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.smart0.xyz/gtofvmuina.html

[T55] Scala：集合过滤
来源：http://hz.chenjidiqi.icu/gtqbyktsiv.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.pycfn.com/gtbuksahvo.html

[T56] Scala：样例类
来源：http://hz.shangyingyoupin.top/gtgcprbffp.html

case class User(name: String, age: Int)
来源：http://hz.hongshengwenyu.top/gtfqdulult.html

[T57] Scala：模式匹配
来源：http://hz.aizwys.cn/gtrdwatwou.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zhiwuduotai.top/gtbxqtptin.html

[T58] Scala：函数定义
来源：http://hz.zhixingplan.top/gtxuaqzshz.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.9152youxi.cn/gtgepyhbpq.html

[T59] Scala：循环
来源：http://hz.sweek.top/gtijnionza.html

for (i <- 1 to 10) println(i)
来源：http://hz.zhengqikj.top/gtshgppxqf.html

[T60] Scala：折叠
来源：http://hz.birdmap.top/gtvwvpampv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.zhixingplan.top/gtakllidba.html

================================================================================
来源：http://hz.hammf.cn/gtckoldnxx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.wangdashe.top/gtadunvofn.html

================================================================================
来源：http://hz.yvedp.cn/gtspkkxszm.html

[U01] Py：创建虚拟环境
来源：http://hz.fengsongda.top/gtyzknsvbu.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.sufxvd.cn/gtrhaxddtx.html

[U02] Py：导出 / 安装依赖
来源：http://hz.yongpay.top/gtxxyufuay.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.ydjk.org.cn/gtyoeizhaj.html

[U03] Py：加载 .env 配置
来源：http://hz.zhengqikj.top/gttwcekpfx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.shzxlz.cn/gtxnfohivk.html

[U04] Py：变量调试打印
来源：http://hz.0kj1m.cn/gtnppsjdco.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.0kj1m.cn/gtlywzszak.html

[U05] Py：列表去重且保序
来源：http://hz.nwbrower.top/gtancjzrew.html

list(dict.fromkeys(arr))
来源：http://hz.yuxming.cn/gtehhyrxjy.html

[U06] Py：合并两个字典
来源：http://hz.xingfuxueyuan.xyz/gtzeoygvwv.html

{**a, **b}
来源：http://hz.bjfxy.top/gtxntdqomk.html

[U07] Py：反转字典键值
来源：http://hz.zhoulong.xyz/gttqiljchl.html

{v: k for k, v in d.items()}
来源：http://hz.ywan-chungtsiang.top/gtlppxqeej.html

[U08] Py：展平二维列表
来源：http://hz.guowangkeji.top/gtbrefvecw.html

[y for x in nested for y in x]
来源：http://hz.xuanzx.com/gtrgniqdda.html

[U09] Py：字典取最大值的键
来源：http://hz.daria6918.cn/gtgwtkieus.html

max(d, key=d.get)
来源：http://hz.quarkkingdee.top/gtnqxxvgtb.html

[U10] Py：按值排序字典
来源：http://hz.cucudq.cn/gtiyhoatmu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.316326.xyz/gtmfuyhwgm.html

[U11] Py：生成器表达式
来源：http://hz.redwolf501.top/gtdjbsgtir.html

(x * 2 for x in arr)
来源：http://hz.cheryme.top/gtkkitotyr.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.haohaochexian.top/gtjlrpwivq.html

Counter(arr).most_common(3)
来源：http://hz.cdnleiting.top/gthmspumsk.html

[U13] Py：固定长度队列
来源：http://hz.ppjwa.cn/gtbcxctrod.html

deque(maxlen=10)
来源：http://hz.tian-w.cn/gtlvekxmrl.html

[U14] Py：分组收集到列表
来源：http://hz.ppjwa.cn/gtsivccafi.html

defaultdict(list)
来源：http://hz.sweek.top/gtdhqaqyfa.html

[U15] Py：高精度计时
来源：http://hz.cucudq.cn/gtwrolucyd.html

t = time.perf_counter()
来源：http://hz.316326.xyz/gthusphhwg.html

[U16] Py：命令行参数解析
来源：http://hz.jianghu66.top/gtlclsjong.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jinghuilouyu.cn/gtttebtnyw.html

[U17] Py：初始化日志
来源：http://hz.vqdsnc.cn/gtuzwzgmkz.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.andypj.xyz/gtszlvcozv.html

[U18] Py：预编译正则
来源：http://hz.shzxlz.cn/gtdsedppbk.html

pat = re.compile(r"\d+")
来源：http://hz.haohaochexian.top/gtmxfpelbj.html

[U19] Py：正则替换带回调
来源：http://hz.hammf.cn/gttnhtnlvj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.jyoumei.cn/gtyaxiesbc.html

[U20] Py：缓存函数结果
来源：http://hz.cashguo.top/gtehzacrmu.html

@functools.lru_cache(maxsize=None)
来源：http://hz.gzhubu.top/gtkadrdvzb.html

[U21] Py：自定义上下文管理器
来源：http://hz.pengpengdd.cyou/gtjisfkqts.html

@contextlib.contextmanager
来源：http://hz.ywan-chungtsiang.top/gtnfgxxfjk.html

[U22] Py：矩阵转置
来源：http://hz.tian-w.cn/gtxhhvikzz.html

list(zip(*m))
来源：http://hz.zhaomingkeji.xyz/gtucuxhczv.html

[U23] Py：分块读取大文件
来源：http://hz.sysykeji.top/gttzxmijfk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.tianlin.xyz/gtnlmraiaq.html

[U24] Py：路径操作
来源：http://hz.hywenlv.cn/gtfqxbudfh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.jqgufenzy.top/gtndipmtxu.html

[U25] Py：CSV 按字典读
来源：http://hz.sufxvd.cn/gtplnsnknu.html

csv.DictReader(f)
来源：http://hz.tian-w.cn/gtruwmsmsj.html

[U26] Py：并发下载
来源：http://hz.andypj.xyz/gtxkrstbym.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.quarkkingdee.top/gtjygtjqzh.html

[U27] Py：异步 HTTP
来源：http://hz.tianlin.xyz/gtuhqtomse.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.zhixingplan.top/gtrtmipvug.html

[U28] Py：类型别名
来源：http://hz.zhoulong.xyz/gtdmsyenbw.html

UserId = int
来源：http://hz.aibaodan.cn/gtlilnvkol.html

[U29] Py：属性校验
来源：http://hz.mhx1999.top/gtxkenarei.html

@property 与 @x.setter 配合
来源：http://hz.ywan-chungtsiang.top/gtfcgrdgsl.html

[U30] Py：数据类
来源：http://hz.ppjwa.cn/gtkavisimi.html

@dataclass(slots=True)
来源：http://hz.nanxinkj.top/gtdhvpsgnp.html

[U31] Py：单测
来源：http://hz.jinghuilouyu.cn/gthwzvzdwd.html

python -m pytest -q
来源：http://hz.haohaochexian.top/gtilbpnage.html

[U32] Py：代码格式化
来源：http://hz.316326.xyz/gttpryhkxy.html

ruff format . && ruff check --fix .
来源：http://hz.smart0.xyz/gtbgwvntxc.html

[U33] Py：打包发布
来源：http://hz.pengpengdd.cyou/gtkgahevjw.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.jlsjyb.cn/gtcklzphsy.html

[U34] Py：判断编码
来源：http://hz.hfpthk.cn/gtvixszjwq.html

chardet.detect(raw)
来源：http://hz.daria6918.cn/gtfvmvrokm.html

[U35] Py：发送邮件
来源：http://hz.tian-w.cn/gtjcdtajmu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.zycfv.cn/gtmgpzsipv.html

[U36] Py：定时任务
来源：http://hz.shanyushiyangtech.top/gtthaalcgm.html

schedule.every(10).minutes.do(job)
来源：http://hz.xuetiantiany.cn/gtuqctvhyq.html

[U37] Py：读写 Excel
来源：http://hz.gzhubu.top/gtkqkohujv.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.haohaochexian.top/gteqxjhrpv.html

[U38] Py：获取脚本所在目录
来源：http://hz.guannengcc.top/gtqbcjupsk.html

Path(__file__).resolve().parent
来源：http://hz.vqdsnc.cn/gtmwwsimaa.html

[U39] Py：判断是否在交互环境
来源：http://hz.pengpengdd.cyou/gtnffychwn.html

sys.stdout.isatty()
来源：http://hz.feifeiyinyue.top/gtdawulygz.html

[U40] Py：打印到标准错误
来源：http://hz.gogol.net.cn/gtlttopnqb.html

print("err", file=sys.stderr)
来源：http://hz.ybcxt.top/gtuvmadahb.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.cqqwz.cn/gtazxutvjw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.zhixingplan.top/gtfplvfawv.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.ybcxt.top/gtpqetgcvp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.shuidangran.top/gtzdmspssc.html


<!-- 参考信息 -->