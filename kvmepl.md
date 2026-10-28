代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.snrcjt.cn/gtvqrsgfzu.html

[S10] C：指针与解引用
来源：http://hz.kuanghao11.cn/gtfxgrwrqd.html

int *p = &a;  *p = 5;
来源：http://hz.chenlongwang.top/gtvmptgyer.html

[S11] C：逐行读文件
来源：http://hz.shanyushiyangtech.top/gtysqpsimr.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jqgufenzy.top/gtbuzzutrp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.9152youxi.cn/gtxjtohsaz.html

fclose(f);
来源：http://hz.gaohongyu789.top/gtaqsrouhx.html

[S12] C：写文件
来源：http://hz.yj20258888.top/gtauuwwbqd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zycfv.cn/gtetitlriw.html

[S13] C：宏定义
来源：http://hz.dashuyun.cn/gttukymsmi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.9152youxi.cn/gtimfqvqoe.html

[S14] C：枚举
来源：http://hz.0kj1m.cn/gtpgyjlftp.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.shangyingyoupin.top/gtuwdzbump.html

[S15] C：类型转换
来源：http://hz.yanxiufei.cn/gtukcafysv.html

(double) a / b
来源：http://hz.dianchejie.cn/gtyjqdhwdr.html

[S16] C：位操作置位
来源：http://hz.hnxiangtu.top/gtblredjoa.html

x |= (1 << 3);
来源：http://hz.sweek.top/gtoupmpgmp.html

[S17] C：安全拼接字符串
来源：http://hz.jlsjyb.cn/gtncqwankk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.dashuyun.cn/gtyxkegihf.html

[S18] C：命令行参数
来源：http://hz.wangdashe.top/gtlsfebjnf.html

int main(int argc, char **argv)
来源：http://hz.sweek.top/gtitjmztbc.html

[S19] C：快速排序
来源：http://hz.chenlongwang.top/gtjlifqapt.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yvedp.cn/gttqprlmkn.html

[S20] C：二分查找
来源：http://hz.xuanzx.com/gtgzyumunh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.shanyushiyangkeji.top/gtfvjmrqbm.html

[S21] C：字符类别判断
来源：http://hz.chenjidiqi.icu/gtglrlqhwb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.kuanghao11.cn/gtgtrbchfv.html

[S22] C：字符串转数字
来源：http://hz.sxryk.cn/gttnaugigt.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.nwbrower.top/gtigyfqeay.html

[S23] C：随机数
来源：http://hz.wangshuangyany.cn/gtcslevwhx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yangfankeji.com/gtcnskmgiw.html

[S24] C：获取本地时间
来源：http://hz.jlsjyb.cn/gttwcvohww.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ywan-chungtsiang.top/gtsknjdqgu.html

[S25] C：内存拷贝
来源：http://hz.wangshuangyany.cn/gtzzvybvrg.html

memcpy(dst, src, n);
来源：http://hz.yj20258888.top/gtewmqzudj.html

[S26] C：内存清零
来源：http://hz.sweek.top/gthyekdypr.html

memset(a, 0, sizeof a);
来源：http://hz.zdqjudy.top/gtrxmnrzfl.html

[S27] C：定义常量
来源：http://hz.haohaochexian.top/gtcoihyykw.html

const double PI = 3.14159;
来源：http://hz.yangfankeji.com/gtcunqxicj.html

[S28] C：静态变量
来源：http://hz.chenjidiqi.icu/gtbbrangox.html

static int counter = 0;
来源：http://hz.kuanghao11.cn/gtrzmbjymk.html

[S29] C：变参函数
来源：http://hz.ehwqpu.com/gtprxhzpxk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.pengpengdd.cyou/gtydyeqcel.html

[S30] C：头文件保护
来源：http://hz.zhengqikj.top/gtvyvysteu.html

#ifndef X_H
来源：http://hz.zhiwuduotai.top/gtjmowfqzs.html

#define X_H
来源：http://hz.ybcxt.top/gtyuecxfsr.html

#endif
来源：http://hz.sufxvd.cn/gtzilvhojc.html

[S31] C++：Hello World
来源：http://hz.zdqjudy.top/gtwyiwzjel.html

#include <iostream>
来源：http://hz.feifeiyinyue.top/gtseknwgsd.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.chenlongwang.top/gtuoqdxmqs.html

[S32] C++：字符串
来源：http://hz.chenlongwang.top/gtdaidhcnd.html

std::string s = "hi";  s += "!";
来源：http://hz.redwolf501.top/gtcvbnkggu.html

