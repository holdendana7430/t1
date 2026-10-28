代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ywan-chungtsiang.top/gtckbswgfp.html

[S13] C：宏定义
来源：http://hz.hysaishi.cn/gtejkpjvsn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.aizwys.cn/gtbtmeiszf.html

[S14] C：枚举
来源：http://hz.zdqjudy.top/gtixhelxfn.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.wangdashe.top/gtwzxikomo.html

[S15] C：类型转换
来源：http://hz.aibaodan.cn/gthqupkwee.html

(double) a / b
来源：http://hz.dashuyun.cn/gtahxvzrpf.html

[S16] C：位操作置位
来源：http://hz.jlsjyb.cn/gtiwqnhohf.html

x |= (1 << 3);
来源：http://hz.yanxiufei.cn/gtfwoenkkk.html

[S17] C：安全拼接字符串
来源：http://hz.dianchejie.cn/gtztmnetzq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.aizwys.cn/gtukpwtpry.html

[S18] C：命令行参数
来源：http://hz.yanxiufei.cn/gtbjupemos.html

int main(int argc, char **argv)
来源：http://hz.xinyue.icu/gtyzxyncpl.html

[S19] C：快速排序
来源：http://hz.cucudq.cn/gtosknmlzs.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.chenjidiqi.icu/gtxhmloqsw.html

[S20] C：二分查找
来源：http://hz.cheryme.top/gthlpuwqfi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.snrcjt.cn/gtsatewuks.html

[S21] C：字符类别判断
来源：http://hz.0kj1m.cn/gtjdngdkvn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ydjk.org.cn/gtumxqhwik.html

[S22] C：字符串转数字
来源：http://hz.yanxiufei.cn/gtvrmuxspp.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yueranfly.top/gtmwvsngsq.html

[S23] C：随机数
来源：http://hz.zhongyouzk.top/gtaxwojdba.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yongpay.top/gthhbchiif.html

[S24] C：获取本地时间
来源：http://hz.tanke756.top/gtrxttcszh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jianghu66.top/gtcxbnzips.html

[S25] C：内存拷贝
来源：http://hz.yonumen.top/gtmgeqmrdy.html

memcpy(dst, src, n);
来源：http://hz.vqdsnc.cn/gtnxudarfq.html

[S26] C：内存清零
来源：http://hz.wangshuangyany.cn/gtaerxmfzw.html

memset(a, 0, sizeof a);
来源：http://hz.jinqigfzy.top/gtvrqdymwa.html

[S27] C：定义常量
来源：http://hz.yj202588.top/gtisliqokz.html

const double PI = 3.14159;
来源：http://hz.shangyingyoupin.top/gtdwzrjito.html

[S28] C：静态变量
来源：http://hz.daxiang520.top/gtikizlbow.html

static int counter = 0;
来源：http://hz.xylfe.cn/gtieegehaq.html

[S29] C：变参函数
来源：http://hz.316326.xyz/gthjdgddbl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.guannengcc.top/gtyzmmjlwp.html

[S30] C：头文件保护
来源：http://hz.birdmap.top/gtzjlsudhj.html

#ifndef X_H
来源：http://hz.yuxming.cn/gtflifjgim.html

#define X_H
来源：http://hz.sweek.top/gtcimoqcyz.html

#endif
来源：http://hz.zhijiandao.cn/gtoifbukkq.html

[S31] C++：Hello World
来源：http://hz.yj202588.top/gtpsikfxvg.html

#include <iostream>
来源：http://hz.redwolf501.top/gtvskluktm.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.tianlin.xyz/gtfqucswjt.html

[S32] C++：字符串
来源：http://hz.hysaishi.cn/gtlhipfbhf.html

std::string s = "hi";  s += "!";
来源：http://hz.daria6918.cn/gtnpnngesf.html

[S33] C++：vector 增删
来源：http://hz.andypj.xyz/gtmjbxvhmx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hnqzz.top/gtapswtrmw.html

