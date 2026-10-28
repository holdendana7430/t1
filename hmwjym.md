代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hnqzz.top/gthmflviwk.html

[S10] C：指针与解引用
来源：http://hz.jlsjyb.cn/gtgxnprnwb.html

int *p = &a;  *p = 5;
来源：http://hz.9152youxi.cn/gtkdnsawmb.html

[S11] C：逐行读文件
来源：http://hz.xinyue.icu/gtthpfqdca.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.hnqzz.top/gtrgtwbfoa.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ehwqpu.com/gtdhkspacd.html

fclose(f);
来源：http://hz.aizwys.cn/gtvyevzzzm.html

[S12] C：写文件
来源：http://hz.shanyushiyangkeji.top/gtlxiarwpq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.haohaochexian.top/gtwbghxnjv.html

[S13] C：宏定义
来源：http://hz.hfpthk.cn/gtjfpfnjho.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.nwbrower.top/gtwryuekpu.html

[S14] C：枚举
来源：http://hz.svipenyu.cn/gtdqhogsyi.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.guowangkeji.top/gtrlyxgoxx.html

[S15] C：类型转换
来源：http://hz.tanke756.top/gttvivtxgs.html

(double) a / b
来源：http://hz.hywenlv.cn/gtobrqsnmn.html

[S16] C：位操作置位
来源：http://hz.meibo888.top/gtqmbdtqxd.html

x |= (1 << 3);
来源：http://hz.aibaodan.cn/gtrtwzkyox.html

[S17] C：安全拼接字符串
来源：http://hz.daria6918.cn/gtlhgfswcm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhijiandao.cn/gtlkzqtgdu.html

[S18] C：命令行参数
来源：http://hz.mhx1999.top/gtcejmkooz.html

int main(int argc, char **argv)
来源：http://hz.hnqzz.top/gtavddudfu.html

[S19] C：快速排序
来源：http://hz.kuanghao11.cn/gtbybilwcx.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.sxryk.cn/gtrmlqaxhv.html

[S20] C：二分查找
来源：http://hz.feifeiyinyue.top/gtcgbhmayk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.kuanghao11.cn/gtlteiqzmj.html

[S21] C：字符类别判断
来源：http://hz.wangshuangyany.cn/gtcufaezgo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.nanxinkj.top/gtptxrfxdv.html

[S22] C：字符串转数字
来源：http://hz.yj20258888.top/gtxoiujlbj.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xuanzx.com/gtcrsdxquh.html

[S23] C：随机数
来源：http://hz.ydzc1.top/gtwanofjko.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.shanyushiyangkeji.top/gtxrmblfts.html

[S24] C：获取本地时间
来源：http://hz.birdmap.top/gtzknmsghc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.guowangkeji.top/gtcdxncihk.html

[S25] C：内存拷贝
来源：http://hz.jqgfzy.top/gtvoqwuulp.html

memcpy(dst, src, n);
来源：http://hz.chenjidiqi.icu/gtqimjkdhr.html

[S26] C：内存清零
来源：http://hz.xinyue.icu/gtzwdadoov.html

memset(a, 0, sizeof a);
来源：http://hz.bjfxy.top/gtrjajlirs.html

[S27] C：定义常量
来源：http://hz.cheryme.top/gtqgnmsvvv.html

const double PI = 3.14159;
来源：http://hz.zhoulong.xyz/gtmvnzjztr.html

[S28] C：静态变量
来源：http://hz.zhoulong.xyz/gtaypqjeyp.html

static int counter = 0;
来源：http://hz.zhixingplan.top/gturkqshct.html

[S29] C：变参函数
来源：http://hz.bjfxy.top/gtohwtugjv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.gogol.net.cn/gtpnpjuccq.html

[S30] C：头文件保护
来源：http://hz.jlsjyb.cn/gtoeqmnknd.html

#ifndef X_H
来源：http://hz.zhijiandao.cn/gtlvpxxiyn.html

