代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.shzxlz.cn/gtcdwarkol.html

[S13] C：宏定义
来源：http://hz.mhx1999.top/gtjqlcrdsb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jyoumei.cn/gtvpxlmlip.html

[S14] C：枚举
来源：http://hz.andypj.xyz/gthyveyceb.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hammf.cn/gtmkcaaijn.html

[S15] C：类型转换
来源：http://hz.xylfe.cn/gtzouihmhs.html

(double) a / b
来源：http://hz.shangyingyoupin.top/gtfwajyehn.html

[S16] C：位操作置位
来源：http://hz.zhixingplan.top/gtglxjztfh.html

x |= (1 << 3);
来源：http://hz.quarkkingdee.top/gtlorehdka.html

[S17] C：安全拼接字符串
来源：http://hz.gotoacloud.top/gtqegwnncg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.wangshuangyany.cn/gtflkjlbwv.html

[S18] C：命令行参数
来源：http://hz.jianghu66.top/gthktpwuux.html

int main(int argc, char **argv)
来源：http://hz.hywenlv.cn/gtbytgsugo.html

[S19] C：快速排序
来源：http://hz.gzhubu.top/gthxnckids.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.0kj1m.cn/gtfatycfxn.html

[S20] C：二分查找
来源：http://hz.hongshengwenyu.top/gtgqtbiikf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.chenjidiqi.icu/gtcbpiivqv.html

[S21] C：字符类别判断
来源：http://hz.zhengqikj.top/gtlilgasvq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.aizwys.cn/gtalzuwnbw.html

[S22] C：字符串转数字
来源：http://hz.hammf.cn/gtuzqjicbm.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.wangdashe.top/gtxnozdelx.html

[S23] C：随机数
来源：http://hz.chenlongwang.top/gtgzcsgssr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yvedp.cn/gtjyavqzwn.html

[S24] C：获取本地时间
来源：http://hz.zhengqikj.top/gtdveclkbf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zycfv.cn/gtrpbdhden.html

[S25] C：内存拷贝
来源：http://hz.zhongyouzk.top/gtgsejilwg.html

memcpy(dst, src, n);
来源：http://hz.jqgufenzy.top/gthbbcbgwn.html

[S26] C：内存清零
来源：http://hz.nanxinkj.top/gtwshxljdx.html

memset(a, 0, sizeof a);
来源：http://hz.yj202588.top/gtvpkkujlb.html

[S27] C：定义常量
来源：http://hz.yj20258888.top/gtnkbtxjia.html

const double PI = 3.14159;
来源：http://hz.sxryk.cn/gtsquygtyb.html

[S28] C：静态变量
来源：http://hz.shangyingyoupin.top/gtdafjibrz.html

static int counter = 0;
来源：http://hz.cqqwz.cn/gtskjcawyz.html

[S29] C：变参函数
来源：http://hz.dashuyun.cn/gtcfnwfwvo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jqgfzy.top/gtbcieqkaq.html

[S30] C：头文件保护
来源：http://hz.shangyingyoupin.top/gthozynwmc.html

#ifndef X_H
来源：http://hz.cheryme.top/gtdhpjkkwl.html

#define X_H
来源：http://hz.hongshengwenyu.top/gtmygjgvav.html

#endif
来源：http://hz.yueranfly.top/gtbixopfqp.html

[S31] C++：Hello World
来源：http://hz.ydzc1.top/gtiybcaomc.html

#include <iostream>
来源：http://hz.cashguo.top/gtbyqzmzxc.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.dashuyun.cn/gtqzkgwygg.html

[S32] C++：字符串
来源：http://hz.shanyushiyangkeji.top/gtvnihpjct.html

std::string s = "hi";  s += "!";
来源：http://hz.0kj1m.cn/gttoqcczmv.html

[S33] C++：vector 增删
来源：http://hz.316326.xyz/gtoudvplyj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.chenlongwang.top/gtwkmubfag.html