[S34] C++：遍历 vector
来源：http://hz.cucudq.cn/gtlscwiyld.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.smart0.xyz/gthvcwjgyb.html

[S35] C++：map
来源：http://hz.yj20258888.top/gtxnyzwiei.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.c1oappe.top/gtpxcarbwu.html

[S36] C++：unordered_map
来源：http://hz.xinyue.icu/gteawqexlo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shangyingyoupin.top/gtitadfqxp.html

[S37] C++：set
来源：http://hz.shuidangran.top/gthlwfzzto.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhijiandao.cn/gtwczucmyw.html

[S38] C++：排序
来源：http://hz.gotoacloud.top/gtybkwoqdu.html

std::sort(v.begin(), v.end());
来源：http://hz.shanyushiyangtech.top/gtfddojpoj.html

[S39] C++：自定义比较器排序
来源：http://hz.gaohongyu789.top/gtzgfwwais.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.cdnleiting.top/gttbmyreig.html

[S40] C++：查找元素
来源：http://hz.zhengqikj.top/gteuhtysij.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.cqqwz.cn/gtmoyeszdj.html

[S41] C++：类与构造函数
来源：http://hz.yj202588.top/gtxasfowud.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jiagoushi.top/gtjysuvsmo.html

[S42] C++：继承与虚函数
来源：http://hz.xylfe.cn/gtjgiudzqr.html

class B : public Base { public: void f() override {} };
来源：http://hz.0kj1m.cn/gtkpsmrlps.html

[S43] C++：智能指针
来源：http://hz.tianlin.xyz/gtirzbundb.html

auto p = std::make_unique<int>(5);
来源：http://hz.yonumen.top/gthbdiznby.html

[S44] C++：引用传参
来源：http://hz.hongshengwenyu.top/gtglyfecga.html

void inc(int &x) { ++x; }
来源：http://hz.316326.xyz/gtdfkfvvuv.html

[S45] C++：lambda
来源：http://hz.yanxiufei.cn/gtfvhcvdoy.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hammf.cn/gtyprpbzwb.html

[S46] C++：函数模板
来源：http://hz.hnxiangtu.top/gtjjrsladm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yj20258.top/gtuzwyyjkx.html

[S47] C++：结构化绑定遍历
来源：http://hz.iojbl.cn/gtuafonmkm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.0kj1m.cn/gtyfftjkdh.html

[S48] C++：逐行读文件
来源：http://hz.wangshuangyany.cn/gtikowlvzu.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shanyushiyangtech.top/gtufymjuvp.html

while (std::getline(in, line)) { }
来源：http://hz.gotoacloud.top/gtsqhlkvxo.html

[S49] C++：写文件
来源：http://hz.yuanzhike.top/gtxvnfcuko.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.0kj1m.cn/gtxbghvcsr.html

[S50] C++：格式化数字
来源：http://hz.52xcode.cn/gtrprpslbm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yangfankeji.com/gtojqjpyrx.html

[S51] C++：显式类型转换
来源：http://hz.sysykeji.top/gtoycyozkf.html

static_cast<double>(a) / b
来源：http://hz.wangshuangyany.cn/gtkzgrmcne.html

[S52] C++：const 与 noexcept
来源：http://hz.nanxuanxn.top/gtaahsdshk.html

int size() const noexcept { return n_; }
来源：http://hz.316326.xyz/gtqkfxmlfw.html

[S53] C++：移动语义
来源：http://hz.zhijiandao.cn/gtoecynrvz.html

std::vector<int> w = std::move(v);
来源：http://hz.shuidangran.top/gtxbrtebtk.html

[S54] C++：异常处理
来源：http://hz.yangfankeji.com/gtspgmsvkq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.bjfxy.top/gtrwmpbdtl.html