#define X_H
来源：http://hz.zhiwuduotai.top/gtrhwzbdek.html

#endif
来源：http://hz.tanke756.top/gthpqvgnvz.html

[S31] C++：Hello World
来源：http://hz.ydzc1.top/gtpniqdixe.html

#include <iostream>
来源：http://hz.jqgufenzy.top/gtrdfastdk.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.cheryme.top/gttwsawxsy.html

[S32] C++：字符串
来源：http://hz.sufxvd.cn/gtclcjetzq.html

std::string s = "hi";  s += "!";
来源：http://hz.hammf.cn/gtktcwzfuf.html

[S33] C++：vector 增删
来源：http://hz.nanxuanxn.top/gtbbutzutq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.tanke756.top/gtppieveoz.html

[S34] C++：遍历 vector
来源：http://hz.nanxuanxn.top/gtwmskrtef.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hongshengwenyu.top/gtcxmvpfnd.html

[S35] C++：map
来源：http://hz.guannengcc.top/gtkwhkfhpo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.smart0.xyz/gtvmxieaaq.html

[S36] C++：unordered_map
来源：http://hz.yj20258.top/gtiuhsiqdl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yuanzhike.top/gtosxznwat.html

[S37] C++：set
来源：http://hz.cdnleiting.top/gtmqscqtjd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.kuanghao11.cn/gttnfcfrhu.html

[S38] C++：排序
来源：http://hz.feifeiyinyue.top/gtndyealat.html

std::sort(v.begin(), v.end());
来源：http://hz.redwolf501.top/gtyeimjjkw.html

[S39] C++：自定义比较器排序
来源：http://hz.meibo888.top/gtqxxzotre.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.smart0.xyz/gtdtoijala.html

[S40] C++：查找元素
来源：http://hz.yuxming.cn/gtrrpovkpt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.ydjk.org.cn/gtukfiuuan.html

[S41] C++：类与构造函数
来源：http://hz.cashguo.top/gtuiuiexmb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hongshengwenyu.top/gtbbvigppu.html

[S42] C++：继承与虚函数
来源：http://hz.andypj.xyz/gtbkhwnzuc.html

class B : public Base { public: void f() override {} };
来源：http://hz.birdmap.top/gthwhtzfeb.html

[S43] C++：智能指针
来源：http://hz.hnxiangtu.top/gtanedfmwa.html

auto p = std::make_unique<int>(5);
来源：http://hz.cqqwz.cn/gtnplcgoug.html

[S44] C++：引用传参
来源：http://hz.daria6918.cn/gttbsucsdt.html

void inc(int &x) { ++x; }
来源：http://hz.tian-w.cn/gtlfmvjvkc.html

[S45] C++：lambda
来源：http://hz.jinqigfzy.top/gtvcezktzh.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hywenlv.cn/gtvjlspdgr.html

[S46] C++：函数模板
来源：http://hz.ydzc1.top/gtmzehofnr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.iojbl.cn/gtsdbxrtvm.html

[S47] C++：结构化绑定遍历
来源：http://hz.meibo888.top/gtnytwfflj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.hfpthk.cn/gtiuuovxlk.html

[S48] C++：逐行读文件
来源：http://hz.kuanghao11.cn/gtokqyzgwz.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.iojbl.cn/gtkjsllvqb.html

while (std::getline(in, line)) { }
来源：http://hz.jinqigufen.top/gtqvobbcxz.html

[S49] C++：写文件
来源：http://hz.nanxuanxn.top/gtafyizdqm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.tian-w.cn/gtdatrmdsz.html

[S50] C++：格式化数字
来源：http://hz.ehwqpu.com/gtrmtfbdyb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhengqikj.top/gtrqrrsecy.html

[S51] C++：显式类型转换
来源：http://hz.daria6918.cn/gthgmnihyw.html

