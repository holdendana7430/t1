代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zdqjudy.top/gtoqxhgoxi.html

[S10] C：指针与解引用
来源：http://hz.0kj1m.cn/gtvrcmxoru.html

int *p = &a;  *p = 5;
来源：http://hz.zhoulong.xyz/gtlpmfwhgx.html

[S11] C：逐行读文件
来源：http://hz.wangshuangyany.cn/gtiuesnbts.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.birdmap.top/gtpnoohgkz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.mhx1999.top/gtqgzvkuco.html

fclose(f);
来源：http://hz.yueranfly.top/gtefixhsmq.html

[S12] C：写文件
来源：http://hz.pycfn.com/gtxpacjveh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hnxiangtu.top/gttuzrdugq.html

[S13] C：宏定义
来源：http://hz.zhongyouzk.top/gtyxzkjjha.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jinghuilouyu.cn/gtwmtgqozv.html

[S14] C：枚举
来源：http://hz.zhengqikj.top/gtshgdrmho.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.nanxuanxn.top/gtmsvageuy.html

[S15] C：类型转换
来源：http://hz.tian-w.cn/gtusjwvypt.html

(double) a / b
来源：http://hz.nwbrower.top/gtegbhinjk.html

[S16] C：位操作置位
来源：http://hz.havefunace.top/gtebcoirqf.html

x |= (1 << 3);
来源：http://hz.yangfankeji.com/gtuhwktjhs.html

[S17] C：安全拼接字符串
来源：http://hz.kuanghao11.cn/gtzgnbimsi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.birdmap.top/gtwfqkniln.html

[S18] C：命令行参数
来源：http://hz.daria6918.cn/gthsojilqn.html

int main(int argc, char **argv)
来源：http://hz.ywan-chungtsiang.top/gtjwhwssei.html

[S19] C：快速排序
来源：http://hz.ehwqpu.com/gtczcexqqh.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.chenzaomai.com/gtsiciejci.html

[S20] C：二分查找
来源：http://hz.nwbrower.top/gtvgxfrnbi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ydjk.org.cn/gtavwoqsyh.html

[S21] C：字符类别判断
来源：http://hz.shzxlz.cn/gtjwgcuqvq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.tian-w.cn/gtpzlurgrh.html

[S22] C：字符串转数字
来源：http://hz.daria6918.cn/gtearupyho.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhongyouzk.top/gtlzummbcl.html

[S23] C：随机数
来源：http://hz.316326.xyz/gtdxtrkszt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.meibo888.top/gtyuxdvgfk.html

[S24] C：获取本地时间
来源：http://hz.jinyuanbaomall.cn/gtmflwsuhl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ppjwa.cn/gtvlwywdxi.html

[S25] C：内存拷贝
来源：http://hz.0kj1m.cn/gtfloghvjv.html

memcpy(dst, src, n);
来源：http://hz.0kj1m.cn/gtiwkfsiks.html

[S26] C：内存清零
来源：http://hz.cashguo.top/gtzzeeciif.html

memset(a, 0, sizeof a);
来源：http://hz.guannengcc.top/gtkaxrivmu.html

[S27] C：定义常量
来源：http://hz.cheryme.top/gtoaepffra.html

const double PI = 3.14159;
来源：http://hz.zhixingplan.top/gthergnirh.html

[S28] C：静态变量
来源：http://hz.chenzaomai.com/gtrqveplts.html

static int counter = 0;
来源：http://hz.daria6918.cn/gtahnbiuud.html

[S29] C：变参函数
来源：http://hz.yvedp.cn/gtggrvnvti.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhaomingkeji.xyz/gtxmvqaucf.html

[S30] C：头文件保护
来源：http://hz.hammf.cn/gtwdwatnkt.html

#ifndef X_H
来源：http://hz.jianghu66.top/gttcqdvzmw.html

#define X_H
来源：http://hz.kuanghao11.cn/gtoqhzaqen.html

#endif
来源：http://hz.hywenlv.cn/gtubymvwps.html

[S31] C++：Hello World
来源：http://hz.cheryme.top/gttxfdkfgb.html

#include <iostream>
来源：http://hz.jyoumei.cn/gtvzrwczdv.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.dianchejie.cn/gtwkisxaoa.html

[S32] C++：字符串
来源：http://hz.meibo888.top/gtspewqbjz.html

std::string s = "hi";  s += "!";
来源：http://hz.xuanzx.com/gtqcsjckha.html

