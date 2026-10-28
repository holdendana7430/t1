代发 wailian999

int main(int argc, char **argv)
来源：http://hz.hysaishi.cn/gtfocsgtbc.html

[S19] C：快速排序
来源：http://hz.hnxiangtu.top/gtfcmyporx.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.havefunace.top/gtjjvznoth.html

[S20] C：二分查找
来源：http://hz.9152youxi.cn/gtdghcgqrf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yvedp.cn/gtpthuiubu.html

[S21] C：字符类别判断
来源：http://hz.yj20258888.top/gtcnlqxvwn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.cheryme.top/gtwfpkwhwg.html

[S22] C：字符串转数字
来源：http://hz.yanxiufei.cn/gtuflikiwe.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yangfankeji.com/gtnlzibzrg.html

[S23] C：随机数
来源：http://hz.c1oappe.top/gtdvaorvmc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yongpay.top/gtriyzialg.html

[S24] C：获取本地时间
来源：http://hz.jyoumei.cn/gtlsrwxaje.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.dianchejie.cn/gtoeditjru.html

[S25] C：内存拷贝
来源：http://hz.gaohongyu789.top/gtnbvvhaxg.html

memcpy(dst, src, n);
来源：http://hz.hnqzz.top/gthvyvdykb.html

[S26] C：内存清零
来源：http://hz.xinyue.icu/gtwunbtjmx.html

memset(a, 0, sizeof a);
来源：http://hz.dianchejie.cn/gtbgxbogog.html

[S27] C：定义常量
来源：http://hz.0kj1m.cn/gtnzedysoy.html

const double PI = 3.14159;
来源：http://hz.jinqigfzy.top/gtsxmgmoav.html

[S28] C：静态变量
来源：http://hz.tianlin.xyz/gtfvaxktom.html

static int counter = 0;
来源：http://hz.hywenlv.cn/gtkpporlpy.html

[S29] C：变参函数
来源：http://hz.ehwqpu.com/gtcrwhnklb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hammf.cn/gthdsqrnxk.html

[S30] C：头文件保护
来源：http://hz.cqqwz.cn/gthuqveqlz.html

#ifndef X_H
来源：http://hz.guowangkeji.top/gtwkgzmwri.html

#define X_H
来源：http://hz.yanxiufei.cn/gtjxbmpihp.html

#endif
来源：http://hz.mhx1999.top/gtwqagmwnu.html

[S31] C++：Hello World
来源：http://hz.xuanzx.com/gtfmeyhtmi.html

#include <iostream>
来源：http://hz.birdmap.top/gtpqapssbe.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.9152youxi.cn/gtyohlvmue.html

[S32] C++：字符串
来源：http://hz.aibaodan.cn/gthwnimkhc.html

std::string s = "hi";  s += "!";
来源：http://hz.mhx1999.top/gtrfbxbxdh.html

[S33] C++：vector 增删
来源：http://hz.hysaishi.cn/gtjceygtik.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yueranfly.top/gtdxinnygr.html

[S34] C++：遍历 vector
来源：http://hz.yj20258888.top/gtjehpzljg.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.shangyingyoupin.top/gtrahxhena.html

[S35] C++：map
来源：http://hz.shanyushiyangtech.top/gtcaafqccl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ydzc1.top/gtcjbgjnyw.html

[S36] C++：unordered_map
来源：http://hz.shanyushiyangtech.top/gtqxhkhwzo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.svipenyu.cn/gtaqjafkni.html

[S37] C++：set
来源：http://hz.kuanghao11.cn/gtcmuibiaf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yanxiufei.cn/gtaqbedqcz.html

[S38] C++：排序
来源：http://hz.yongpay.top/gtzkwyicat.html

std::sort(v.begin(), v.end());
来源：http://hz.yuxming.cn/gtnbhdtbmi.html