[S33] C++：vector 增删
来源：http://hz.zhaomingkeji.xyz/gtljqaxbco.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.birdmap.top/gtbxmogszj.html

[S34] C++：遍历 vector
来源：http://hz.mhx1999.top/gtdcjehigr.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hongshengwenyu.top/gttnqnsoxo.html

[S35] C++：map
来源：http://hz.nanxinkj.top/gtulalnyiu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hfpthk.cn/gtlfcrzwvp.html

[S36] C++：unordered_map
来源：http://hz.quarkkingdee.top/gtxgwlnokf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tianlin.xyz/gtcsinbler.html

[S37] C++：set
来源：http://hz.0kj1m.cn/gtgufwnizz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yanxiufei.cn/gtpqbukdfn.html

[S38] C++：排序
来源：http://hz.yongpay.top/gtaruiwybm.html

std::sort(v.begin(), v.end());
来源：http://hz.yanxiufei.cn/gtwshdfpdv.html

[S39] C++：自定义比较器排序
来源：http://hz.shanyushiyangtech.top/gthdjsdbqt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.316326.xyz/gtlhrfxzli.html

[S40] C++：查找元素
来源：http://hz.zdqjudy.top/gtuoooegge.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.cdnleiting.top/gtlabuswmi.html

[S41] C++：类与构造函数
来源：http://hz.pengpengdd.cyou/gtpraeqakk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yueranfly.top/gtvrhgzrzm.html

[S42] C++：继承与虚函数
来源：http://hz.jyoumei.cn/gtyqkavbuv.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhoulong.xyz/gtjhpwpaja.html

[S43] C++：智能指针
来源：http://hz.sweek.top/gthtpqgofv.html

auto p = std::make_unique<int>(5);
来源：http://hz.ppjwa.cn/gtygyvechg.html

[S44] C++：引用传参
来源：http://hz.quarkkingdee.top/gtpidatsdm.html

void inc(int &x) { ++x; }
来源：http://hz.shangyingyoupin.top/gtutjtqhhx.html

[S45] C++：lambda
来源：http://hz.ivvv.top/gtccpunoke.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhixingplan.top/gtwoihcezn.html

[S46] C++：函数模板
来源：http://hz.nanxinkj.top/gtwmelmrre.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.haohaochexian.top/gtagnnhufv.html

[S47] C++：结构化绑定遍历
来源：http://hz.yanxiufei.cn/gtbkudvcii.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.chenjidiqi.icu/gtnyihnhez.html

[S48] C++：逐行读文件
来源：http://hz.quarkkingdee.top/gtehbtyhbe.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jinqigufen.top/gtzmgiiesc.html

while (std::getline(in, line)) { }
来源：http://hz.yvedp.cn/gtqicvmnzn.html

[S49] C++：写文件
来源：http://hz.haohaochexian.top/gthdnrxqun.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhengqikj.top/gttgcfaufg.html

[S50] C++：格式化数字
来源：http://hz.jinqigfzy.top/gtlxoeneni.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yuanzhike.top/gtkdfbqrnz.html

[S51] C++：显式类型转换
来源：http://hz.zhengqikj.top/gtyptvtyik.html

static_cast<double>(a) / b
来源：http://hz.sxryk.cn/gtbbugnbcx.html

[S52] C++：const 与 noexcept
来源：http://hz.jqgfzy.top/gteimczfnj.html

int size() const noexcept { return n_; }
来源：http://hz.cqqwz.cn/gtcvasujxs.html

[S53] C++：移动语义
来源：http://hz.dashuyun.cn/gtkgqipnsb.html

std::vector<int> w = std::move(v);
来源：http://hz.xuanzx.com/gtawqtpwyy.html

[S54] C++：异常处理
来源：http://hz.wangdashe.top/gtipeomqtn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.dianchejie.cn/gtwomxamef.html

[S55] C++：结构化绑定
来源：http://hz.hywenlv.cn/gtgwxatfpd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.tian-w.cn/gtoilweesc.html

[S56] C++：optional
来源：http://hz.chenlongwang.top/gtpinnpece.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yangfankeji.com/gtgkyiswdg.html

[S57] C++：编译期常量
来源：http://hz.vqdsnc.cn/gtanljayox.html

constexpr int N = 10;
来源：http://hz.shangyingyoupin.top/gtymcudmts.html

[S58] C++：命名空间
来源：http://hz.jqgfzy.top/gtszjcfiiz.html