[S33] C++：vector 增删
来源：http://hz.gzhubu.top/gtytkrqblw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yongpay.top/gtsvhjahsx.html

[S34] C++：遍历 vector
来源：http://hz.jinqigufen.top/gtfhmlwest.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xingfuxueyuan.xyz/gteceopfqo.html

[S35] C++：map
来源：http://hz.zhiwuduotai.top/gtonexbwee.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.svipenyu.cn/gttmgrbres.html

[S36] C++：unordered_map
来源：http://hz.wangshuangyany.cn/gtbcwvaumz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sxryk.cn/gtspjqhebc.html

[S37] C++：set
来源：http://hz.snrcjt.cn/gtacjpuqfg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jinqigufen.top/gtgjqhfamq.html

[S38] C++：排序
来源：http://hz.quarkkingdee.top/gtafbvmmjc.html

std::sort(v.begin(), v.end());
来源：http://hz.sweek.top/gtsjgxxewj.html

[S39] C++：自定义比较器排序
来源：http://hz.wangshuangyany.cn/gttrkpzppg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.dashuyun.cn/gtgnihourw.html

[S40] C++：查找元素
来源：http://hz.bjfxy.top/gtxuewrbsl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.cqqwz.cn/gtijvliqlk.html

[S41] C++：类与构造函数
来源：http://hz.cqqwz.cn/gtfptyirfe.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhijiandao.cn/gthynlfloz.html

[S42] C++：继承与虚函数
来源：http://hz.quarkkingdee.top/gtdyqfxyoq.html

class B : public Base { public: void f() override {} };
来源：http://hz.cdnleiting.top/gtmrqeffji.html

[S43] C++：智能指针
来源：http://hz.guannengcc.top/gtutyzabfr.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhengqikj.top/gtbrwnkcnk.html

[S44] C++：引用传参
来源：http://hz.zhixingplan.top/gtjljlquzs.html

void inc(int &x) { ++x; }
来源：http://hz.svipenyu.cn/gttshydajj.html

[S45] C++：lambda
来源：http://hz.gaohongyu789.top/gtixugidvn.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cucudq.cn/gtnnrzsetb.html

[S46] C++：函数模板
来源：http://hz.zhiwuduotai.top/gtivevmwnz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.aibaodan.cn/gtqknrxzfo.html

[S47] C++：结构化绑定遍历
来源：http://hz.hnqzz.top/gtlkabcafo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.hnqzz.top/gtaltplemi.html

[S48] C++：逐行读文件
来源：http://hz.dashuyun.cn/gtqgrsspie.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.feifeiyinyue.top/gtptxltudf.html

while (std::getline(in, line)) { }
来源：http://hz.gotoacloud.top/gterrhwqbc.html

[S49] C++：写文件
来源：http://hz.shangyingyoupin.top/gttqmxseuu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yj20258888.top/gtznivhsyt.html

[S50] C++：格式化数字
来源：http://hz.zhengqikj.top/gttgagqgmd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hammf.cn/gtlgmrwrvr.html

[S51] C++：显式类型转换
来源：http://hz.aizwys.cn/gtbnjnimze.html

static_cast<double>(a) / b
来源：http://hz.gotoacloud.top/gthcgiacjr.html

[S52] C++：const 与 noexcept
来源：http://hz.sysykeji.top/gtfybnktkf.html

int size() const noexcept { return n_; }
来源：http://hz.wangshuangyany.cn/gtpyqvdcvb.html

[S53] C++：移动语义
来源：http://hz.jinghuilouyu.cn/gtgwvbaqxa.html

std::vector<int> w = std::move(v);
来源：http://hz.jyoumei.cn/gtryqoidjt.html

[S54] C++：异常处理
来源：http://hz.xziqi.cn/gtrapytlxr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.sxryk.cn/gtjhdbpvts.html

[S55] C++：结构化绑定
来源：http://hz.fengsongda.top/gtlbubvfuy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.shanyushiyangkeji.top/gtqfqijsji.html

[S56] C++：optional
来源：http://hz.zhiwuduotai.top/gtjetuppbx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhongyouzk.top/gtkxwhnydt.html

[S57] C++：编译期常量
来源：http://hz.zhoulong.xyz/gtifhruypg.html

constexpr int N = 10;
来源：http://hz.ivvv.top/gtpvrllevm.html

[S58] C++：命名空间
来源：http://hz.52xcode.cn/gtclpfqmyy.html

namespace ns { int f() { return 1; } }
来源：http://hz.dianchejie.cn/gtwwmcrtew.html