[S39] C++：自定义比较器排序
来源：http://hz.jiagoushi.top/gtmxgfvbou.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.xziqi.cn/gtnpbugjtc.html

[S40] C++：查找元素
来源：http://hz.yongpay.top/gtwymfvkql.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.chenzaomai.com/gtboqlnste.html

[S41] C++：类与构造函数
来源：http://hz.ydjk.org.cn/gtpanwzjlk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xingfuxueyuan.xyz/gtodbrbxkn.html

[S42] C++：继承与虚函数
来源：http://hz.zhengqikj.top/gtotjtzuzn.html

class B : public Base { public: void f() override {} };
来源：http://hz.mhx1999.top/gtfubirjkz.html

[S43] C++：智能指针
来源：http://hz.yuxming.cn/gtszvoneff.html

auto p = std::make_unique<int>(5);
来源：http://hz.andypj.xyz/gtyzlkowah.html

[S44] C++：引用传参
来源：http://hz.9152youxi.cn/gtrbznptwv.html

void inc(int &x) { ++x; }
来源：http://hz.nanxuanxn.top/gtuazobnyi.html

[S45] C++：lambda
来源：http://hz.fzhhl.top/gtmrghrsou.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.guannengcc.top/gtiqrdweoy.html

[S46] C++：函数模板
来源：http://hz.cashguo.top/gtcimaznwq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.dashuyun.cn/gtugokxgmo.html

[S47] C++：结构化绑定遍历
来源：http://hz.svipenyu.cn/gtkzuwfhyy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zycfv.cn/gteypairfj.html

[S48] C++：逐行读文件
来源：http://hz.shangyingyoupin.top/gtrznyfbfz.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zdqjudy.top/gtiuubaqmn.html

while (std::getline(in, line)) { }
来源：http://hz.ehwqpu.com/gteokytosr.html

[S49] C++：写文件
来源：http://hz.fzhhl.top/gtwydjjfzc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yuxming.cn/gtxhrbguge.html

[S50] C++：格式化数字
来源：http://hz.yj202588.top/gtknldhlyn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhixingplan.top/gtovhawfnx.html

[S51] C++：显式类型转换
来源：http://hz.aibaodan.cn/gtbecduaau.html

static_cast<double>(a) / b
来源：http://hz.snrcjt.cn/gtcizuhsyr.html

[S52] C++：const 与 noexcept
来源：http://hz.hnxiangtu.top/gtpdeqyous.html

int size() const noexcept { return n_; }
来源：http://hz.jqgfzy.top/gtngscavfp.html

[S53] C++：移动语义
来源：http://hz.zhijiandao.cn/gtgopqkacu.html

std::vector<int> w = std::move(v);
来源：http://hz.hnqzz.top/gtwaigeakh.html

[S54] C++：异常处理
来源：http://hz.yuanzhike.top/gttllecytd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.mhx1999.top/gticwbxppq.html

[S55] C++：结构化绑定
来源：http://hz.aizwys.cn/gtdlnoxfdz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.havefunace.top/gtwjoqaluu.html

[S56] C++：optional
来源：http://hz.jiagoushi.top/gtgjgcafxf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.9152youxi.cn/gtgtnsuafd.html

[S57] C++：编译期常量
来源：http://hz.aibaodan.cn/gtchmtpyqk.html

constexpr int N = 10;
来源：http://hz.hysaishi.cn/gtradngems.html

[S58] C++：命名空间
来源：http://hz.haohaochexian.top/gtrapgtyiq.html

namespace ns { int f() { return 1; } }
来源：http://hz.pycfn.com/gtawlsdqhz.html

[S59] C++：静态断言
来源：http://hz.cashguo.top/gtgjjywgfv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ivvv.top/gtlcrajzpj.html

[S60] C++：遍历并删除元素
来源：http://hz.jinqigufen.top/gtbiuwcnqp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.meibo888.top/gtjcfgbtlw.html