namespace ns { int f() { return 1; } }
来源：http://hz.bjfxy.top/gtxwownglu.html

[S59] C++：静态断言
来源：http://hz.gotoacloud.top/gtloiauhep.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yanxiufei.cn/gtomlijpog.html

[S60] C++：遍历并删除元素
来源：http://hz.yonumen.top/gtitfchlqh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.mhx1999.top/gtorpnhtfw.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtcbsvwpal.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhijiandao.cn/gtxipbluzx.html

================================================================================
来源：http://hz.jyoumei.cn/gtkxesccae.html

[T01] Kotlin：Hello World
来源：http://hz.wangdashe.top/gtrtjokrox.html

println("Hello")
来源：http://hz.yuxming.cn/gtnjsiepbx.html

[T02] Kotlin：变量
来源：http://hz.9152youxi.cn/gtfamtlozp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yonumen.top/gtzdkzqbfd.html

[T03] Kotlin：字符串模板
来源：http://hz.yuanzhike.top/gtjuliztmj.html

"值: $b"
来源：http://hz.cheryme.top/gtzbompnrj.html

[T04] Kotlin：空安全
来源：http://hz.0kj1m.cn/gtrcbwernr.html

val n: String? = null;  n?.length
来源：http://hz.jinghuilouyu.cn/gtxjkkdtdp.html

[T05] Kotlin：when 表达式
来源：http://hz.mhx1999.top/gtyrjwthjq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.xuetiantiany.cn/gtscuxfrei.html

[T06] Kotlin：集合映射
来源：http://hz.snrcjt.cn/gtcvecskxc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.wangshuangyany.cn/gtsetaysdc.html

[T07] Kotlin：集合过滤
来源：http://hz.hnqzz.top/gtmccecwid.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.gogol.net.cn/gtpxlgprds.html

[T08] Kotlin：数据类
来源：http://hz.jqgufenzy.top/gtaqaevgba.html

data class User(val name: String, val age: Int)
来源：http://hz.gzhubu.top/gtyjbxavtw.html

[T09] Kotlin：扩展函数
来源：http://hz.pengpengdd.cyou/gtdyvezixt.html

fun String.exclaim() = this + "!"
来源：http://hz.havefunace.top/gtsibabtgf.html

[T10] Kotlin：默认参数
来源：http://hz.tanke756.top/gtyloojavt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.cashguo.top/gteosfpwjo.html

[T11] Kotlin：协程
来源：http://hz.aizwys.cn/gtyqdubrcc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.hnqzz.top/gtdvfjunog.html

[T12] Kotlin：解构声明
来源：http://hz.yvedp.cn/gtiqcwjcbu.html

val (a, b) = Pair(1, 2)
来源：http://hz.andypj.xyz/gtkfrnhbnc.html

[T13] Kotlin：只读 Map
来源：http://hz.316326.xyz/gtzjmojfab.html

val m = mapOf("a" to 1)
来源：http://hz.birdmap.top/gtozkyzojw.html

[T14] Kotlin：循环
来源：http://hz.smart0.xyz/gtwaryyqbw.html

for (i in 1..10) println(i)
来源：http://hz.daxiang520.top/gtvwdngzai.html

[T15] Kotlin：接口
来源：http://hz.haohaochexian.top/gtumeohxgh.html

interface Shape { fun area(): Double }
来源：http://hz.fengsongda.top/gtwkiclvdu.html

[T16] Swift：Hello World
来源：http://hz.hongshengwenyu.top/gtgdvwijol.html

print("Hello")
来源：http://hz.zhoulong.xyz/gtflkiwpzw.html

[T17] Swift：变量与常量
来源：http://hz.hammf.cn/gtppmtgxls.html

var a = 1;  let b = 2
来源：http://hz.hnqzz.top/gtwhijntnx.html

[T18] Swift：字符串插值
来源：http://hz.jianghu66.top/gtrborzwah.html

"值: \(b)"
来源：http://hz.chenjidiqi.icu/gtqtcesuim.html

[T19] Swift：可选绑定
来源：http://hz.havefunace.top/gtuvxcuhwu.html

if let n = opt { print(n) }
来源：http://hz.yvedp.cn/gtcfydmhtc.html

[T20] Swift：数组操作
来源：http://hz.andypj.xyz/gtblijgekj.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.chenlongwang.top/gtvifutxzp.html

[T21] Swift：遍历
来源：http://hz.shangyingyoupin.top/gtbowurres.html

for x in a { print(x) }
来源：http://hz.hfpthk.cn/gtrcjdijbo.html