[S59] C++：静态断言
来源：http://hz.dianchejie.cn/gtedboeoaz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.tian-w.cn/gtqcrzjcvk.html

[S60] C++：遍历并删除元素
来源：http://hz.hnqzz.top/gtujdmsymb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.pycfn.com/gtfxjwfloi.html

================================================================================
来源：http://hz.zhixingplan.top/gtjftyzayj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jianghu66.top/gtvbpfsoir.html

================================================================================
来源：http://hz.jqgfzy.top/gtzoepbxhs.html

[T01] Kotlin：Hello World
来源：http://hz.ppjwa.cn/gtdvzfyuci.html

println("Hello")
来源：http://hz.jqgfzy.top/gtswrbjejw.html

[T02] Kotlin：变量
来源：http://hz.yj202588.top/gtladyltpm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.mhx1999.top/gtlerpnxhr.html

[T03] Kotlin：字符串模板
来源：http://hz.zhongyouzk.top/gtxxoynpxw.html

"值: $b"
来源：http://hz.vqdsnc.cn/gtchjqlcby.html

[T04] Kotlin：空安全
来源：http://hz.ivvv.top/gtgfkyymzk.html

val n: String? = null;  n?.length
来源：http://hz.hnqzz.top/gtxububimu.html

[T05] Kotlin：when 表达式
来源：http://hz.xuanzx.com/gtuxqblmpx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.mhx1999.top/gtugvnntwi.html

[T06] Kotlin：集合映射
来源：http://hz.sysykeji.top/gttthebuij.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.gogol.net.cn/gtpxtmpkqe.html

[T07] Kotlin：集合过滤
来源：http://hz.ydzc1.top/gtuaokwaun.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.chenzaomai.com/gtsubnwfly.html

[T08] Kotlin：数据类
来源：http://hz.ydzc1.top/gtfimjutbf.html

data class User(val name: String, val age: Int)
来源：http://hz.jinqigfzy.top/gtdtyvlpmq.html

[T09] Kotlin：扩展函数
来源：http://hz.jinyuanbaomall.cn/gthurtyeei.html

fun String.exclaim() = this + "!"
来源：http://hz.tian-w.cn/gtbphelqyu.html

[T10] Kotlin：默认参数
来源：http://hz.zhongyouzk.top/gtlabqxcdc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.feifeiyinyue.top/gthjbockgi.html

[T11] Kotlin：协程
来源：http://hz.ehwqpu.com/gtgjevhnbe.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.quarkkingdee.top/gtffzxpeol.html

[T12] Kotlin：解构声明
来源：http://hz.52xcode.cn/gtmgjjvayd.html

val (a, b) = Pair(1, 2)
来源：http://hz.xylfe.cn/gtoqvjoprl.html

[T13] Kotlin：只读 Map
来源：http://hz.shuidangran.top/gtryfcqdoc.html

val m = mapOf("a" to 1)
来源：http://hz.tanke756.top/gtwffjnuim.html

[T14] Kotlin：循环
来源：http://hz.daxiang520.top/gtwxhllkjy.html

for (i in 1..10) println(i)
来源：http://hz.ywan-chungtsiang.top/gtnzjujwwn.html

[T15] Kotlin：接口
来源：http://hz.cdnleiting.top/gtarytjpwe.html

interface Shape { fun area(): Double }
来源：http://hz.hammf.cn/gtzgkndyfo.html

[T16] Swift：Hello World
来源：http://hz.feifeiyinyue.top/gtvnxcrfgu.html

print("Hello")
来源：http://hz.hammf.cn/gtsjytwnfa.html

[T17] Swift：变量与常量
来源：http://hz.cheryme.top/gtlgpyxsex.html

var a = 1;  let b = 2
来源：http://hz.chenlongwang.top/gtfhrijznl.html

[T18] Swift：字符串插值
来源：http://hz.ybcxt.top/gtnrrxbqdi.html

"值: \(b)"
来源：http://hz.zhiwuduotai.top/gtchhzvvui.html

[T19] Swift：可选绑定
来源：http://hz.yonumen.top/gtzrxacxfo.html

if let n = opt { print(n) }
来源：http://hz.shuidangran.top/gtbrjgqpni.html

[T20] Swift：数组操作
来源：http://hz.iojbl.cn/gtcbudmnhw.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.mhx1999.top/gtzwrukwpz.html

[T21] Swift：遍历
来源：http://hz.gotoacloud.top/gteuryvtka.html

for x in a { print(x) }
来源：http://hz.jinqigufen.top/gtaosdpwbd.html