================================================================================
来源：http://hz.kuanghao11.cn/gtntkzallc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jqgufenzy.top/gtjdbohwte.html

================================================================================
来源：http://hz.jyoumei.cn/gtcaxjfsub.html

[T01] Kotlin：Hello World
来源：http://hz.wangshuangyany.cn/gttbedxdng.html

println("Hello")
来源：http://hz.52xcode.cn/gtpjesaqur.html

[T02] Kotlin：变量
来源：http://hz.9152youxi.cn/gtainuwxdg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jqgfzy.top/gtnfsgdhah.html

[T03] Kotlin：字符串模板
来源：http://hz.hammf.cn/gtfikivrhv.html

"值: $b"
来源：http://hz.ppjwa.cn/gtjerpeqcr.html

[T04] Kotlin：空安全
来源：http://hz.yongpay.top/gtyzgnaemr.html

val n: String? = null;  n?.length
来源：http://hz.aizwys.cn/gtlznfgtqo.html

[T05] Kotlin：when 表达式
来源：http://hz.tanke756.top/gtjkucfrds.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ydjk.org.cn/gtayujloui.html

[T06] Kotlin：集合映射
来源：http://hz.zhengqikj.top/gthkokdvhm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.xylfe.cn/gtogoqvtkv.html

[T07] Kotlin：集合过滤
来源：http://hz.jianghu66.top/gtrgnpzofy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yuanzhike.top/gtihvbvhma.html

[T08] Kotlin：数据类
来源：http://hz.cqqwz.cn/gtbrydwxwp.html

data class User(val name: String, val age: Int)
来源：http://hz.ywan-chungtsiang.top/gtqjdfahqu.html

[T09] Kotlin：扩展函数
来源：http://hz.daxiang520.top/gttwtqqscj.html

fun String.exclaim() = this + "!"
来源：http://hz.hysaishi.cn/gtuklhpnif.html

[T10] Kotlin：默认参数
来源：http://hz.gzhubu.top/gtwylpfpby.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yuanzhike.top/gtfqlmeysj.html

[T11] Kotlin：协程
来源：http://hz.gotoacloud.top/gtujkmtorg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.52xcode.cn/gtrtwveqor.html

[T12] Kotlin：解构声明
来源：http://hz.tanke756.top/gtappentbs.html

val (a, b) = Pair(1, 2)
来源：http://hz.hywenlv.cn/gtqgacgbrr.html

[T13] Kotlin：只读 Map
来源：http://hz.quarkkingdee.top/gtksbltdwa.html

val m = mapOf("a" to 1)
来源：http://hz.chenjidiqi.icu/gtbtgtmjmf.html

[T14] Kotlin：循环
来源：http://hz.chenzaomai.com/gtprzzivev.html

for (i in 1..10) println(i)
来源：http://hz.bjfxy.top/gtsmnlwpnf.html

[T15] Kotlin：接口
来源：http://hz.meibo888.top/gtitgbzjwv.html

interface Shape { fun area(): Double }
来源：http://hz.daria6918.cn/gtzmfyhayh.html

[T16] Swift：Hello World
来源：http://hz.pengpengdd.cyou/gtnrmbkpmg.html

print("Hello")
来源：http://hz.jiagoushi.top/gtdkwwontt.html

[T17] Swift：变量与常量
来源：http://hz.jqgufenzy.top/gtiorfpyxa.html

var a = 1;  let b = 2
来源：http://hz.meibo888.top/gtlblxmysq.html

[T18] Swift：字符串插值
来源：http://hz.shanyushiyangtech.top/gtwslowjiy.html

"值: \(b)"
来源：http://hz.ivvv.top/gtwahqikcr.html

[T19] Swift：可选绑定
来源：http://hz.xinyue.icu/gtjyvglcli.html

if let n = opt { print(n) }
来源：http://hz.yangfankeji.com/gtbzqbyjee.html