static_cast<double>(a) / b
来源：http://hz.0kj1m.cn/gtplknzbmc.html

[S52] C++：const 与 noexcept
来源：http://hz.shangyingyoupin.top/gtlzcuduak.html

int size() const noexcept { return n_; }
来源：http://hz.xylfe.cn/gtkfcmnsww.html

[S53] C++：移动语义
来源：http://hz.snrcjt.cn/gtflndycwv.html

std::vector<int> w = std::move(v);
来源：http://hz.yueranfly.top/gtnnoyyisi.html

[S54] C++：异常处理
来源：http://hz.shanyushiyangtech.top/gtyelbjoab.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.meibo888.top/gtsiovkqrn.html

[S55] C++：结构化绑定
来源：http://hz.xylfe.cn/gtyweohznv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.52xcode.cn/gtbiczqlao.html

[S56] C++：optional
来源：http://hz.kuanghao11.cn/gtorkgfhbh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.guowangkeji.top/gtjnnnqpxk.html

[S57] C++：编译期常量
来源：http://hz.hfpthk.cn/gtakvzjzse.html

constexpr int N = 10;
来源：http://hz.xuetiantiany.cn/gtnfvqmajn.html

[S58] C++：命名空间
来源：http://hz.ywan-chungtsiang.top/gtcahmuara.html

namespace ns { int f() { return 1; } }
来源：http://hz.shanyushiyangkeji.top/gtlbpdcsgf.html

[S59] C++：静态断言
来源：http://hz.hnxiangtu.top/gtuzyvlmtq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xziqi.cn/gtxmbfutnj.html

[S60] C++：遍历并删除元素
来源：http://hz.cashguo.top/gtlcezcuni.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.xuetiantiany.cn/gtwpixsoel.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtpzwytskb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jyoumei.cn/gtjdjxqkkm.html

================================================================================
来源：http://hz.iojbl.cn/gtmsooirko.html

[T01] Kotlin：Hello World
来源：http://hz.ybcxt.top/gtgtlguwbx.html

println("Hello")
来源：http://hz.dianchejie.cn/gtiwgknhnp.html

[T02] Kotlin：变量
来源：http://hz.redwolf501.top/gtymtjfrhx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.ydzc1.top/gtmihdxohn.html

[T03] Kotlin：字符串模板
来源：http://hz.sxryk.cn/gtmfggqoub.html

"值: $b"
来源：http://hz.tianlin.xyz/gtqdgxtjot.html

[T04] Kotlin：空安全
来源：http://hz.zycfv.cn/gtumlqmady.html

val n: String? = null;  n?.length
来源：http://hz.xziqi.cn/gtaihjbwsn.html

[T05] Kotlin：when 表达式
来源：http://hz.jqgufenzy.top/gttgqvuizw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.shzxlz.cn/gtollyqqxv.html

[T06] Kotlin：集合映射
来源：http://hz.shanyushiyangkeji.top/gthtqseznt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.aibaodan.cn/gtsyjazcfw.html

[T07] Kotlin：集合过滤
来源：http://hz.pycfn.com/gtiwatcaji.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.shzxlz.cn/gtkotmsqww.html

[T08] Kotlin：数据类
来源：http://hz.shuidangran.top/gtwcyhdxzq.html

data class User(val name: String, val age: Int)
来源：http://hz.jqgufenzy.top/gtnlsgtmsm.html

[T09] Kotlin：扩展函数
来源：http://hz.xylfe.cn/gtdhfcczbe.html

fun String.exclaim() = this + "!"
来源：http://hz.haohaochexian.top/gtynujuinb.html

[T10] Kotlin：默认参数
来源：http://hz.haohaochexian.top/gtknaajwpq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.sysykeji.top/gtnnyevmgk.html

[T11] Kotlin：协程
来源：http://hz.yvedp.cn/gtuvawxglf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.52xcode.cn/gtavhoudnq.html