[S55] C++：结构化绑定
来源：http://hz.jinqigfzy.top/gteanwqeyt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.daxiang520.top/gtjeknzfbe.html

[S56] C++：optional
来源：http://hz.yanxiufei.cn/gtkwoxeshq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.cdnleiting.top/gtganqtaso.html

[S57] C++：编译期常量
来源：http://hz.zhaomingkeji.xyz/gtlauxjawu.html

constexpr int N = 10;
来源：http://hz.wangshuangyany.cn/gtuvqzived.html

[S58] C++：命名空间
来源：http://hz.xuanzx.com/gtiuftppue.html

namespace ns { int f() { return 1; } }
来源：http://hz.dashuyun.cn/gtwpfwogjm.html

[S59] C++：静态断言
来源：http://hz.redwolf501.top/gtmivywwfn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yangfankeji.com/gtcvsficeq.html

[S60] C++：遍历并删除元素
来源：http://hz.0kj1m.cn/gtascentdq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.shzxlz.cn/gtmwozgham.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtbtjrzlqt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.dashuyun.cn/gtgjkqbrhi.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtpnjuwtvz.html

[T01] Kotlin：Hello World
来源：http://hz.guowangkeji.top/gtdbbxfzsf.html

println("Hello")
来源：http://hz.yj20258.top/gtgyinexwe.html

[T02] Kotlin：变量
来源：http://hz.hywenlv.cn/gtewifijik.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhiwuduotai.top/gtjaqikmvj.html

[T03] Kotlin：字符串模板
来源：http://hz.52xcode.cn/gtkphpxkgy.html

"值: $b"
来源：http://hz.svipenyu.cn/gtdukyfnqw.html

[T04] Kotlin：空安全
来源：http://hz.hnxiangtu.top/gtwxlrjusz.html

val n: String? = null;  n?.length
来源：http://hz.guannengcc.top/gtxpdcujdf.html

[T05] Kotlin：when 表达式
来源：http://hz.xylfe.cn/gtvrgqkxut.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.birdmap.top/gtibscmiyj.html

[T06] Kotlin：集合映射
来源：http://hz.cdnleiting.top/gtggpjyamv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.gaohongyu789.top/gtngrwriju.html

[T07] Kotlin：集合过滤
来源：http://hz.hammf.cn/gtshhrzndp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.ehwqpu.com/gtenldfngb.html

[T08] Kotlin：数据类
来源：http://hz.xinyue.icu/gtteeojmir.html

data class User(val name: String, val age: Int)
来源：http://hz.hfpthk.cn/gtpznijkba.html

[T09] Kotlin：扩展函数
来源：http://hz.yangfankeji.com/gtvimeknke.html

fun String.exclaim() = this + "!"
来源：http://hz.shangyingyoupin.top/gtpwpwdzap.html

[T10] Kotlin：默认参数
来源：http://hz.redwolf501.top/gtpxsxtlsd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.svipenyu.cn/gtainavulq.html

[T11] Kotlin：协程
来源：http://hz.ydzc1.top/gtwuajewua.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.aibaodan.cn/gtiuwpujow.html

[T12] Kotlin：解构声明
来源：http://hz.cheryme.top/gtdojvebpb.html

val (a, b) = Pair(1, 2)
来源：http://hz.yuanzhike.top/gtvupfmeic.html

[T13] Kotlin：只读 Map
来源：http://hz.havefunace.top/gtolgksnar.html

val m = mapOf("a" to 1)
来源：http://hz.xziqi.cn/gtpfnzgwmd.html

[T14] Kotlin：循环
来源：http://hz.tian-w.cn/gtyflkrsni.html

for (i in 1..10) println(i)
来源：http://hz.zhongyouzk.top/gtknlocibg.html

[T15] Kotlin：接口
来源：http://hz.gogol.net.cn/gtyzojunji.html

interface Shape { fun area(): Double }
来源：http://hz.fzhhl.top/gtlcbpctdv.html