[T22] Swift：字典
来源：http://hz.yj20258888.top/gttijuvqeu.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.xuetiantiany.cn/gtptgpumgt.html

[T23] Swift：函数
来源：http://hz.gzhubu.top/gtztuaahey.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.hnxiangtu.top/gtnxabkhxu.html

[T24] Swift：闭包
来源：http://hz.xziqi.cn/gtpamehvlk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.9152youxi.cn/gtzmhdebca.html

[T25] Swift：结构体
来源：http://hz.cqqwz.cn/gtpqmtzlww.html

struct P { var x: Int }
来源：http://hz.jinghuilouyu.cn/gtanhgxsqp.html

[T26] Swift：类与重写
来源：http://hz.chenzaomai.com/gtswmwykch.html

class A: Base { override func f() {} }
来源：http://hz.zhixingplan.top/gtlqbrwhjt.html

[T27] Swift：错误处理
来源：http://hz.havefunace.top/gtdpdgvpav.html

do { try f() } catch { print(error) }
来源：http://hz.yangfankeji.com/gtnqlzopao.html

[T28] Swift：枚举
来源：http://hz.wangdashe.top/gtzvugyrsi.html

enum Color { case red, green }
来源：http://hz.hywenlv.cn/gtukurbphd.html

[T29] Swift：guard 提前返回
来源：http://hz.gogol.net.cn/gtpkghozqv.html

guard let x = opt else { return }
来源：http://hz.redwolf501.top/gtedjjexgq.html

[T30] Swift：协议
来源：http://hz.hammf.cn/gthuxvkfkx.html

protocol Shape { func area() -> Double }
来源：http://hz.yongpay.top/gtegfqyzbd.html

[T31] Lua：Hello World
来源：http://hz.svipenyu.cn/gtbgtvyxsj.html

print("Hello")
来源：http://hz.smart0.xyz/gtjvseniwj.html

[T32] Lua：局部变量
来源：http://hz.jianghu66.top/gtizssfcny.html

local a = 1
来源：http://hz.xuetiantiany.cn/gtcgnmhfuy.html

[T33] Lua：表（数组）
来源：http://hz.haohaochexian.top/gtlcxfpvus.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.cucudq.cn/gtdlcgnzow.html

[T34] Lua：遍历表
来源：http://hz.yueranfly.top/gthrdefmgf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.sysykeji.top/gteqycmozu.html

[T35] Lua：字典表
来源：http://hz.sxryk.cn/gttjaeareh.html

local d = { a = 1 };  d.b = 2
来源：http://hz.cucudq.cn/gtfzackfli.html

[T36] Lua：函数
来源：http://hz.hywenlv.cn/gtrarhdvxk.html

function add(a, b) return a + b end
来源：http://hz.cheryme.top/gtyhackwor.html

[T37] Lua：字符串拼接
来源：http://hz.hysaishi.cn/gteyxiyzmf.html

"a" .. "b"
来源：http://hz.ywan-chungtsiang.top/gttnfwbwmj.html

[T38] Lua：条件
来源：http://hz.yueranfly.top/gtushweowa.html

if x > 0 then print("正") end
来源：http://hz.yvedp.cn/gtzigjbobq.html

[T39] Lua：模式匹配
来源：http://hz.meibo888.top/gtkhxbzlnk.html

string.find(s, "%d+")
来源：http://hz.yanxiufei.cn/gtxjgiccvs.html

[T40] Lua：元表
来源：http://hz.hywenlv.cn/gtulpumvby.html

setmetatable({}, { __index = base })
来源：http://hz.jinghuilouyu.cn/gtpkqpucaq.html

[T41] Perl：Hello World
来源：http://hz.dianchejie.cn/gtlvrvvftb.html

print "Hello\n";
来源：http://hz.shzxlz.cn/gturksbupb.html

[T42] Perl：变量类型
来源：http://hz.xuetiantiany.cn/gtscvdczoh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.sufxvd.cn/gtgrcopdky.html

[T43] Perl：字符串插值
来源：http://hz.vqdsnc.cn/gtsyfemekd.html

"值: $a"
来源：http://hz.aizwys.cn/gtkxnamqxb.html

[T44] Perl：条件
来源：http://hz.52xcode.cn/gtuxzzurkw.html

if ($a > 0) { print "正"; }
来源：http://hz.kuanghao11.cn/gtvzqrledz.html

[T45] Perl：数组遍历
来源：http://hz.zhengqikj.top/gtxxgolxoi.html