[T12] Kotlin：解构声明
来源：http://hz.jinghuilouyu.cn/gtxnqwuelv.html

val (a, b) = Pair(1, 2)
来源：http://hz.pengpengdd.cyou/gtrqlsifqq.html

[T13] Kotlin：只读 Map
来源：http://hz.ybcxt.top/gtqdorezjx.html

val m = mapOf("a" to 1)
来源：http://hz.yonumen.top/gtjkstxzkz.html

[T14] Kotlin：循环
来源：http://hz.jinyuanbaomall.cn/gtaxcautvk.html

for (i in 1..10) println(i)
来源：http://hz.vqdsnc.cn/gtfuhottgz.html

[T15] Kotlin：接口
来源：http://hz.ywan-chungtsiang.top/gtedjbposo.html

interface Shape { fun area(): Double }
来源：http://hz.andypj.xyz/gteahccmcs.html

[T16] Swift：Hello World
来源：http://hz.yongpay.top/gteqwqgjzc.html

print("Hello")
来源：http://hz.redwolf501.top/gthcunmvrz.html

[T17] Swift：变量与常量
来源：http://hz.daxiang520.top/gtmwbdiwiw.html

var a = 1;  let b = 2
来源：http://hz.havefunace.top/gtnopokzam.html

[T18] Swift：字符串插值
来源：http://hz.xziqi.cn/gtrvsqroaz.html

"值: \(b)"
来源：http://hz.dashuyun.cn/gtomsrllnf.html

[T19] Swift：可选绑定
来源：http://hz.xuetiantiany.cn/gtrwlzqqnb.html

if let n = opt { print(n) }
来源：http://hz.svipenyu.cn/gtxettifvh.html

[T20] Swift：数组操作
来源：http://hz.ydjk.org.cn/gtobffnakc.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.xylfe.cn/gtrwkutded.html

[T21] Swift：遍历
来源：http://hz.xingfuxueyuan.xyz/gtsygzjgav.html

for x in a { print(x) }
来源：http://hz.shanyushiyangtech.top/gtkilsuctr.html

[T22] Swift：字典
来源：http://hz.hnqzz.top/gtxhoahfmy.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.tian-w.cn/gtghcmwxtf.html

[T23] Swift：函数
来源：http://hz.ivvv.top/gtcmheaubf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.andypj.xyz/gtlautzsie.html

[T24] Swift：闭包
来源：http://hz.zhoulong.xyz/gthwdrvvdj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jinyuanbaomall.cn/gtekmegsbl.html

[T25] Swift：结构体
来源：http://hz.zhijiandao.cn/gtwhabjcmq.html

struct P { var x: Int }
来源：http://hz.pengpengdd.cyou/gtkibuiodf.html

[T26] Swift：类与重写
来源：http://hz.cdnleiting.top/gtpkwvchkr.html

class A: Base { override func f() {} }
来源：http://hz.dianchejie.cn/gtiayrtmii.html

[T27] Swift：错误处理
来源：http://hz.pengpengdd.cyou/gtqcllgdof.html

do { try f() } catch { print(error) }
来源：http://hz.smart0.xyz/gttqesprri.html

[T28] Swift：枚举
来源：http://hz.vqdsnc.cn/gtdbsipkhq.html

enum Color { case red, green }
来源：http://hz.c1oappe.top/gtiotaicgu.html

[T29] Swift：guard 提前返回
来源：http://hz.cheryme.top/gtfevfxmqa.html

guard let x = opt else { return }
来源：http://hz.tanke756.top/gtofztlpsl.html

[T30] Swift：协议
来源：http://hz.bjfxy.top/gtzhwermic.html

protocol Shape { func area() -> Double }
来源：http://hz.pengpengdd.cyou/gtjeepbkwl.html

[T31] Lua：Hello World
来源：http://hz.yongpay.top/gtaskspjdz.html