[T20] Swift：数组操作
来源：http://hz.kuanghao11.cn/gtcfzjanax.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.cashguo.top/gtuitqbioj.html

[T21] Swift：遍历
来源：http://hz.ivvv.top/gtylqtefdd.html

for x in a { print(x) }
来源：http://hz.hongshengwenyu.top/gtvavejbhd.html

[T22] Swift：字典
来源：http://hz.mhx1999.top/gtfvyphygc.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.daxiang520.top/gtspobfikl.html

[T23] Swift：函数
来源：http://hz.guowangkeji.top/gtjsvlvwke.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.havefunace.top/gtlwontgtp.html

[T24] Swift：闭包
来源：http://hz.cheryme.top/gtlbhffrzd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.chenjidiqi.icu/gttnkuidpo.html

[T25] Swift：结构体
来源：http://hz.yangfankeji.com/gtxgsqqewj.html

struct P { var x: Int }
来源：http://hz.yanxiufei.cn/gtqgqnzteq.html

[T26] Swift：类与重写
来源：http://hz.sufxvd.cn/gtnkwwkkiq.html

class A: Base { override func f() {} }
来源：http://hz.hongshengwenyu.top/gtnserlwgk.html

[T27] Swift：错误处理
来源：http://hz.0kj1m.cn/gtdxzysfhk.html

do { try f() } catch { print(error) }
来源：http://hz.kuanghao11.cn/gtkkyosbtt.html

[T28] Swift：枚举
来源：http://hz.aizwys.cn/gtesxdkxpm.html

enum Color { case red, green }
来源：http://hz.hywenlv.cn/gtmckyzayj.html

[T29] Swift：guard 提前返回
来源：http://hz.nwbrower.top/gthmqutjrv.html

guard let x = opt else { return }
来源：http://hz.jianghu66.top/gtjfdwdibd.html

[T30] Swift：协议
来源：http://hz.yonumen.top/gtclmutrec.html

protocol Shape { func area() -> Double }
来源：http://hz.shangyingyoupin.top/gtwcnemkvs.html

[T31] Lua：Hello World
来源：http://hz.jinqigfzy.top/gtxappvbzg.html

print("Hello")
来源：http://hz.jqgfzy.top/gtvvmdzzsv.html

[T32] Lua：局部变量
来源：http://hz.shanyushiyangtech.top/gtbquhmpln.html

local a = 1
来源：http://hz.zycfv.cn/gtpipumlmo.html

[T33] Lua：表（数组）
来源：http://hz.xuetiantiany.cn/gtjvrtmmtb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.hnqzz.top/gtdgnqqhtj.html

[T34] Lua：遍历表
来源：http://hz.shanyushiyangtech.top/gtaietprey.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.snrcjt.cn/gtaavffwiq.html

[T35] Lua：字典表
来源：http://hz.jinyuanbaomall.cn/gthktemxon.html

local d = { a = 1 };  d.b = 2
来源：http://hz.cdnleiting.top/gthnjopxwq.html

[T36] Lua：函数
来源：http://hz.cqqwz.cn/gtfktjzsjd.html

function add(a, b) return a + b end
来源：http://hz.xuanzx.com/gtzpbmiket.html

[T37] Lua：字符串拼接
来源：http://hz.zhaomingkeji.xyz/gtwwxqzank.html

"a" .. "b"
来源：http://hz.shzxlz.cn/gtweghjeqd.html

[T38] Lua：条件
来源：http://hz.mhx1999.top/gtfakrculr.html

if x > 0 then print("正") end
来源：http://hz.gotoacloud.top/gtxtuvmrug.html

[T39] Lua：模式匹配
来源：http://hz.nanxuanxn.top/gtspwuqgzt.html

string.find(s, "%d+")
来源：http://hz.gaohongyu789.top/gtyqovegja.html

[T40] Lua：元表
来源：http://hz.daxiang520.top/gturiqjywj.html