for my $x (@arr) { print $x; }
来源：http://hz.feifeiyinyue.top/gtoavagxhp.html

[T46] Perl：哈希操作
来源：http://hz.zycfv.cn/gtmbrpdqmn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.fzhhl.top/gtplntxzrr.html

[T47] Perl：正则捕获
来源：http://hz.svipenyu.cn/gttmzxhlml.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.shuidangran.top/gtkpvbphgk.html

[T48] Perl：正则替换
来源：http://hz.chenzaomai.com/gtafbxypxa.html

$s =~ s/old/new/g;
来源：http://hz.ybcxt.top/gtcystuglf.html

[T49] Perl：函数
来源：http://hz.0kj1m.cn/gtjzhypasf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.xziqi.cn/gtoeunlaez.html

[T50] Perl：逐行读文件
来源：http://hz.jinqigfzy.top/gtbrsqllxb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.daria6918.cn/gtddeorgih.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.aibaodan.cn/gtwlfpfmrg.html

[T51] Scala：Hello World
来源：http://hz.smart0.xyz/gticvmhzlh.html

println("Hello")
来源：http://hz.sweek.top/gtrphqpfdw.html

[T52] Scala：变量
来源：http://hz.birdmap.top/gtjjldaxjt.html

val a = 1;  var b = 2
来源：http://hz.andypj.xyz/gtzfoxfekg.html

[T53] Scala：字符串插值
来源：http://hz.bjfxy.top/gtwdwxkibw.html

s"值: $b"
来源：http://hz.xuetiantiany.cn/gtdegszjpj.html

[T54] Scala：集合映射
来源：http://hz.xuanzx.com/gtbrghwlfu.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.jyoumei.cn/gtulfitodt.html

[T55] Scala：集合过滤
来源：http://hz.vqdsnc.cn/gtjfchrsjr.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jinqigufen.top/gthuvxgpdq.html

[T56] Scala：样例类
来源：http://hz.xuanzx.com/gtdlsuckte.html

case class User(name: String, age: Int)
来源：http://hz.zhoulong.xyz/gtnahhddrc.html

[T57] Scala：模式匹配
来源：http://hz.wangdashe.top/gtiifgotxg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.cashguo.top/gtsoivozsy.html

[T58] Scala：函数定义
来源：http://hz.havefunace.top/gtzaesgksl.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.cdnleiting.top/gtmxdxfpsp.html

[T59] Scala：循环
来源：http://hz.gzhubu.top/gtiapdbxrk.html

for (i <- 1 to 10) println(i)
来源：http://hz.yj20258888.top/gtkfeiohce.html

[T60] Scala：折叠
来源：http://hz.zhengqikj.top/gtihawdjgh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.vqdsnc.cn/gtouguxmuq.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtpyyaurfz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.tian-w.cn/gtezjzvurm.html

================================================================================
来源：http://hz.jinqigufen.top/gtjvnrjujx.html

[U01] Py：创建虚拟环境
来源：http://hz.yuxming.cn/gtxndfobjp.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.xuanzx.com/gtonywntfb.html

[U02] Py：导出 / 安装依赖
来源：http://hz.gaohongyu789.top/gtszhzppzq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jqgfzy.top/gtmrelfhyn.html

[U03] Py：加载 .env 配置
来源：http://hz.zhiwuduotai.top/gtvymigifu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.52xcode.cn/gtcvdnnuwn.html

[U04] Py：变量调试打印
来源：http://hz.fengsongda.top/gtvjzwnjve.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.gotoacloud.top/gtpgjbwowo.html

[U05] Py：列表去重且保序
来源：http://hz.zhaomingkeji.xyz/gthilxvdcu.html

list(dict.fromkeys(arr))
来源：http://hz.zycfv.cn/gtzrpmsbaj.html

[U06] Py：合并两个字典
来源：http://hz.vqdsnc.cn/gtljvknnug.html

{**a, **b}
来源：http://hz.xylfe.cn/gtunuisbba.html

[U07] Py：反转字典键值
来源：http://hz.mhx1999.top/gtkahidiwz.html

{v: k for k, v in d.items()}
来源：http://hz.shangyingyoupin.top/gtqykislnv.html

[U08] Py：展平二维列表
来源：http://hz.chenjidiqi.icu/gtfhvddjrc.html

[y for x in nested for y in x]
来源：http://hz.cashguo.top/gtpqeivekz.html

[U09] Py：字典取最大值的键
来源：http://hz.haohaochexian.top/gtwhzzsjai.html