print("Hello")
来源：http://hz.hongshengwenyu.top/gtzqgskvry.html

[T32] Lua：局部变量
来源：http://hz.kuanghao11.cn/gtadtflizc.html

local a = 1
来源：http://hz.xylfe.cn/gtfuelqzgq.html

[T33] Lua：表（数组）
来源：http://hz.yanxiufei.cn/gtquopnfhs.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.nwbrower.top/gtmoykkrpe.html

[T34] Lua：遍历表
来源：http://hz.ydzc1.top/gtppyibgcf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.0kj1m.cn/gtcrvtbxoi.html

[T35] Lua：字典表
来源：http://hz.hfpthk.cn/gtezsdbulp.html

local d = { a = 1 };  d.b = 2
来源：http://hz.ppjwa.cn/gttlbsykxk.html

[T36] Lua：函数
来源：http://hz.yanxiufei.cn/gtazhuypnt.html

function add(a, b) return a + b end
来源：http://hz.yuxming.cn/gtbywifhxz.html

[T37] Lua：字符串拼接
来源：http://hz.9152youxi.cn/gtyliavzor.html

"a" .. "b"
来源：http://hz.ybcxt.top/gtvxgmlnpw.html

[T38] Lua：条件
来源：http://hz.xinyue.icu/gtffojbzqi.html

if x > 0 then print("正") end
来源：http://hz.zhixingplan.top/gtckzfbxer.html

[T39] Lua：模式匹配
来源：http://hz.jiagoushi.top/gtrfglrecc.html

string.find(s, "%d+")
来源：http://hz.guannengcc.top/gtpzoaoyfp.html

[T40] Lua：元表
来源：http://hz.ydzc1.top/gtuqpkjkmw.html

setmetatable({}, { __index = base })
来源：http://hz.chenlongwang.top/gtiipepbpa.html

[T41] Perl：Hello World
来源：http://hz.quarkkingdee.top/gtmxbkznda.html

print "Hello\n";
来源：http://hz.hfpthk.cn/gtijbawjgj.html

[T42] Perl：变量类型
来源：http://hz.aizwys.cn/gtatzhewpo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.ydjk.org.cn/gtpbcjfdfr.html

[T43] Perl：字符串插值
来源：http://hz.0kj1m.cn/gtxvkiankl.html

"值: $a"
来源：http://hz.zhiwuduotai.top/gttvqmqgru.html

[T44] Perl：条件
来源：http://hz.daria6918.cn/gttawadugm.html

if ($a > 0) { print "正"; }
来源：http://hz.cucudq.cn/gtvyyvcuon.html

[T45] Perl：数组遍历
来源：http://hz.cqqwz.cn/gtshntklul.html

for my $x (@arr) { print $x; }
来源：http://hz.andypj.xyz/gtrlmmncck.html

[T46] Perl：哈希操作
来源：http://hz.iojbl.cn/gtlznoaeon.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.ehwqpu.com/gtfwmqsqux.html

[T47] Perl：正则捕获
来源：http://hz.feifeiyinyue.top/gtulyezhth.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.wangshuangyany.cn/gtftvyvptd.html

[T48] Perl：正则替换
来源：http://hz.ivvv.top/gtjelitqcj.html

$s =~ s/old/new/g;
来源：http://hz.ehwqpu.com/gtxuotxgme.html

[T49] Perl：函数
来源：http://hz.nwbrower.top/gtmenscdhz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.nanxuanxn.top/gtvqsgnsaj.html

[T50] Perl：逐行读文件
来源：http://hz.sxryk.cn/gtmtjzjlio.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.52xcode.cn/gtjjrpanpi.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.c1oappe.top/gtewaouvcl.html

[T51] Scala：Hello World
来源：http://hz.zhijiandao.cn/gtwsunejxj.html

println("Hello")
来源：http://hz.ivvv.top/gtozmazobt.html