[S34] C++：遍历 vector
来源：http://hz.gzhubu.top/gtbjpqyclm.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zycfv.cn/gtexecjjyt.html

[S35] C++：map
来源：http://hz.ydzc1.top/gtdrpkpsbv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.chenlongwang.top/gtzcyduwah.html

[S36] C++：unordered_map
来源：http://hz.jqgufenzy.top/gtvgsrdnix.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shangyingyoupin.top/gtaamirdwj.html

[S37] C++：set
来源：http://hz.chenzaomai.com/gtrbchjugy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.haohaochexian.top/gtpkbqdmul.html

[S38] C++：排序
来源：http://hz.bjfxy.top/gttfofojzs.html

std::sort(v.begin(), v.end());
来源：http://hz.cheryme.top/gtqvqenfqu.html

[S39] C++：自定义比较器排序
来源：http://hz.vqdsnc.cn/gtjtwfhplp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhijiandao.cn/gtyxtwicqg.html

[S40] C++：查找元素
来源：http://hz.yvedp.cn/gtwntzzcln.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.bjfxy.top/gtjblyjdyi.html

[S41] C++：类与构造函数
来源：http://hz.zhengqikj.top/gtnagccxzb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.meibo888.top/gtwudzecfk.html

[S42] C++：继承与虚函数
来源：http://hz.9152youxi.cn/gtlfwvwdfi.html

class B : public Base { public: void f() override {} };
来源：http://hz.aibaodan.cn/gtpvchfoik.html

[S43] C++：智能指针
来源：http://hz.mhx1999.top/gtjyidvgkv.html

auto p = std::make_unique<int>(5);
来源：http://hz.zdqjudy.top/gtscmzplut.html

[S44] C++：引用传参
来源：http://hz.yuxming.cn/gtxrnyyoke.html

void inc(int &x) { ++x; }
来源：http://hz.feifeiyinyue.top/gthcwgnbno.html

[S45] C++：lambda
来源：http://hz.snrcjt.cn/gtlwgnsrsw.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jinqigufen.top/gtrulpuzoh.html

[S46] C++：函数模板
来源：http://hz.ydzc1.top/gtaouqgmly.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.hammf.cn/gtjrxmuwin.html

[S47] C++：结构化绑定遍历
来源：http://hz.ywan-chungtsiang.top/gtgmvxpfzm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.tian-w.cn/gtvcnyvvzs.html

[S48] C++：逐行读文件
来源：http://hz.nanxinkj.top/gtgydncohs.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shangyingyoupin.top/gtsgudvvbv.html

while (std::getline(in, line)) { }
来源：http://hz.svipenyu.cn/gtnmccnusu.html

[S49] C++：写文件
来源：http://hz.guowangkeji.top/gtdqfgtinq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.wangdashe.top/gtbxrjarnn.html

[S50] C++：格式化数字
来源：http://hz.feifeiyinyue.top/gtibzogjmm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.tian-w.cn/gtmjaywybx.html

[S51] C++：显式类型转换
来源：http://hz.shangyingyoupin.top/gtnmbgjjco.html

static_cast<double>(a) / b
来源：http://hz.dashuyun.cn/gtwbjomvww.html

[S52] C++：const 与 noexcept
来源：http://hz.xziqi.cn/gtuhxuxxrf.html

int size() const noexcept { return n_; }
来源：http://hz.xuetiantiany.cn/gtgefqxewz.html

[S53] C++：移动语义
来源：http://hz.yj20258888.top/gtrjyzxajb.html

std::vector<int> w = std::move(v);
来源：http://hz.gotoacloud.top/gtjtgydlem.html

[S54] C++：异常处理
来源：http://hz.cheryme.top/gtibtvvcll.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ppjwa.cn/gtnthypdyi.html

[S55] C++：结构化绑定
来源：http://hz.yuanzhike.top/gtckcecqrs.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jiagoushi.top/gtpawiandd.html