setmetatable({}, { __index = base })
来源：http://hz.aizwys.cn/gtdqwgsaxx.html

[T41] Perl：Hello World
来源：http://hz.ywan-chungtsiang.top/gtgdeobpio.html

print "Hello\n";
来源：http://hz.xuanzx.com/gtoswkdrwa.html

[T42] Perl：变量类型
来源：http://hz.zhaomingkeji.xyz/gtmwedqepy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.cheryme.top/gtpfpygkex.html

[T43] Perl：字符串插值
来源：http://hz.cucudq.cn/gtvfchvtnl.html

"值: $a"
来源：http://hz.snrcjt.cn/gtnsrdrypv.html

[T44] Perl：条件
来源：http://hz.zdqjudy.top/gtmlegbdei.html

if ($a > 0) { print "正"; }
来源：http://hz.dashuyun.cn/gtqcznklbq.html

[T45] Perl：数组遍历
来源：http://hz.jinqigfzy.top/gtvyjnwmzi.html

for my $x (@arr) { print $x; }
来源：http://hz.shangyingyoupin.top/gtiwcuzldv.html

[T46] Perl：哈希操作
来源：http://hz.gaohongyu789.top/gtlqtwgkcf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.dianchejie.cn/gtidngnaac.html

[T47] Perl：正则捕获
来源：http://hz.yangfankeji.com/gtpijfomxn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yuxming.cn/gtlcfnowam.html

[T48] Perl：正则替换
来源：http://hz.sxryk.cn/gtqpasqaqi.html

$s =~ s/old/new/g;
来源：http://hz.yj20258888.top/gtgttvueus.html

[T49] Perl：函数
来源：http://hz.hammf.cn/gtljjeznue.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.birdmap.top/gtuxboijsx.html

[T50] Perl：逐行读文件
来源：http://hz.zhoulong.xyz/gtqiqxdmpz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.chenjidiqi.icu/gtatmpibex.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yj20258888.top/gtfmcnpcui.html

[T51] Scala：Hello World
来源：http://hz.snrcjt.cn/gtxraeyxye.html

println("Hello")
来源：http://hz.ywan-chungtsiang.top/gteyyrnzif.html

[T52] Scala：变量
来源：http://hz.meibo888.top/gtqwlutozf.html

val a = 1;  var b = 2
来源：http://hz.mhx1999.top/gtltnaweit.html

[T53] Scala：字符串插值
来源：http://hz.yj20258.top/gtbntwnpwa.html

s"值: $b"
来源：http://hz.ehwqpu.com/gtsvmczqvd.html

[T54] Scala：集合映射
来源：http://hz.jinyuanbaomall.cn/gtlyeemkrd.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.cashguo.top/gtsjllrkfw.html

[T55] Scala：集合过滤
来源：http://hz.hnqzz.top/gtddixdliq.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.hnxiangtu.top/gtliyacymo.html

[T56] Scala：样例类
来源：http://hz.andypj.xyz/gtqanextwv.html

case class User(name: String, age: Int)
来源：http://hz.quarkkingdee.top/gttnpmgcub.html

[T57] Scala：模式匹配
来源：http://hz.iojbl.cn/gtivqvjzae.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.fzhhl.top/gtqtwpooou.html

[T58] Scala：函数定义
来源：http://hz.yj20258888.top/gthyncwotw.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.vqdsnc.cn/gttmxtderz.html

[T59] Scala：循环
来源：http://hz.dianchejie.cn/gtohlddzgi.html

for (i <- 1 to 10) println(i)
来源：http://hz.smart0.xyz/gthjhwvird.html

[T60] Scala：折叠
来源：http://hz.0kj1m.cn/gttqqqkabq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.xuanzx.com/gtxpiyvjpz.html

================================================================================
来源：http://hz.jlsjyb.cn/gtpxqxlnko.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.tian-w.cn/gtciqalvoy.html