[T52] Scala：变量
来源：http://hz.dianchejie.cn/gtabqqymou.html

val a = 1;  var b = 2
来源：http://hz.dashuyun.cn/gtgurjlmrn.html

[T53] Scala：字符串插值
来源：http://hz.daria6918.cn/gtnqifbyvm.html

s"值: $b"
来源：http://hz.hywenlv.cn/gtnaqoufop.html

[T54] Scala：集合映射
来源：http://hz.yanxiufei.cn/gtgigoasae.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.gaohongyu789.top/gtsykgruwi.html

[T55] Scala：集合过滤
来源：http://hz.feifeiyinyue.top/gtckmnegzn.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jianghu66.top/gtymwhzqri.html

[T56] Scala：样例类
来源：http://hz.jqgfzy.top/gtmuwpyuyi.html

case class User(name: String, age: Int)
来源：http://hz.dashuyun.cn/gtwoblbwkq.html

[T57] Scala：模式匹配
来源：http://hz.nwbrower.top/gtqdcgybmc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.cdnleiting.top/gtijsfwohe.html

[T58] Scala：函数定义
来源：http://hz.shuidangran.top/gtvfqtadwo.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.chenjidiqi.icu/gtvjqcqldn.html

[T59] Scala：循环
来源：http://hz.nanxuanxn.top/gtcvofiqmc.html

for (i <- 1 to 10) println(i)
来源：http://hz.yuanzhike.top/gtxlcgvudc.html

[T60] Scala：折叠
来源：http://hz.tian-w.cn/gtuwxysxfy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hammf.cn/gtosebdydm.html

================================================================================
来源：http://hz.cqqwz.cn/gtturvrcnv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.feifeiyinyue.top/gtmodaimeu.html

================================================================================
来源：http://hz.hnxiangtu.top/gtjhbduupm.html

[U01] Py：创建虚拟环境
来源：http://hz.jinghuilouyu.cn/gtdnuhgtbp.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.svipenyu.cn/gtqqujtwim.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jinghuilouyu.cn/gtyunibpeb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yuanzhike.top/gtcelophbv.html

[U03] Py：加载 .env 配置
来源：http://hz.zhengqikj.top/gtwuaxrxax.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.svipenyu.cn/gtvkfyevxc.html

[U04] Py：变量调试打印
来源：http://hz.smart0.xyz/gtuowwrbfh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.guannengcc.top/gtscufunzj.html

[U05] Py：列表去重且保序
来源：http://hz.xylfe.cn/gtilcoyqxr.html

list(dict.fromkeys(arr))
来源：http://hz.ydjk.org.cn/gtyxatbohc.html

[U06] Py：合并两个字典
来源：http://hz.gotoacloud.top/gtvgegjmis.html

{**a, **b}
来源：http://hz.shuidangran.top/gtzmcppbqu.html

[U07] Py：反转字典键值
来源：http://hz.zdqjudy.top/gtjhuckkdt.html

{v: k for k, v in d.items()}
来源：http://hz.haohaochexian.top/gtzhrzuwdi.html

[U08] Py：展平二维列表
来源：http://hz.xuetiantiany.cn/gtqlytzfxd.html

[y for x in nested for y in x]
来源：http://hz.dashuyun.cn/gtgurffnba.html

[U09] Py：字典取最大值的键
来源：http://hz.zhengqikj.top/gtvrzeurka.html

max(d, key=d.get)
来源：http://hz.zycfv.cn/gtfntkhsbi.html

[U10] Py：按值排序字典
来源：http://hz.cucudq.cn/gtdkbtjvrl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.nwbrower.top/gtsjopdktx.html

[U11] Py：生成器表达式
来源：http://hz.xziqi.cn/gtpggahhfr.html

(x * 2 for x in arr)
来源：http://hz.yueranfly.top/gtqdudnvrm.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.jinqigfzy.top/gtjnsebulw.html