[T22] Swift：字典
来源：http://hz.yonumen.top/gtjxzzudpc.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.daria6918.cn/gthyqhsccr.html

[T23] Swift：函数
来源：http://hz.ybcxt.top/gtofdrhpmk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.shangyingyoupin.top/gtqmqkamlb.html

[T24] Swift：闭包
来源：http://hz.gaohongyu789.top/gtzixroazt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jinqigfzy.top/gtpbjegstc.html

[T25] Swift：结构体
来源：http://hz.pengpengdd.cyou/gtkwoivfbl.html

struct P { var x: Int }
来源：http://hz.yanxiufei.cn/gtqebgjsyp.html

[T26] Swift：类与重写
来源：http://hz.c1oappe.top/gtovoikpwc.html

class A: Base { override func f() {} }
来源：http://hz.aizwys.cn/gtyjkurbmu.html

[T27] Swift：错误处理
来源：http://hz.yongpay.top/gtfqzmugzl.html

do { try f() } catch { print(error) }
来源：http://hz.wangshuangyany.cn/gttgxutyyz.html

[T28] Swift：枚举
来源：http://hz.cqqwz.cn/gtzhdwacyb.html

enum Color { case red, green }
来源：http://hz.fzhhl.top/gtcmfmmpoa.html

[T29] Swift：guard 提前返回
来源：http://hz.jianghu66.top/gtegslsaqg.html

guard let x = opt else { return }
来源：http://hz.ydzc1.top/gtnqkbeyvw.html

[T30] Swift：协议
来源：http://hz.snrcjt.cn/gteshdrfnj.html

protocol Shape { func area() -> Double }
来源：http://hz.nwbrower.top/gthvgfxbvf.html

[T31] Lua：Hello World
来源：http://hz.yj20258.top/gtizaytlue.html

print("Hello")
来源：http://hz.jyoumei.cn/gtonafloep.html

[T32] Lua：局部变量
来源：http://hz.yj202588.top/gtidkzldxa.html

local a = 1
来源：http://hz.fengsongda.top/gtjxuezcyp.html

[T33] Lua：表（数组）
来源：http://hz.guannengcc.top/gtxhqdylcy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yongpay.top/gtvhghlgzq.html

[T34] Lua：遍历表
来源：http://hz.xziqi.cn/gtnudumwpc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.gotoacloud.top/gtwvcyscpr.html

[T35] Lua：字典表
来源：http://hz.zhengqikj.top/gtxiwbdrqt.html

local d = { a = 1 };  d.b = 2
来源：http://hz.wangshuangyany.cn/gtmccifdwc.html

[T36] Lua：函数
来源：http://hz.fengsongda.top/gtsqeupgfg.html

function add(a, b) return a + b end
来源：http://hz.gzhubu.top/gtkhgvbdqp.html

[T37] Lua：字符串拼接
来源：http://hz.xingfuxueyuan.xyz/gtrprszyno.html

"a" .. "b"
来源：http://hz.316326.xyz/gtamvfoeij.html

[T38] Lua：条件
来源：http://hz.pengpengdd.cyou/gttkpikiqk.html

if x > 0 then print("正") end
来源：http://hz.c1oappe.top/gtpquynlyw.html

[T39] Lua：模式匹配
来源：http://hz.316326.xyz/gtemonqjyi.html

string.find(s, "%d+")
来源：http://hz.hfpthk.cn/gtlcvsvwyl.html

[T40] Lua：元表
来源：http://hz.redwolf501.top/gttauhvqtg.html

setmetatable({}, { __index = base })
来源：http://hz.yvedp.cn/gtrgihadof.html

[T41] Perl：Hello World
来源：http://hz.iojbl.cn/gtgukblmah.html

print "Hello\n";
来源：http://hz.shzxlz.cn/gtociohjvw.html

[T42] Perl：变量类型
来源：http://hz.guannengcc.top/gttcnpdhju.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.snrcjt.cn/gtjjgbpfgw.html

[T43] Perl：字符串插值
来源：http://hz.shanyushiyangkeji.top/gtgnbtsuhr.html

"值: $a"
来源：http://hz.hysaishi.cn/gtnydaefto.html

[T44] Perl：条件
来源：http://hz.yj20258888.top/gtjpbjyuol.html

if ($a > 0) { print "正"; }
来源：http://hz.jinyuanbaomall.cn/gtyyyxrhia.html

[T45] Perl：数组遍历
来源：http://hz.316326.xyz/gtjfaxflld.html