[T16] Swift：Hello World
来源：http://hz.xylfe.cn/gtsywxkadl.html

print("Hello")
来源：http://hz.zhoulong.xyz/gtorltarvq.html

[T17] Swift：变量与常量
来源：http://hz.daria6918.cn/gtnfnwnndi.html

var a = 1;  let b = 2
来源：http://hz.jinqigfzy.top/gtkggtpqvz.html

[T18] Swift：字符串插值
来源：http://hz.yueranfly.top/gtrpdbijjw.html

"值: \(b)"
来源：http://hz.yonumen.top/gtslehcwjq.html

[T19] Swift：可选绑定
来源：http://hz.shanyushiyangkeji.top/gtaknhdzjo.html

if let n = opt { print(n) }
来源：http://hz.ybcxt.top/gtrnnapavy.html

[T20] Swift：数组操作
来源：http://hz.zhaomingkeji.xyz/gtxckhdexa.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jiagoushi.top/gtckxuytyx.html

[T21] Swift：遍历
来源：http://hz.sxryk.cn/gtukflodgz.html

for x in a { print(x) }
来源：http://hz.meibo888.top/gtozsoopit.html

[T22] Swift：字典
来源：http://hz.wangdashe.top/gtmrukxwef.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.sufxvd.cn/gtsfyhgujg.html

[T23] Swift：函数
来源：http://hz.chenzaomai.com/gtyuwaelrk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.nanxuanxn.top/gtxqghqbwa.html

[T24] Swift：闭包
来源：http://hz.yonumen.top/gtqgpejqkj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.shanyushiyangkeji.top/gteqaaeaab.html

[T25] Swift：结构体
来源：http://hz.smart0.xyz/gtkqsvxypa.html

struct P { var x: Int }
来源：http://hz.cqqwz.cn/gtnvfdwype.html

[T26] Swift：类与重写
来源：http://hz.smart0.xyz/gtzjriayjm.html

class A: Base { override func f() {} }
来源：http://hz.zycfv.cn/gtvojspvfv.html

[T27] Swift：错误处理
来源：http://hz.yangfankeji.com/gtwqggwlxj.html

do { try f() } catch { print(error) }
来源：http://hz.shanyushiyangkeji.top/gtnfeivxtm.html

[T28] Swift：枚举
来源：http://hz.yongpay.top/gtdldmvqzt.html

enum Color { case red, green }
来源：http://hz.cashguo.top/gtdmkxangq.html

[T29] Swift：guard 提前返回
来源：http://hz.shanyushiyangkeji.top/gtborcdjfr.html

guard let x = opt else { return }
来源：http://hz.andypj.xyz/gtqndsmitv.html

[T30] Swift：协议
来源：http://hz.ehwqpu.com/gtjznapdbw.html

protocol Shape { func area() -> Double }
来源：http://hz.yangfankeji.com/gtoumynmah.html

[T31] Lua：Hello World
来源：http://hz.cheryme.top/gtxmjmqfgj.html

print("Hello")
来源：http://hz.svipenyu.cn/gtfqtzjlci.html

[T32] Lua：局部变量
来源：http://hz.sxryk.cn/gtmuivrjtl.html

local a = 1
来源：http://hz.nwbrower.top/gtsvdbqymb.html

[T33] Lua：表（数组）
来源：http://hz.zhijiandao.cn/gthrbsyycn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jinqigfzy.top/gtqsqnomqm.html

[T34] Lua：遍历表
来源：http://hz.sweek.top/gtwywcshsm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.ywan-chungtsiang.top/gtvjzfvtli.html

[T35] Lua：字典表
来源：http://hz.zhaomingkeji.xyz/gtnbankpvn.html

local d = { a = 1 };  d.b = 2
来源：http://hz.0kj1m.cn/gtkimjawlz.html