[S56] C++：optional
来源：http://hz.0kj1m.cn/gthrvmzyyh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhijiandao.cn/gtujiwuuuh.html

[S57] C++：编译期常量
来源：http://hz.xylfe.cn/gtdtfqcyim.html

constexpr int N = 10;
来源：http://hz.tianlin.xyz/gtjpvtcxen.html

[S58] C++：命名空间
来源：http://hz.yuanzhike.top/gtuadmnucj.html

namespace ns { int f() { return 1; } }
来源：http://hz.wangdashe.top/gtwggcfkfn.html

[S59] C++：静态断言
来源：http://hz.yj202588.top/gtylnnzzcg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.chenzaomai.com/gtjcbgkxda.html

[S60] C++：遍历并删除元素
来源：http://hz.hnxiangtu.top/gtdfrmekew.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.shangyingyoupin.top/gtvogduhpm.html

================================================================================
来源：http://hz.svipenyu.cn/gttcwcppeh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.chenzaomai.com/gtvmebbmak.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtbsllvfoi.html

[T01] Kotlin：Hello World
来源：http://hz.hnqzz.top/gtphoqpsik.html

println("Hello")
来源：http://hz.shanyushiyangtech.top/gthersxawl.html

[T02] Kotlin：变量
来源：http://hz.sxryk.cn/gtyquxctzz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xylfe.cn/gtbedcacig.html

[T03] Kotlin：字符串模板
来源：http://hz.zhixingplan.top/gtqbfozrld.html

"值: $b"
来源：http://hz.shanyushiyangtech.top/gtbergdwqt.html

[T04] Kotlin：空安全
来源：http://hz.xingfuxueyuan.xyz/gtkiwqrwhg.html

val n: String? = null;  n?.length
来源：http://hz.shzxlz.cn/gtwlzfhnsm.html

[T05] Kotlin：when 表达式
来源：http://hz.yj20258.top/gtdswbeshy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.wangshuangyany.cn/gtobyjtkim.html

[T06] Kotlin：集合映射
来源：http://hz.daxiang520.top/gtgkdyshex.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.aizwys.cn/gtjpbfshrf.html

[T07] Kotlin：集合过滤
来源：http://hz.shzxlz.cn/gtwfntejoc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.sweek.top/gtjkjgeqmo.html

[T08] Kotlin：数据类
来源：http://hz.svipenyu.cn/gtspiadwfh.html

data class User(val name: String, val age: Int)
来源：http://hz.smart0.xyz/gtbhqjdpkw.html

[T09] Kotlin：扩展函数
来源：http://hz.pengpengdd.cyou/gtupgznbqr.html

fun String.exclaim() = this + "!"
来源：http://hz.dashuyun.cn/gtgunrxntj.html

[T10] Kotlin：默认参数
来源：http://hz.gzhubu.top/gtriiwnujv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.havefunace.top/gtyimlzvfi.html

[T11] Kotlin：协程
来源：http://hz.svipenyu.cn/gteqaejwlg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.hfpthk.cn/gtyzhfobuf.html

[T12] Kotlin：解构声明
来源：http://hz.chenjidiqi.icu/gttidbaucu.html

val (a, b) = Pair(1, 2)
来源：http://hz.vqdsnc.cn/gtrnglgvdm.html

[T13] Kotlin：只读 Map
来源：http://hz.yongpay.top/gtpeceoykn.html

val m = mapOf("a" to 1)
来源：http://hz.dianchejie.cn/gtdqjiwavy.html

[T14] Kotlin：循环
来源：http://hz.jianghu66.top/gtriyfqext.html

for (i in 1..10) println(i)
来源：http://hz.pycfn.com/gtgqcnkkms.html

[T15] Kotlin：接口
来源：http://hz.zhaomingkeji.xyz/gtjiyadusl.html