for my $x (@arr) { print $x; }
来源：http://hz.zhengqikj.top/gtxstmveya.html

[T46] Perl：哈希操作
来源：http://hz.ppjwa.cn/gtjeviahzi.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yueranfly.top/gtonoboxca.html

[T47] Perl：正则捕获
来源：http://hz.gogol.net.cn/gthgbmuflu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.cdnleiting.top/gtwemhmgvq.html

[T48] Perl：正则替换
来源：http://hz.yonumen.top/gtsfqjjfxb.html

$s =~ s/old/new/g;
来源：http://hz.quarkkingdee.top/gtqskvrdxq.html

[T49] Perl：函数
来源：http://hz.chenlongwang.top/gtarayykqe.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.xinyue.icu/gtcdgptpyg.html

[T50] Perl：逐行读文件
来源：http://hz.iojbl.cn/gtmgbdwphz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yj20258.top/gtxrsfhwdk.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.cdnleiting.top/gtlrktcizb.html

[T51] Scala：Hello World
来源：http://hz.jiagoushi.top/gtpontsrnh.html

println("Hello")
来源：http://hz.jianghu66.top/gtjkjabisy.html

[T52] Scala：变量
来源：http://hz.pycfn.com/gtrpoxzyqm.html

val a = 1;  var b = 2
来源：http://hz.pycfn.com/gtovlknjus.html

[T53] Scala：字符串插值
来源：http://hz.nwbrower.top/gtutpjiixz.html

s"值: $b"
来源：http://hz.pengpengdd.cyou/gtnxjxerwx.html

[T54] Scala：集合映射
来源：http://hz.yuanzhike.top/gtdrldpwzt.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.shuidangran.top/gtnlnuhzqe.html

[T55] Scala：集合过滤
来源：http://hz.kuanghao11.cn/gtrgerjrua.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.gotoacloud.top/gtewyrvfhz.html

[T56] Scala：样例类
来源：http://hz.tianlin.xyz/gtvwbjmrjd.html

case class User(name: String, age: Int)
来源：http://hz.xuanzx.com/gtmcwnrijv.html

[T57] Scala：模式匹配
来源：http://hz.xylfe.cn/gtdirnaodr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.chenjidiqi.icu/gtktgnhwqs.html

[T58] Scala：函数定义
来源：http://hz.chenjidiqi.icu/gtnkmiqtat.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.hnxiangtu.top/gtwcysqaxd.html

[T59] Scala：循环
来源：http://hz.yanxiufei.cn/gtdefwyvbn.html

for (i <- 1 to 10) println(i)
来源：http://hz.ppjwa.cn/gtiejjjweh.html

[T60] Scala：折叠
来源：http://hz.hongshengwenyu.top/gtszylkijc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.aizwys.cn/gtodrkafpq.html

================================================================================
来源：http://hz.iojbl.cn/gtiqzziohk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.chenzaomai.com/gtgcwkdyhf.html

================================================================================
来源：http://hz.vqdsnc.cn/gtwoclkozp.html

[U01] Py：创建虚拟环境
来源：http://hz.316326.xyz/gtlfqoskpv.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.shanyushiyangtech.top/gtuguoqmwq.html

[U02] Py：导出 / 安装依赖
来源：http://hz.iojbl.cn/gtamjggpcc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.andypj.xyz/gtukyenunl.html

[U03] Py：加载 .env 配置
来源：http://hz.xinyue.icu/gttqbqzkul.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.sweek.top/gtgcpylqby.html

[U04] Py：变量调试打印
来源：http://hz.ydjk.org.cn/gtpdyeshle.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zhiwuduotai.top/gtoaoxruks.html

[U05] Py：列表去重且保序
来源：http://hz.zhaomingkeji.xyz/gtyguojdrr.html

list(dict.fromkeys(arr))
来源：http://hz.ppjwa.cn/gtnfkbcris.html

[U06] Py：合并两个字典
来源：http://hz.mhx1999.top/gtgentljnd.html

{**a, **b}
来源：http://hz.yj20258888.top/gtgxgakkva.html

[U07] Py：反转字典键值
来源：http://hz.jqgfzy.top/gtjrlecxnn.html

{v: k for k, v in d.items()}
来源：http://hz.cdnleiting.top/gtemetcnpq.html

[U08] Py：展平二维列表
来源：http://hz.jinqigufen.top/gtdrivhuee.html

[y for x in nested for y in x]
来源：http://hz.tanke756.top/gtrpdphdao.html