[T36] Lua：函数
来源：http://hz.gotoacloud.top/gtrdsfbksl.html

function add(a, b) return a + b end
来源：http://hz.dianchejie.cn/gtdtqkjvbl.html

[T37] Lua：字符串拼接
来源：http://hz.gotoacloud.top/gtiacyuael.html

"a" .. "b"
来源：http://hz.cucudq.cn/gtbwkidqnm.html

[T38] Lua：条件
来源：http://hz.yj202588.top/gtiviegjwf.html

if x > 0 then print("正") end
来源：http://hz.cdnleiting.top/gttaefonca.html

[T39] Lua：模式匹配
来源：http://hz.jqgufenzy.top/gtesnjigpx.html

string.find(s, "%d+")
来源：http://hz.birdmap.top/gtzlcbgfwq.html

[T40] Lua：元表
来源：http://hz.ivvv.top/gtruzojtcx.html

setmetatable({}, { __index = base })
来源：http://hz.cashguo.top/gtquylcfcx.html

[T41] Perl：Hello World
来源：http://hz.dashuyun.cn/gtfiipfcop.html

print "Hello\n";
来源：http://hz.yuanzhike.top/gtbsfyxhkt.html

[T42] Perl：变量类型
来源：http://hz.gogol.net.cn/gtilokoyov.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zhengqikj.top/gtivmcbyfw.html

[T43] Perl：字符串插值
来源：http://hz.gotoacloud.top/gtojbojxwg.html

"值: $a"
来源：http://hz.birdmap.top/gtfvnpixwz.html

[T44] Perl：条件
来源：http://hz.jyoumei.cn/gthjiyccta.html

if ($a > 0) { print "正"; }
来源：http://hz.cashguo.top/gtyorsrhrh.html

[T45] Perl：数组遍历
来源：http://hz.xuetiantiany.cn/gtkqwopfks.html

for my $x (@arr) { print $x; }
来源：http://hz.bjfxy.top/gtdlicefsj.html

[T46] Perl：哈希操作
来源：http://hz.ehwqpu.com/gtsaieieqx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.bjfxy.top/gtvrjmrllm.html

[T47] Perl：正则捕获
来源：http://hz.shuidangran.top/gtsjdswoqr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.cqqwz.cn/gtmmiqwbta.html

[T48] Perl：正则替换
来源：http://hz.wangdashe.top/gtomfidyxh.html

$s =~ s/old/new/g;
来源：http://hz.zhijiandao.cn/gtjgyvhrhj.html

[T49] Perl：函数
来源：http://hz.chenzaomai.com/gtnpstlach.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.ydjk.org.cn/gtnpdyptuh.html

[T50] Perl：逐行读文件
来源：http://hz.redwolf501.top/gtgobwbtar.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jiagoushi.top/gtbfbgyifu.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.aizwys.cn/gtliqwjixc.html

[T51] Scala：Hello World
来源：http://hz.yj20258.top/gtcqywcpfg.html

println("Hello")
来源：http://hz.gotoacloud.top/gtxjlghunh.html

[T52] Scala：变量
来源：http://hz.dashuyun.cn/gtqovatgqb.html

val a = 1;  var b = 2
来源：http://hz.ppjwa.cn/gtoquykkan.html

[T53] Scala：字符串插值
来源：http://hz.shanyushiyangtech.top/gtbtzfhvce.html

s"值: $b"
来源：http://hz.jqgfzy.top/gtaphiyssy.html

[T54] Scala：集合映射
来源：http://hz.tian-w.cn/gtoixkibdh.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.jinqigfzy.top/gtccgnzlvx.html

[T55] Scala：集合过滤
来源：http://hz.jiagoushi.top/gtqczzvshf.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.zdqjudy.top/gtmmgdazbd.html

[T56] Scala：样例类
来源：http://hz.gzhubu.top/gtadqrmygo.html

case class User(name: String, age: Int)
来源：http://hz.quarkkingdee.top/gtmenpjjea.html