interface Shape { fun area(): Double }
来源：http://hz.haohaochexian.top/gtchqaqxue.html

[T16] Swift：Hello World
来源：http://hz.zhaomingkeji.xyz/gtsccialnd.html

print("Hello")
来源：http://hz.redwolf501.top/gtxiqlfaac.html

[T17] Swift：变量与常量
来源：http://hz.guowangkeji.top/gtvccwwvpj.html

var a = 1;  let b = 2
来源：http://hz.meibo888.top/gtvylmxmde.html

[T18] Swift：字符串插值
来源：http://hz.fzhhl.top/gtysaeaynh.html

"值: \(b)"
来源：http://hz.gotoacloud.top/gtgfdmgwen.html

[T19] Swift：可选绑定
来源：http://hz.shzxlz.cn/gtprhbyuvh.html

if let n = opt { print(n) }
来源：http://hz.shzxlz.cn/gtmfdpfmmi.html

[T20] Swift：数组操作
来源：http://hz.jqgfzy.top/gtjdkmarcf.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.sufxvd.cn/gtcgckxmqr.html

[T21] Swift：遍历
来源：http://hz.aibaodan.cn/gtmjbsjxap.html

for x in a { print(x) }
来源：http://hz.xziqi.cn/gtkoqspvlt.html

[T22] Swift：字典
来源：http://hz.yanxiufei.cn/gtqxesochb.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.gaohongyu789.top/gtishcanjp.html

[T23] Swift：函数
来源：http://hz.wangshuangyany.cn/gtjbsipuhg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yanxiufei.cn/gtktppabmb.html

[T24] Swift：闭包
来源：http://hz.chenjidiqi.icu/gtqbvpdgoq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.dianchejie.cn/gtsjyslhdt.html

[T25] Swift：结构体
来源：http://hz.haohaochexian.top/gtasaoougd.html

struct P { var x: Int }
来源：http://hz.jinqigfzy.top/gtvjujbskd.html

[T26] Swift：类与重写
来源：http://hz.zdqjudy.top/gtecvkjwjp.html

class A: Base { override func f() {} }
来源：http://hz.yj202588.top/gthckhdgop.html

[T27] Swift：错误处理
来源：http://hz.sxryk.cn/gtiuvumhgc.html

do { try f() } catch { print(error) }
来源：http://hz.shanyushiyangtech.top/gtamnstsrh.html

[T28] Swift：枚举
来源：http://hz.cucudq.cn/gtxrmwlvhq.html

enum Color { case red, green }
来源：http://hz.haohaochexian.top/gtwhoegtwv.html

[T29] Swift：guard 提前返回
来源：http://hz.vqdsnc.cn/gtbrthwccy.html

guard let x = opt else { return }
来源：http://hz.ydzc1.top/gtyutmtrkj.html

[T30] Swift：协议
来源：http://hz.ywan-chungtsiang.top/gtsjejejbk.html

protocol Shape { func area() -> Double }
来源：http://hz.yvedp.cn/gtbyrpxgxs.html

[T31] Lua：Hello World
来源：http://hz.cqqwz.cn/gtjzmocorq.html

print("Hello")
来源：http://hz.hongshengwenyu.top/gttmwutfji.html

[T32] Lua：局部变量
来源：http://hz.jianghu66.top/gtlxpcqxid.html

local a = 1
来源：http://hz.haohaochexian.top/gtcxlfhxjr.html

[T33] Lua：表（数组）
来源：http://hz.yanxiufei.cn/gtdekdfuws.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.xingfuxueyuan.xyz/gtxflsuvbz.html

[T34] Lua：遍历表
来源：http://hz.gogol.net.cn/gtrvotbgxx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.guannengcc.top/gtgzmtqwkc.html

[T35] Lua：字典表
来源：http://hz.c1oappe.top/gtrhzdthrm.html