Counter(arr).most_common(3)
来源：http://hz.nanxuanxn.top/gtyplkiczk.html

[U13] Py：固定长度队列
来源：http://hz.c1oappe.top/gtoitfnxwr.html

deque(maxlen=10)
来源：http://hz.guannengcc.top/gtlqhovfho.html

[U14] Py：分组收集到列表
来源：http://hz.yueranfly.top/gtbowliwfr.html

defaultdict(list)
来源：http://hz.yangfankeji.com/gthsxacvcb.html

[U15] Py：高精度计时
来源：http://hz.nwbrower.top/gtovlygloa.html

t = time.perf_counter()
来源：http://hz.yuxming.cn/gtsxxowovx.html

[U16] Py：命令行参数解析
来源：http://hz.mhx1999.top/gtsjoihemj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.snrcjt.cn/gthxjcmmei.html

[U17] Py：初始化日志
来源：http://hz.jyoumei.cn/gtksspnsku.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.hysaishi.cn/gtemmmeeyf.html

[U18] Py：预编译正则
来源：http://hz.chenlongwang.top/gtgzvsdhpy.html

pat = re.compile(r"\d+")
来源：http://hz.smart0.xyz/gtaesqpnqp.html

[U19] Py：正则替换带回调
来源：http://hz.haohaochexian.top/gttksippqj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.nanxinkj.top/gtkdqwrmgv.html

[U20] Py：缓存函数结果
来源：http://hz.dianchejie.cn/gtifuintiz.html

@functools.lru_cache(maxsize=None)
来源：http://hz.0kj1m.cn/gtphtlqmro.html

[U21] Py：自定义上下文管理器
来源：http://hz.zhengqikj.top/gtqmizlsrg.html

@contextlib.contextmanager
来源：http://hz.quarkkingdee.top/gtuyvbdiyx.html

[U22] Py：矩阵转置
来源：http://hz.aibaodan.cn/gtlatkqzqo.html

list(zip(*m))
来源：http://hz.daria6918.cn/gtstwpxman.html

[U23] Py：分块读取大文件
来源：http://hz.tian-w.cn/gtxnujhqwl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yvedp.cn/gtvrzxbgmi.html

[U24] Py：路径操作
来源：http://hz.gotoacloud.top/gtseuomuwf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.guannengcc.top/gtoizlfted.html

[U25] Py：CSV 按字典读
来源：http://hz.zhaomingkeji.xyz/gtzkzggxqb.html

csv.DictReader(f)
来源：http://hz.ydzc1.top/gtcofzolvu.html

[U26] Py：并发下载
来源：http://hz.aibaodan.cn/gtwtjoumsb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.shanyushiyangtech.top/gtjjyuwgdz.html

[U27] Py：异步 HTTP
来源：http://hz.shangyingyoupin.top/gtfiqcfbxc.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.jinqigufen.top/gtserztzmm.html

[U28] Py：类型别名
来源：http://hz.tanke756.top/gtdltpuiib.html

UserId = int
来源：http://hz.jlsjyb.cn/gtmijyptro.html

[U29] Py：属性校验
来源：http://hz.hnxiangtu.top/gtbtcqgljk.html

@property 与 @x.setter 配合
来源：http://hz.cdnleiting.top/gtgcdfflbu.html

[U30] Py：数据类
来源：http://hz.zhaomingkeji.xyz/gtcyhdqlcc.html

@dataclass(slots=True)
来源：http://hz.smart0.xyz/gtlcbshfot.html

[U31] Py：单测
来源：http://hz.guowangkeji.top/gtjpxycopv.html

python -m pytest -q
来源：http://hz.ppjwa.cn/gtfeppfnbi.html

[U32] Py：代码格式化
来源：http://hz.pycfn.com/gtidxcnaxi.html

ruff format . && ruff check --fix .
来源：http://hz.gzhubu.top/gtbdazniax.html


<!-- 参考信息 -->