[T57] Scala：模式匹配
来源：http://hz.yj202588.top/gtqzpoporc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.tian-w.cn/gtcilddgzf.html

[T58] Scala：函数定义
来源：http://hz.feifeiyinyue.top/gtbgsvnkix.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.shanyushiyangtech.top/gtuezbemdw.html

[T59] Scala：循环
来源：http://hz.ybcxt.top/gtfkfqgofe.html

for (i <- 1 to 10) println(i)
来源：http://hz.jinghuilouyu.cn/gtooqsqcjr.html

[T60] Scala：折叠
来源：http://hz.gogol.net.cn/gtxvkivwct.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yuanzhike.top/gtlacgxhob.html

================================================================================
来源：http://hz.jinqigufen.top/gtormxxgol.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.kuanghao11.cn/gtwuorqcyy.html

================================================================================
来源：http://hz.ppjwa.cn/gtckbqikys.html

[U01] Py：创建虚拟环境
来源：http://hz.shuidangran.top/gtdjaujrte.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.birdmap.top/gtykewsnvu.html

[U02] Py：导出 / 安装依赖
来源：http://hz.shanyushiyangtech.top/gtmsfddafq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.zhiwuduotai.top/gtovjyzqzc.html

[U03] Py：加载 .env 配置
来源：http://hz.jinqigufen.top/gtkqwyctod.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yj20258.top/gtnmvlnhsu.html

[U04] Py：变量调试打印
来源：http://hz.daria6918.cn/gtazsgqsbq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zdqjudy.top/gtsagfdess.html

[U05] Py：列表去重且保序
来源：http://hz.tianlin.xyz/gtzmuyeszq.html

list(dict.fromkeys(arr))
来源：http://hz.quarkkingdee.top/gtgesiwcjj.html

[U06] Py：合并两个字典
来源：http://hz.shangyingyoupin.top/gtuldvmsgc.html

{**a, **b}
来源：http://hz.nanxinkj.top/gtuwkdmuhq.html

[U07] Py：反转字典键值
来源：http://hz.chenjidiqi.icu/gtlwecaoqk.html

{v: k for k, v in d.items()}
来源：http://hz.guannengcc.top/gtomuwdvbn.html

[U08] Py：展平二维列表
来源：http://hz.kuanghao11.cn/gtctthtikz.html

[y for x in nested for y in x]
来源：http://hz.sweek.top/gtnmnspkuw.html

[U09] Py：字典取最大值的键
来源：http://hz.cheryme.top/gtvtrlvcvg.html

max(d, key=d.get)
来源：http://hz.ppjwa.cn/gtuyuzppiu.html

[U10] Py：按值排序字典
来源：http://hz.hfpthk.cn/gtmkwkuzfv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.svipenyu.cn/gttgahzrqt.html

[U11] Py：生成器表达式
来源：http://hz.yuanzhike.top/gtdramtprn.html

(x * 2 for x in arr)
来源：http://hz.c1oappe.top/gtxqvounwn.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.jinqigfzy.top/gtxmarlkno.html

Counter(arr).most_common(3)
来源：http://hz.meibo888.top/gtbvbgdyhu.html

[U13] Py：固定长度队列
来源：http://hz.jlsjyb.cn/gtokbmcymk.html

deque(maxlen=10)
来源：http://hz.fzhhl.top/gttqbutqif.html

[U14] Py：分组收集到列表
来源：http://hz.daria6918.cn/gtcniadzee.html

defaultdict(list)
来源：http://hz.yuxming.cn/gtwnlofozc.html

[U15] Py：高精度计时
来源：http://hz.aizwys.cn/gtivicfepb.html

t = time.perf_counter()
来源：http://hz.haohaochexian.top/gteorhqwxe.html

[U16] Py：命令行参数解析
来源：http://hz.jqgufenzy.top/gtnvdzkwpy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.ywan-chungtsiang.top/gtskdkdptt.html