local d = { a = 1 };  d.b = 2
来源：http://hz.cdnleiting.top/gtrzoyxccs.html

[T36] Lua：函数
来源：http://hz.xinyue.icu/gtjnttiswf.html

function add(a, b) return a + b end
来源：http://hz.redwolf501.top/gttwbvpgvc.html

[T37] Lua：字符串拼接
来源：http://hz.bjfxy.top/gtbdtbxtru.html

"a" .. "b"
来源：http://hz.shzxlz.cn/gtevlhqfdj.html

[T38] Lua：条件
来源：http://hz.snrcjt.cn/gtzbfyergf.html

if x > 0 then print("正") end
来源：http://hz.tanke756.top/gtylcqdzxd.html

[T39] Lua：模式匹配
来源：http://hz.jinghuilouyu.cn/gtgbdyrzdl.html

string.find(s, "%d+")
来源：http://hz.hongshengwenyu.top/gtwiwdxell.html

[T40] Lua：元表
来源：http://hz.yanxiufei.cn/gtlaalneby.html

setmetatable({}, { __index = base })
来源：http://hz.vqdsnc.cn/gtruhwbalj.html

[T41] Perl：Hello World
来源：http://hz.yj20258888.top/gtneiggvvs.html

print "Hello\n";
来源：http://hz.iojbl.cn/gthnsrqpor.html

[T42] Perl：变量类型
来源：http://hz.svipenyu.cn/gtxaivnkjx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jinyuanbaomall.cn/gtmvroohxl.html

[T43] Perl：字符串插值
来源：http://hz.zhengqikj.top/gtmsiftrfn.html

"值: $a"
来源：http://hz.nwbrower.top/gtcnjmazto.html

[T44] Perl：条件
来源：http://hz.sweek.top/gtdfkitlzt.html

if ($a > 0) { print "正"; }
来源：http://hz.pycfn.com/gtlqrkzsfy.html

[T45] Perl：数组遍历
来源：http://hz.ppjwa.cn/gtpucuipkz.html

for my $x (@arr) { print $x; }
来源：http://hz.ppjwa.cn/gtlfwmekvm.html

[T46] Perl：哈希操作
来源：http://hz.chenzaomai.com/gthmqyfrpz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.mhx1999.top/gtedvrbdfk.html

[T47] Perl：正则捕获
来源：http://hz.smart0.xyz/gtvnahyacp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.snrcjt.cn/gtciuktajj.html

[T48] Perl：正则替换
来源：http://hz.chenlongwang.top/gtypwfqhjh.html

$s =~ s/old/new/g;
来源：http://hz.bjfxy.top/gtzztpjeqc.html

[T49] Perl：函数
来源：http://hz.hysaishi.cn/gtzfkilygt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jyoumei.cn/gtquzjhlss.html

[T50] Perl：逐行读文件
来源：http://hz.shuidangran.top/gtrpnkfaid.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.tian-w.cn/gtppczcnpw.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.xuanzx.com/gtacitrhta.html

[T51] Scala：Hello World
来源：http://hz.jiagoushi.top/gtqlejfdid.html

println("Hello")
来源：http://hz.cdnleiting.top/gtoferpyto.html

[T52] Scala：变量
来源：http://hz.smart0.xyz/gtpoxbrocf.html

val a = 1;  var b = 2
来源：http://hz.sysykeji.top/gtjfqszrjc.html

[T53] Scala：字符串插值
来源：http://hz.hongshengwenyu.top/gtoiibyirr.html

s"值: $b"
来源：http://hz.yvedp.cn/gtvuflvlqt.html

[T54] Scala：集合映射
来源：http://hz.hammf.cn/gtrqxugjxj.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.fzhhl.top/gturdqjhug.html

[T55] Scala：集合过滤
来源：http://hz.bjfxy.top/gtqedszyyj.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.xziqi.cn/gturznoqlj.html

[T56] Scala：样例类
来源：http://hz.316326.xyz/gtlrtaykev.html