================================================================================
来源：http://hz.jinqigfzy.top/gtfgsanltx.html

[U01] Py：创建虚拟环境
来源：http://hz.jlsjyb.cn/gtjgeklhhn.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.chenzaomai.com/gtmwdoqzcm.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jinghuilouyu.cn/gtcbdzedtv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.ppjwa.cn/gtixrnjdxg.html

[U03] Py：加载 .env 配置
来源：http://hz.tianlin.xyz/gtxnksluha.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.shzxlz.cn/gtqoxjzzoj.html

[U04] Py：变量调试打印
来源：http://hz.yj202588.top/gtkxudzwna.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yonumen.top/gtsjlfqnne.html

[U05] Py：列表去重且保序
来源：http://hz.0kj1m.cn/gthdgerzbt.html

list(dict.fromkeys(arr))
来源：http://hz.sysykeji.top/gtfpdoyusi.html

[U06] Py：合并两个字典
来源：http://hz.xylfe.cn/gtvpsrvhjr.html

{**a, **b}
来源：http://hz.fengsongda.top/gtyowmdcqk.html

[U07] Py：反转字典键值
来源：http://hz.jlsjyb.cn/gtdejcopvf.html

{v: k for k, v in d.items()}
来源：http://hz.jinqigfzy.top/gthzabzisc.html

[U08] Py：展平二维列表
来源：http://hz.nwbrower.top/gtulpbbwoj.html

[y for x in nested for y in x]
来源：http://hz.tanke756.top/gtvrzklabh.html

[U09] Py：字典取最大值的键
来源：http://hz.shzxlz.cn/gtxomwxzdo.html

max(d, key=d.get)
来源：http://hz.yj20258.top/gtddlkvrgp.html

[U10] Py：按值排序字典
来源：http://hz.tianlin.xyz/gttwkolqtu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.quarkkingdee.top/gtkrujlsoh.html

[U11] Py：生成器表达式
来源：http://hz.yangfankeji.com/gtnrhoiyrz.html

(x * 2 for x in arr)
来源：http://hz.ivvv.top/gtcvnrrqdj.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.shzxlz.cn/gtayluiluh.html

Counter(arr).most_common(3)
来源：http://hz.nanxuanxn.top/gtqubujehx.html

[U13] Py：固定长度队列
来源：http://hz.shangyingyoupin.top/gtugowyins.html

deque(maxlen=10)
来源：http://hz.jqgufenzy.top/gttpqpeuvj.html

[U14] Py：分组收集到列表
来源：http://hz.xinyue.icu/gtxgqbsmnz.html

defaultdict(list)
来源：http://hz.sufxvd.cn/gtgqmiafve.html

[U15] Py：高精度计时
来源：http://hz.yongpay.top/gtvyydlsvq.html

t = time.perf_counter()
来源：http://hz.ybcxt.top/gtpcinqmjb.html

[U16] Py：命令行参数解析
来源：http://hz.ydzc1.top/gtjomfrsao.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.smart0.xyz/gtdegowvjj.html

[U17] Py：初始化日志
来源：http://hz.jqgufenzy.top/gttlvijefp.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.andypj.xyz/gtphozvpqw.html

[U18] Py：预编译正则
来源：http://hz.jlsjyb.cn/gthrfpdcjx.html

pat = re.compile(r"\d+")
来源：http://hz.ybcxt.top/gtbgdfocpt.html

[U19] Py：正则替换带回调
来源：http://hz.jinqigfzy.top/gtimewefkj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.jqgfzy.top/gtaiesolbd.html

[U20] Py：缓存函数结果
来源：http://hz.jiagoushi.top/gtbgxlryhu.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yuxming.cn/gtatcdcpqe.html

[U21] Py：自定义上下文管理器
来源：http://hz.dashuyun.cn/gtprvaoojb.html