[U17] Py：初始化日志
来源：http://hz.zhengqikj.top/gtuxlrtelu.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yanxiufei.cn/gthgmhwsan.html

[U18] Py：预编译正则
来源：http://hz.ybcxt.top/gtwhnhlecf.html

pat = re.compile(r"\d+")
来源：http://hz.smart0.xyz/gtdaotytvr.html

[U19] Py：正则替换带回调
来源：http://hz.aizwys.cn/gtmsqldagg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.ivvv.top/gtnoqjtpck.html

[U20] Py：缓存函数结果
来源：http://hz.daria6918.cn/gtlnahsfyy.html

@functools.lru_cache(maxsize=None)
来源：http://hz.tianlin.xyz/gtvpfjcdpg.html

[U21] Py：自定义上下文管理器
来源：http://hz.ywan-chungtsiang.top/gtnfjbgavz.html

@contextlib.contextmanager
来源：http://hz.redwolf501.top/gtllbhtrua.html

[U22] Py：矩阵转置
来源：http://hz.shanyushiyangkeji.top/gtsupkdndb.html

list(zip(*m))
来源：http://hz.hongshengwenyu.top/gtqmmkddrk.html

[U23] Py：分块读取大文件
来源：http://hz.xuetiantiany.cn/gtjnktcewh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.gogol.net.cn/gtqhqzshql.html

[U24] Py：路径操作
来源：http://hz.andypj.xyz/gtvxwmlyuj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.chenjidiqi.icu/gtuhhnpojm.html

[U25] Py：CSV 按字典读
来源：http://hz.cheryme.top/gthbcydjav.html

csv.DictReader(f)
来源：http://hz.yvedp.cn/gthpzorgho.html

[U26] Py：并发下载
来源：http://hz.yj20258888.top/gtvsqzxshc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.zhixingplan.top/gtcicpwhxq.html

[U27] Py：异步 HTTP
来源：http://hz.gzhubu.top/gttkrofqxw.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.316326.xyz/gtstlksqjk.html

[U28] Py：类型别名
来源：http://hz.zdqjudy.top/gtzxlforsb.html

UserId = int
来源：http://hz.jinyuanbaomall.cn/gtqfpdxuwu.html

[U29] Py：属性校验
来源：http://hz.yanxiufei.cn/gtfolqyuof.html

@property 与 @x.setter 配合
来源：http://hz.daria6918.cn/gticdvcvsf.html

[U30] Py：数据类
来源：http://hz.zdqjudy.top/gtjntpowga.html

@dataclass(slots=True)
来源：http://hz.gotoacloud.top/gtmvlaguwn.html

[U31] Py：单测
来源：http://hz.aibaodan.cn/gtiycagtje.html

python -m pytest -q
来源：http://hz.aibaodan.cn/gtctxjrllk.html

[U32] Py：代码格式化
来源：http://hz.wangshuangyany.cn/gtsqnvjcoj.html

ruff format . && ruff check --fix .
来源：http://hz.gotoacloud.top/gtxpoenluu.html

[U33] Py：打包发布
来源：http://hz.sweek.top/gtgvkwmnil.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.sysykeji.top/gtfmtloguy.html

[U34] Py：判断编码
来源：http://hz.cdnleiting.top/gtdrkrvgbg.html

chardet.detect(raw)
来源：http://hz.yueranfly.top/gtghgrsfdo.html

[U35] Py：发送邮件
来源：http://hz.hfpthk.cn/gtnuwnmlde.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.bjfxy.top/gtecjrvgfe.html

[U36] Py：定时任务
来源：http://hz.zhaomingkeji.xyz/gtlztpcvoo.html

schedule.every(10).minutes.do(job)
来源：http://hz.zhongyouzk.top/gtxdfatzsz.html


<!-- 参考信息 -->