case class User(name: String, age: Int)
来源：http://hz.shanyushiyangtech.top/gtpvripwgd.html

[T57] Scala：模式匹配
来源：http://hz.wangshuangyany.cn/gtwrqnwzgu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.shuidangran.top/gtblxopoep.html

[T58] Scala：函数定义
来源：http://hz.52xcode.cn/gtzlpwwqly.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.kuanghao11.cn/gttixesqil.html

[T59] Scala：循环
来源：http://hz.zdqjudy.top/gtweipwoiv.html

for (i <- 1 to 10) println(i)
来源：http://hz.yuxming.cn/gtjsblfwwc.html

[T60] Scala：折叠
来源：http://hz.sweek.top/gttjrqncid.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.zhoulong.xyz/gthpvhhnxw.html

================================================================================
来源：http://hz.jqgufenzy.top/gtxrimngsw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.haohaochexian.top/gtpcqywhsq.html

================================================================================
来源：http://hz.gzhubu.top/gtktfmpydq.html

[U01] Py：创建虚拟环境
来源：http://hz.dashuyun.cn/gthxniyjcf.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.jinqigufen.top/gtzeeqlijj.html

[U02] Py：导出 / 安装依赖
来源：http://hz.tanke756.top/gtigtomlko.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.xingfuxueyuan.xyz/gtqdtkxixv.html

[U03] Py：加载 .env 配置
来源：http://hz.hywenlv.cn/gtoqhcsqes.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.chenlongwang.top/gtmnjucvgh.html

[U04] Py：变量调试打印
来源：http://hz.shuidangran.top/gtileknnun.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yuxming.cn/gtfffbrqel.html

[U05] Py：列表去重且保序
来源：http://hz.jyoumei.cn/gtqutwkrxd.html

list(dict.fromkeys(arr))
来源：http://hz.ywan-chungtsiang.top/gtibxibayr.html

[U06] Py：合并两个字典
来源：http://hz.kuanghao11.cn/gtgtkgwgag.html

{**a, **b}
来源：http://hz.chenzaomai.com/gtzzrqqbfs.html

[U07] Py：反转字典键值
来源：http://hz.guannengcc.top/gtjtgeakfy.html

{v: k for k, v in d.items()}
来源：http://hz.xziqi.cn/gtxfxsvmgg.html

[U08] Py：展平二维列表
来源：http://hz.xziqi.cn/gtedsuzdpo.html

[y for x in nested for y in x]
来源：http://hz.aizwys.cn/gtckridzho.html

[U09] Py：字典取最大值的键
来源：http://hz.gotoacloud.top/gtyvdrprnc.html

max(d, key=d.get)
来源：http://hz.hnqzz.top/gttocmjhgt.html

[U10] Py：按值排序字典
来源：http://hz.hongshengwenyu.top/gtxoctzqzi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.jiagoushi.top/gtodcyngvb.html

[U11] Py：生成器表达式
来源：http://hz.wangdashe.top/gtywnzkuyk.html

(x * 2 for x in arr)
来源：http://hz.xuanzx.com/gtjdgskxbu.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.quarkkingdee.top/gtoimosqqa.html

Counter(arr).most_common(3)
来源：http://hz.hammf.cn/gtpxrwnjqp.html

[U13] Py：固定长度队列
来源：http://hz.andypj.xyz/gteasmhrlg.html

deque(maxlen=10)
来源：http://hz.redwolf501.top/gtfhfjrjwd.html

[U14] Py：分组收集到列表
来源：http://hz.cqqwz.cn/gtughovoho.html

defaultdict(list)
来源：http://hz.ydjk.org.cn/gtvnwmnqbj.html

[U15] Py：高精度计时
来源：http://hz.tian-w.cn/gtoluruckw.html

t = time.perf_counter()
来源：http://hz.jinyuanbaomall.cn/gtyuyglqup.html