[U09] Py：字典取最大值的键
来源：http://hz.zhixingplan.top/gtlakztqja.html

max(d, key=d.get)
来源：http://hz.cheryme.top/gtucczkuzo.html

[U10] Py：按值排序字典
来源：http://hz.birdmap.top/gtftgeekdd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.chenlongwang.top/gtvxiqcqdi.html

[U11] Py：生成器表达式
来源：http://hz.svipenyu.cn/gtsbrvhygv.html

(x * 2 for x in arr)
来源：http://hz.xingfuxueyuan.xyz/gtcwnowkjc.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.sysykeji.top/gtvyqammol.html

Counter(arr).most_common(3)
来源：http://hz.hnxiangtu.top/gtaicnglrw.html

[U13] Py：固定长度队列
来源：http://hz.redwolf501.top/gtnnmrrqjw.html

deque(maxlen=10)
来源：http://hz.fengsongda.top/gtrseznfcy.html

[U14] Py：分组收集到列表
来源：http://hz.nanxuanxn.top/gtaopnbesj.html

defaultdict(list)
来源：http://hz.sweek.top/gtxqmlzqag.html

[U15] Py：高精度计时
来源：http://hz.cdnleiting.top/gtwvbxlmaq.html

t = time.perf_counter()
来源：http://hz.chenzaomai.com/gtnmczzqlj.html

[U16] Py：命令行参数解析
来源：http://hz.zhiwuduotai.top/gtpufikeqb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yueranfly.top/gtsddunrzp.html

[U17] Py：初始化日志
来源：http://hz.xuetiantiany.cn/gtbuznvdfk.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.hammf.cn/gthqokvlce.html

[U18] Py：预编译正则
来源：http://hz.pengpengdd.cyou/gtjgvdudge.html

pat = re.compile(r"\d+")
来源：http://hz.hongshengwenyu.top/gtvqmtqaao.html

[U19] Py：正则替换带回调
来源：http://hz.316326.xyz/gtzkbteyri.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.jlsjyb.cn/gtrrptcyoy.html

[U20] Py：缓存函数结果
来源：http://hz.pycfn.com/gtskjjlyla.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yueranfly.top/gtwyvizeax.html

[U21] Py：自定义上下文管理器
来源：http://hz.nanxinkj.top/gtwmqqislk.html

@contextlib.contextmanager
来源：http://hz.52xcode.cn/gtumpzetqb.html

[U22] Py：矩阵转置
来源：http://hz.yvedp.cn/gtgdnxjson.html

list(zip(*m))
来源：http://hz.yj202588.top/gtqkpdvynx.html

[U23] Py：分块读取大文件
来源：http://hz.shuidangran.top/gtfuinqcdk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.ywan-chungtsiang.top/gtycihjzgb.html

[U24] Py：路径操作
来源：http://hz.wangdashe.top/gtqkraunlq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.shanyushiyangtech.top/gtnpaudncw.html

[U25] Py：CSV 按字典读
来源：http://hz.xylfe.cn/gtvfiwchpj.html

csv.DictReader(f)
来源：http://hz.sysykeji.top/gtdfilekwn.html

[U26] Py：并发下载
来源：http://hz.iojbl.cn/gtirhpkoet.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.xylfe.cn/gtwgwwmaqt.html

[U27] Py：异步 HTTP
来源：http://hz.wangdashe.top/gtisdiftah.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.xingfuxueyuan.xyz/gtxebxbdwp.html

[U28] Py：类型别名
来源：http://hz.sxryk.cn/gtqearqjsj.html

UserId = int
来源：http://hz.guannengcc.top/gtgkbormug.html

[U29] Py：属性校验
来源：http://hz.gzhubu.top/gtazoyoizr.html

@property 与 @x.setter 配合
来源：http://hz.mhx1999.top/gtulptknqv.html

[U30] Py：数据类
来源：http://hz.yj20258.top/gtxkuxnyuf.html

@dataclass(slots=True)
来源：http://hz.chenlongwang.top/gtkvcwcnrh.html

[U31] Py：单测
来源：http://hz.yj20258888.top/gtvrrzyvuw.html

python -m pytest -q
来源：http://hz.zhijiandao.cn/gtetjcjtkc.html

[U32] Py：代码格式化
来源：http://hz.xuetiantiany.cn/gtynsobolr.html

ruff format . && ruff check --fix .
来源：http://hz.mhx1999.top/gtyeqjraks.html


<!-- 参考信息 -->