max(d, key=d.get)
来源：http://hz.shanyushiyangkeji.top/gttyigmnhi.html

[U10] Py：按值排序字典
来源：http://hz.jinyuanbaomall.cn/gtleorgbnk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.jinqigufen.top/gtfucfgimi.html

[U11] Py：生成器表达式
来源：http://hz.ywan-chungtsiang.top/gtxluxygkk.html

(x * 2 for x in arr)
来源：http://hz.zycfv.cn/gthtdkfyck.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.ydjk.org.cn/gtpqkncyaf.html

Counter(arr).most_common(3)
来源：http://hz.jinqigufen.top/gtbxxiabzc.html

[U13] Py：固定长度队列
来源：http://hz.dianchejie.cn/gtkjiyyyvv.html

deque(maxlen=10)
来源：http://hz.xingfuxueyuan.xyz/gtvpldppiy.html

[U14] Py：分组收集到列表
来源：http://hz.chenlongwang.top/gtqitcihun.html

defaultdict(list)
来源：http://hz.pengpengdd.cyou/gtlxkhdzpb.html

[U15] Py：高精度计时
来源：http://hz.shanyushiyangtech.top/gtabbjrxfd.html

t = time.perf_counter()
来源：http://hz.wangshuangyany.cn/gtvubeotes.html

[U16] Py：命令行参数解析
来源：http://hz.jqgufenzy.top/gtpezzytfj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.ywan-chungtsiang.top/gtvzgzmhyw.html

[U17] Py：初始化日志
来源：http://hz.xuanzx.com/gtmbedxszn.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.sysykeji.top/gtovfpbodo.html

[U18] Py：预编译正则
来源：http://hz.tianlin.xyz/gtyjygftbz.html

pat = re.compile(r"\d+")
来源：http://hz.jlsjyb.cn/gtsflxpmva.html

[U19] Py：正则替换带回调
来源：http://hz.tianlin.xyz/gtnukpqsxh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.jinghuilouyu.cn/gtyxroebty.html

[U20] Py：缓存函数结果
来源：http://hz.gzhubu.top/gtoksuajvf.html

@functools.lru_cache(maxsize=None)
来源：http://hz.ywan-chungtsiang.top/gtwzefceod.html

[U21] Py：自定义上下文管理器
来源：http://hz.shzxlz.cn/gtwemsjrfs.html

@contextlib.contextmanager
来源：http://hz.shzxlz.cn/gtlzogalkl.html

[U22] Py：矩阵转置
来源：http://hz.ydzc1.top/gtzkmgcmsh.html

list(zip(*m))
来源：http://hz.yueranfly.top/gtszwqfxvx.html

[U23] Py：分块读取大文件
来源：http://hz.shuidangran.top/gtbqytqzkq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.kuanghao11.cn/gtebgpjedy.html

[U24] Py：路径操作
来源：http://hz.nwbrower.top/gtiqcehmhm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.zhongyouzk.top/gtppjeunbc.html

[U25] Py：CSV 按字典读
来源：http://hz.shuidangran.top/gtxuczssmj.html

csv.DictReader(f)
来源：http://hz.cheryme.top/gtktrhpuga.html

[U26] Py：并发下载
来源：http://hz.hnxiangtu.top/gtoqlaxtmo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jyoumei.cn/gthknmdjfz.html

[U27] Py：异步 HTTP
来源：http://hz.cheryme.top/gtrnxxeisv.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.hywenlv.cn/gtdasqsijp.html

[U28] Py：类型别名
来源：http://hz.hnqzz.top/gtrjegqqse.html

UserId = int
来源：http://hz.ywan-chungtsiang.top/gtysyissqr.html

[U29] Py：属性校验
来源：http://hz.gaohongyu789.top/gtfwppniel.html

@property 与 @x.setter 配合
来源：http://hz.0kj1m.cn/gtoskwcian.html

[U30] Py：数据类
来源：http://hz.c1oappe.top/gteglxedzh.html

@dataclass(slots=True)
来源：http://hz.aizwys.cn/gtsoaapxob.html

[U31] Py：单测
来源：http://hz.shzxlz.cn/gtmptruuej.html

python -m pytest -q
来源：http://hz.mhx1999.top/gttfncgxdw.html

[U32] Py：代码格式化
来源：http://hz.ppjwa.cn/gtcoziazqd.html

ruff format . && ruff check --fix .
来源：http://hz.jinqigufen.top/gtsjpoyahq.html


<!-- 参考信息 -->