[U16] Py：命令行参数解析
来源：http://hz.sweek.top/gtbwbypmxv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.nanxinkj.top/gtkzgmuuwp.html

[U17] Py：初始化日志
来源：http://hz.xuanzx.com/gtsmvxtxuy.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.ydzc1.top/gtnoffxyrh.html

[U18] Py：预编译正则
来源：http://hz.sysykeji.top/gteqmjxfha.html

pat = re.compile(r"\d+")
来源：http://hz.hongshengwenyu.top/gtdzpntkzi.html

[U19] Py：正则替换带回调
来源：http://hz.jinqigfzy.top/gtvetfmfkq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.hysaishi.cn/gtjtwkahya.html

[U20] Py：缓存函数结果
来源：http://hz.tanke756.top/gtbmunazat.html

@functools.lru_cache(maxsize=None)
来源：http://hz.ehwqpu.com/gtgabcpldx.html

[U21] Py：自定义上下文管理器
来源：http://hz.yj202588.top/gtusvwgnsr.html

@contextlib.contextmanager
来源：http://hz.hammf.cn/gtqlysvzuu.html

[U22] Py：矩阵转置
来源：http://hz.andypj.xyz/gtnnmlfint.html

list(zip(*m))
来源：http://hz.fengsongda.top/gttzklgtfa.html

[U23] Py：分块读取大文件
来源：http://hz.svipenyu.cn/gtflotzspu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.jlsjyb.cn/gtdaqegywe.html

[U24] Py：路径操作
来源：http://hz.yongpay.top/gtaysnaeyq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.yvedp.cn/gtliutsyqw.html

[U25] Py：CSV 按字典读
来源：http://hz.gzhubu.top/gtflqseyxj.html

csv.DictReader(f)
来源：http://hz.pycfn.com/gtrhrtlpmw.html

[U26] Py：并发下载
来源：http://hz.zhoulong.xyz/gtldaqcwhe.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.chenzaomai.com/gtbaoscxpr.html

[U27] Py：异步 HTTP
来源：http://hz.gogol.net.cn/gtypaskwrb.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.pengpengdd.cyou/gtpsumrjod.html

[U28] Py：类型别名
来源：http://hz.yonumen.top/gtieifpewd.html

UserId = int
来源：http://hz.ppjwa.cn/gtfaoxplbj.html

[U29] Py：属性校验
来源：http://hz.cqqwz.cn/gtazxhujro.html

@property 与 @x.setter 配合
来源：http://hz.52xcode.cn/gtrfyozhuh.html

[U30] Py：数据类
来源：http://hz.birdmap.top/gtznxrcwax.html

@dataclass(slots=True)
来源：http://hz.shanyushiyangtech.top/gtywsoaecr.html

[U31] Py：单测
来源：http://hz.smart0.xyz/gtlpmccoib.html

python -m pytest -q
来源：http://hz.fengsongda.top/gtfywygkae.html

[U32] Py：代码格式化
来源：http://hz.dashuyun.cn/gtofzltfgu.html

ruff format . && ruff check --fix .
来源：http://hz.ivvv.top/gtalzfnoel.html

[U33] Py：打包发布
来源：http://hz.feifeiyinyue.top/gtkrunvdwt.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.shanyushiyangtech.top/gtubxhfhzb.html

[U34] Py：判断编码
来源：http://hz.redwolf501.top/gtegxeiwla.html

chardet.detect(raw)
来源：http://hz.yj202588.top/gtorvvogyt.html

[U35] Py：发送邮件
来源：http://hz.jyoumei.cn/gtqkiuchuc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.pengpengdd.cyou/gtirfwuqfj.html

[U36] Py：定时任务
来源：http://hz.yj20258.top/gtneoooizq.html

schedule.every(10).minutes.do(job)
来源：http://hz.ppjwa.cn/gtzjhraayk.html


<!-- 参考信息 -->