@contextlib.contextmanager
来源：http://hz.mhx1999.top/gtpngalaxw.html

[U22] Py：矩阵转置
来源：http://hz.nanxinkj.top/gttxuaqmpf.html

list(zip(*m))
来源：http://hz.ybcxt.top/gtdpfmzquu.html

[U23] Py：分块读取大文件
来源：http://hz.bjfxy.top/gtfydhjhdm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.bjfxy.top/gtsrzvngpi.html

[U24] Py：路径操作
来源：http://hz.hongshengwenyu.top/gttxdidvad.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.jiagoushi.top/gtvaofqtdy.html

[U25] Py：CSV 按字典读
来源：http://hz.tanke756.top/gtvjlxxwkh.html

csv.DictReader(f)
来源：http://hz.zhongyouzk.top/gtbmqqfzgt.html

[U26] Py：并发下载
来源：http://hz.dashuyun.cn/gtbkerzuhn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jiagoushi.top/gtlwryccsi.html

[U27] Py：异步 HTTP
来源：http://hz.birdmap.top/gtetufxram.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.iojbl.cn/gtydfqsivs.html

[U28] Py：类型别名
来源：http://hz.hongshengwenyu.top/gtjnmfceei.html

UserId = int
来源：http://hz.havefunace.top/gtqqnzqums.html

[U29] Py：属性校验
来源：http://hz.zhongyouzk.top/gtefqddgxc.html

@property 与 @x.setter 配合
来源：http://hz.ehwqpu.com/gtjmwxeobe.html

[U30] Py：数据类
来源：http://hz.zhoulong.xyz/gtfovobpvy.html

@dataclass(slots=True)
来源：http://hz.nanxuanxn.top/gtnhtegepf.html

[U31] Py：单测
来源：http://hz.zhengqikj.top/gtjyoqvdcw.html

python -m pytest -q
来源：http://hz.c1oappe.top/gtyprrxolg.html

[U32] Py：代码格式化
来源：http://hz.aibaodan.cn/gtojrvxquv.html

ruff format . && ruff check --fix .
来源：http://hz.zhijiandao.cn/gtuwssaucq.html

[U33] Py：打包发布
来源：http://hz.hywenlv.cn/gtyzpaxfoe.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.jinqigfzy.top/gthugcjjqb.html

[U34] Py：判断编码
来源：http://hz.yanxiufei.cn/gtonlcnajh.html

chardet.detect(raw)
来源：http://hz.hnqzz.top/gtluhsqwtj.html

[U35] Py：发送邮件
来源：http://hz.9152youxi.cn/gtmeohcjpa.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.xylfe.cn/gthjskqlxh.html

[U36] Py：定时任务
来源：http://hz.tianlin.xyz/gtemxdebfi.html

schedule.every(10).minutes.do(job)
来源：http://hz.daria6918.cn/gtryivbksg.html

[U37] Py：读写 Excel
来源：http://hz.hysaishi.cn/gtgvfhgbuo.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.shzxlz.cn/gtjvurtqgn.html

[U38] Py：获取脚本所在目录
来源：http://hz.yanxiufei.cn/gtktvjgxzv.html

Path(__file__).resolve().parent
来源：http://hz.yueranfly.top/gtokyvwlod.html

[U39] Py：判断是否在交互环境
来源：http://hz.zhijiandao.cn/gtojhvwztw.html

sys.stdout.isatty()
来源：http://hz.cqqwz.cn/gtsvadxitw.html

[U40] Py：打印到标准错误
来源：http://hz.hywenlv.cn/gtksuhwalv.html

print("err", file=sys.stderr)
来源：http://hz.gogol.net.cn/gtypeoywbd.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.hysaishi.cn/gtwmprupxx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.gaohongyu789.top/gtbhwcblmm.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.zhixingplan.top/gtfptjjkqn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.shangyingyoupin.top/gtwqoqkvnu.html


<!-- 参考信息 -->