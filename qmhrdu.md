代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.haohaochexian.top/gtidufguxf.html

[S08] C：动态内存分配与释放
来源：http://hz.0kj1m.cn/gtcvlaasjg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hnqzz.top/gttwargnpi.html

[S09] C：结构体定义与初始化
来源：http://hz.chenlongwang.top/gthvwqilwf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhaomingkeji.xyz/gtsqevqbpq.html

[S10] C：指针与解引用
来源：http://hz.wangshuangyany.cn/gtlxhvncrl.html

int *p = &a;  *p = 5;
来源：http://hz.jqgufenzy.top/gtleagvydn.html

[S11] C：逐行读文件
来源：http://hz.iojbl.cn/gtvtjmnpnu.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.haohaochexian.top/gtrhjdxamb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.cdnleiting.top/gttdexslwp.html

fclose(f);
来源：http://hz.zhongyouzk.top/gtyjhmarxy.html

[S12] C：写文件
来源：http://hz.daria6918.cn/gtgepdrgwn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.sxryk.cn/gtsuwtwxmm.html

[S13] C：宏定义
来源：http://hz.bjfxy.top/gtltvbhgpo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yonumen.top/gthuyeavyh.html

[S14] C：枚举
来源：http://hz.xuanzx.com/gtoskcfikw.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xuanzx.com/gtrnzuzaxc.html

[S15] C：类型转换
来源：http://hz.xinyue.icu/gtfydghums.html

(double) a / b
来源：http://hz.gaohongyu789.top/gtnvgewxyn.html

[S16] C：位操作置位
来源：http://hz.yvedp.cn/gtsbvmibem.html

x |= (1 << 3);
来源：http://hz.cqqwz.cn/gtfnkikjgp.html

[S17] C：安全拼接字符串
来源：http://hz.pycfn.com/gtiffrzlnq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.sxryk.cn/gtehvgdvgm.html

[S18] C：命令行参数
来源：http://hz.havefunace.top/gtkzfyfvip.html

int main(int argc, char **argv)
来源：http://hz.mhx1999.top/gtjvtenusy.html

[S19] C：快速排序
来源：http://hz.zhixingplan.top/gthlavaein.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.nwbrower.top/gtmzpurokg.html

[S20] C：二分查找
来源：http://hz.bjfxy.top/gtfxsvkzuf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.pengpengdd.cyou/gtgrteutbn.html

[S21] C：字符类别判断
来源：http://hz.pengpengdd.cyou/gtbszlxgla.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.wangdashe.top/gtransrxkv.html

[S22] C：字符串转数字
来源：http://hz.wangdashe.top/gtdnttnupi.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhiwuduotai.top/gtugmjheol.html

[S23] C：随机数
来源：http://hz.xziqi.cn/gtqzplpaev.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.tianlin.xyz/gtyumfhblo.html

[S24] C：获取本地时间
来源：http://hz.cqqwz.cn/gtkrnyglqu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.shangyingyoupin.top/gtqruwtrci.html

[S25] C：内存拷贝
来源：http://hz.hammf.cn/gtnvwpvrqc.html

memcpy(dst, src, n);
来源：http://hz.hnqzz.top/gtpsqpgztv.html

[S26] C：内存清零
来源：http://hz.gogol.net.cn/gtgbqazfid.html

memset(a, 0, sizeof a);
来源：http://hz.jqgfzy.top/gtxiroltut.html

[S27] C：定义常量
来源：http://hz.chenlongwang.top/gtummbefwq.html

const double PI = 3.14159;
来源：http://hz.vqdsnc.cn/gtzceqdeco.html

[S28] C：静态变量
来源：http://hz.iojbl.cn/gtocmwadjt.html

static int counter = 0;
来源：http://hz.9152youxi.cn/gtpgkjubcu.html

[S29] C：变参函数
来源：http://hz.tian-w.cn/gtzncbspmh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.xuetiantiany.cn/gtqrjamsnp.html

[S30] C：头文件保护
来源：http://hz.cdnleiting.top/gtayfnllka.html

#ifndef X_H
来源：http://hz.yangfankeji.com/gtrokxwzuc.html

#define X_H
来源：http://hz.tianlin.xyz/gtymgqiitw.html

#endif
来源：http://hz.gogol.net.cn/gtjfnhgcqd.html

[S31] C++：Hello World
来源：http://hz.ppjwa.cn/gtszvirbzg.html

#include <iostream>
来源：http://hz.zhaomingkeji.xyz/gtlwcokjwn.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jinqigfzy.top/gtzmmxqwgz.html

[S32] C++：字符串
来源：http://hz.ydjk.org.cn/gtnrnibazl.html

std::string s = "hi";  s += "!";
来源：http://hz.yj20258888.top/gtzsmrnxyc.html

[S33] C++：vector 增删
来源：http://hz.havefunace.top/gtwnslqhwl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.sufxvd.cn/gtlsoylfkg.html

[S34] C++：遍历 vector
来源：http://hz.yj20258.top/gtwqrlpias.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.52xcode.cn/gtkwfegxoh.html

[S35] C++：map
来源：http://hz.guannengcc.top/gtzkzlgfvd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xuanzx.com/gtuzpwpill.html

[S36] C++：unordered_map
来源：http://hz.zhengqikj.top/gtbkwzdnce.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj20258888.top/gtjidrzfvt.html

[S37] C++：set
来源：http://hz.pengpengdd.cyou/gtikjrxtpg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hfpthk.cn/gtmpjefjsu.html

[S38] C++：排序
来源：http://hz.jyoumei.cn/gtamizjmnv.html

std::sort(v.begin(), v.end());
来源：http://hz.pengpengdd.cyou/gtdymifwhe.html

[S39] C++：自定义比较器排序
来源：http://hz.xylfe.cn/gtwqcgfqpb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ydzc1.top/gtxymteued.html

[S40] C++：查找元素
来源：http://hz.havefunace.top/gtlwsdnhsu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.andypj.xyz/gtheshtxep.html

[S41] C++：类与构造函数
来源：http://hz.zhongyouzk.top/gtdjfavwqc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.gaohongyu789.top/gtzbwvvglo.html

[S42] C++：继承与虚函数
来源：http://hz.shanyushiyangtech.top/gthutyejll.html

class B : public Base { public: void f() override {} };
来源：http://hz.hfpthk.cn/gtjvoktanp.html

[S43] C++：智能指针
来源：http://hz.andypj.xyz/gtscxgomlh.html

auto p = std::make_unique<int>(5);
来源：http://hz.nanxuanxn.top/gtblgjqldl.html

[S44] C++：引用传参
来源：http://hz.0kj1m.cn/gttjphyuyq.html

void inc(int &x) { ++x; }
来源：http://hz.zhijiandao.cn/gtzncavqke.html

[S45] C++：lambda
来源：http://hz.andypj.xyz/gtjlxrhqdy.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.shanyushiyangtech.top/gticpgwnzs.html

[S46] C++：函数模板
来源：http://hz.gzhubu.top/gtyezodabx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.sufxvd.cn/gtvdbihzia.html

[S47] C++：结构化绑定遍历
来源：http://hz.yj202588.top/gtsiqjtphj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jinqigufen.top/gtvscoiqjs.html

[S48] C++：逐行读文件
来源：http://hz.guannengcc.top/gtsauymubt.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shanyushiyangkeji.top/gtoqpgwhhb.html

while (std::getline(in, line)) { }
来源：http://hz.chenzaomai.com/gtaxglonyi.html

[S49] C++：写文件
来源：http://hz.mhx1999.top/gtlablqpyw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.tian-w.cn/gtqzuglwei.html

[S50] C++：格式化数字
来源：http://hz.iojbl.cn/gtrhidjmlr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jqgfzy.top/gtmqzmemgc.html

[S51] C++：显式类型转换
来源：http://hz.xuanzx.com/gtjvmzysuo.html

static_cast<double>(a) / b
来源：http://hz.cheryme.top/gtdaxbuuba.html

[S52] C++：const 与 noexcept
来源：http://hz.sxryk.cn/gtuveneknr.html

int size() const noexcept { return n_; }
来源：http://hz.nwbrower.top/gtvgvihkih.html

[S53] C++：移动语义
来源：http://hz.ydjk.org.cn/gtxsroihbe.html

std::vector<int> w = std::move(v);
来源：http://hz.guannengcc.top/gtfyszyhmq.html

[S54] C++：异常处理
来源：http://hz.yongpay.top/gtjwphuutn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.nanxinkj.top/gtddhqqmyd.html

[S55] C++：结构化绑定
来源：http://hz.chenlongwang.top/gtppvucmpj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yj20258.top/gtivbqrxhl.html

[S56] C++：optional
来源：http://hz.hammf.cn/gtjrudwjbz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yuanzhike.top/gtnebcjfth.html

[S57] C++：编译期常量
来源：http://hz.0kj1m.cn/gtcgawwqnm.html

constexpr int N = 10;
来源：http://hz.nanxinkj.top/gtaedlrmhm.html

[S58] C++：命名空间
来源：http://hz.jiagoushi.top/gtwahmxtnb.html

namespace ns { int f() { return 1; } }
来源：http://hz.52xcode.cn/gtezwxyklf.html

[S59] C++：静态断言
来源：http://hz.birdmap.top/gtniwcmfaq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.pycfn.com/gthskzbomp.html

[S60] C++：遍历并删除元素
来源：http://hz.svipenyu.cn/gtnhfrktpf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jianghu66.top/gtsurqpgjl.html

================================================================================
来源：http://hz.gotoacloud.top/gticnggpks.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shuidangran.top/gtolhihxxa.html

================================================================================
来源：http://hz.gzhubu.top/gtciorasty.html

[T01] Kotlin：Hello World
来源：http://hz.ehwqpu.com/gtjblmccko.html

println("Hello")
来源：http://hz.cqqwz.cn/gttmlwszsu.html

[T02] Kotlin：变量
来源：http://hz.svipenyu.cn/gtnsnejujd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.shuidangran.top/gtzgirhtzk.html

[T03] Kotlin：字符串模板
来源：http://hz.nwbrower.top/gtuzigsvtg.html

"值: $b"
来源：http://hz.ydzc1.top/gtzgwvdzbh.html

[T04] Kotlin：空安全
来源：http://hz.yj20258888.top/gtqxwqsjsa.html

val n: String? = null;  n?.length
来源：http://hz.jianghu66.top/gtodcrfioh.html

[T05] Kotlin：when 表达式
来源：http://hz.cdnleiting.top/gtulvsdlbr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.kuanghao11.cn/gtpdodrxit.html

[T06] Kotlin：集合映射
来源：http://hz.yvedp.cn/gtynmlosuc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yj20258888.top/gtzizfinwo.html

[T07] Kotlin：集合过滤
来源：http://hz.yongpay.top/gtmwuxhsbd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.nanxinkj.top/gtzhfjdqnl.html

[T08] Kotlin：数据类
来源：http://hz.ivvv.top/gttxsvlzuz.html

data class User(val name: String, val age: Int)
来源：http://hz.52xcode.cn/gtawtpvzcg.html

[T09] Kotlin：扩展函数
来源：http://hz.jqgufenzy.top/gtygazhjud.html

fun String.exclaim() = this + "!"
来源：http://hz.hnxiangtu.top/gtmgbvxijw.html

[T10] Kotlin：默认参数
来源：http://hz.pengpengdd.cyou/gtzrmpewut.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.guannengcc.top/gtqxwabdri.html

[T11] Kotlin：协程
来源：http://hz.chenzaomai.com/gtqmpynsxr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.52xcode.cn/gttlavqmpz.html

[T12] Kotlin：解构声明
来源：http://hz.mhx1999.top/gtkymakvri.html

val (a, b) = Pair(1, 2)
来源：http://hz.smart0.xyz/gtusfcyqez.html

[T13] Kotlin：只读 Map
来源：http://hz.sysykeji.top/gtopsdeovb.html

val m = mapOf("a" to 1)
来源：http://hz.0kj1m.cn/gtgzvzloto.html

[T14] Kotlin：循环
来源：http://hz.yvedp.cn/gtwgmsfozy.html

for (i in 1..10) println(i)
来源：http://hz.zhongyouzk.top/gtqpeobvdm.html

[T15] Kotlin：接口
来源：http://hz.yanxiufei.cn/gtwjdtdayi.html

interface Shape { fun area(): Double }
来源：http://hz.daxiang520.top/gtdbcgeeej.html

[T16] Swift：Hello World
来源：http://hz.daxiang520.top/gtsirrjvwj.html

print("Hello")
来源：http://hz.havefunace.top/gtjclihsro.html

[T17] Swift：变量与常量
来源：http://hz.zhongyouzk.top/gtqvakejxd.html

var a = 1;  let b = 2
来源：http://hz.xingfuxueyuan.xyz/gtuzxrppkd.html

[T18] Swift：字符串插值
来源：http://hz.xziqi.cn/gtkodlfvye.html

"值: \(b)"
来源：http://hz.bjfxy.top/gtyehndwff.html

[T19] Swift：可选绑定
来源：http://hz.aizwys.cn/gtbdydznau.html

if let n = opt { print(n) }
来源：http://hz.shuidangran.top/gtjioaufvz.html

[T20] Swift：数组操作
来源：http://hz.nanxuanxn.top/gtejyxojtf.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.nanxuanxn.top/gtozxanrzz.html

[T21] Swift：遍历
来源：http://hz.zycfv.cn/gtiriqlmql.html

for x in a { print(x) }
来源：http://hz.guowangkeji.top/gtooxkfglx.html

[T22] Swift：字典
来源：http://hz.guowangkeji.top/gtgwmagypn.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zhixingplan.top/gtxqvjnjpv.html

[T23] Swift：函数
来源：http://hz.0kj1m.cn/gtlfuxfvtk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yuanzhike.top/gthptxcbag.html

[T24] Swift：闭包
来源：http://hz.xuetiantiany.cn/gtqztlyurk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.wangdashe.top/gtshsdtnsv.html

[T25] Swift：结构体
来源：http://hz.nwbrower.top/gtakmixgrl.html

struct P { var x: Int }
来源：http://hz.ywan-chungtsiang.top/gtkailwkws.html

[T26] Swift：类与重写
来源：http://hz.tian-w.cn/gtqwrzlorp.html

class A: Base { override func f() {} }
来源：http://hz.pengpengdd.cyou/gtfoczvtut.html

[T27] Swift：错误处理
来源：http://hz.cashguo.top/gtsewnbvvf.html

do { try f() } catch { print(error) }
来源：http://hz.xinyue.icu/gtkeusyifq.html

[T28] Swift：枚举
来源：http://hz.shangyingyoupin.top/gtmvoujbdm.html

enum Color { case red, green }
来源：http://hz.yongpay.top/gtmaaiueaw.html

[T29] Swift：guard 提前返回
来源：http://hz.cucudq.cn/gttxcahomi.html

guard let x = opt else { return }
来源：http://hz.guowangkeji.top/gtauowpezf.html

[T30] Swift：协议
来源：http://hz.jiagoushi.top/gtnqvoejsj.html

protocol Shape { func area() -> Double }
来源：http://hz.ivvv.top/gtmcotcqyi.html

[T31] Lua：Hello World
来源：http://hz.gzhubu.top/gtfykimvyt.html

print("Hello")
来源：http://hz.sysykeji.top/gteawzfhdk.html

[T32] Lua：局部变量
来源：http://hz.guannengcc.top/gtabsksbjl.html

local a = 1
来源：http://hz.bjfxy.top/gtjhuflwpe.html

[T33] Lua：表（数组）
来源：http://hz.zhongyouzk.top/gtcesijzfy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.cucudq.cn/gtimzvlezn.html

[T34] Lua：遍历表
来源：http://hz.shanyushiyangkeji.top/gtfkmbbhbn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yonumen.top/gtyyzwvkeh.html

[T35] Lua：字典表
来源：http://hz.pycfn.com/gtenmhipdc.html

local d = { a = 1 };  d.b = 2
来源：http://hz.svipenyu.cn/gtrhttnslx.html

[T36] Lua：函数
来源：http://hz.shuidangran.top/gtlcqdzaej.html

function add(a, b) return a + b end
来源：http://hz.sweek.top/gtniqmicgc.html

[T37] Lua：字符串拼接
来源：http://hz.yonumen.top/gtujnwkfyk.html

"a" .. "b"
来源：http://hz.aizwys.cn/gtpzxcokqf.html

[T38] Lua：条件
来源：http://hz.zhongyouzk.top/gtvikptrgn.html

if x > 0 then print("正") end
来源：http://hz.shzxlz.cn/gtuujodepd.html

[T39] Lua：模式匹配
来源：http://hz.kuanghao11.cn/gtwjbnbpem.html

string.find(s, "%d+")
来源：http://hz.ydjk.org.cn/gtxjhfyuog.html

[T40] Lua：元表
来源：http://hz.shuidangran.top/gtpmoqcltc.html

setmetatable({}, { __index = base })
来源：http://hz.svipenyu.cn/gtyxfuixqq.html

[T41] Perl：Hello World
来源：http://hz.daria6918.cn/gtjgezqvul.html

print "Hello\n";
来源：http://hz.xingfuxueyuan.xyz/gtefscobki.html

[T42] Perl：变量类型
来源：http://hz.redwolf501.top/gtriljsrtr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yonumen.top/gtdotcjtbv.html

[T43] Perl：字符串插值
来源：http://hz.jianghu66.top/gtdhdkadqm.html

"值: $a"
来源：http://hz.ehwqpu.com/gthlralztf.html

[T44] Perl：条件
来源：http://hz.yongpay.top/gtjqoxjcfr.html

if ($a > 0) { print "正"; }
来源：http://hz.jiagoushi.top/gtuzeddqhl.html

[T45] Perl：数组遍历
来源：http://hz.sxryk.cn/gtwcbxojrj.html

for my $x (@arr) { print $x; }
来源：http://hz.sxryk.cn/gtrjcmqikp.html

[T46] Perl：哈希操作
来源：http://hz.xuetiantiany.cn/gttncodfdg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.0kj1m.cn/gteycojsfi.html

[T47] Perl：正则捕获
来源：http://hz.ydzc1.top/gtqblhdjor.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yj202588.top/gtvslsduii.html

[T48] Perl：正则替换
来源：http://hz.shangyingyoupin.top/gtjtjtsdei.html

$s =~ s/old/new/g;
来源：http://hz.xylfe.cn/gtbrujxoes.html

[T49] Perl：函数
来源：http://hz.ehwqpu.com/gtskowlber.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.svipenyu.cn/gtbeulhrrl.html

[T50] Perl：逐行读文件
来源：http://hz.yonumen.top/gtiurjhjek.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jiagoushi.top/gtbdmvfpmz.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.cdnleiting.top/gteiyhvvrm.html

[T51] Scala：Hello World
来源：http://hz.ydjk.org.cn/gtxcbqjqbn.html

println("Hello")
来源：http://hz.yvedp.cn/gtbogxkgfu.html

[T52] Scala：变量
来源：http://hz.ybcxt.top/gtxcytmflz.html

val a = 1;  var b = 2
来源：http://hz.nanxuanxn.top/gtohumlbcm.html

[T53] Scala：字符串插值
来源：http://hz.wangshuangyany.cn/gtnludvane.html

s"值: $b"
来源：http://hz.yj20258.top/gtraoyrisb.html

[T54] Scala：集合映射
来源：http://hz.zhijiandao.cn/gtplszwvnw.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.shanyushiyangtech.top/gtgzfpjnmm.html

[T55] Scala：集合过滤
来源：http://hz.jianghu66.top/gtxzenjujo.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.zhijiandao.cn/gtnvxtuong.html

[T56] Scala：样例类
来源：http://hz.gzhubu.top/gtzhgicyvc.html

case class User(name: String, age: Int)
来源：http://hz.gzhubu.top/gtqkypttif.html

[T57] Scala：模式匹配
来源：http://hz.quarkkingdee.top/gtoytrscrw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.chenzaomai.com/gtfmjzrxyl.html

[T58] Scala：函数定义
来源：http://hz.mhx1999.top/gtpezrozgt.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.guannengcc.top/gtcjfqlpqq.html

[T59] Scala：循环
来源：http://hz.yvedp.cn/gtzbcuvysi.html

for (i <- 1 to 10) println(i)
来源：http://hz.xinyue.icu/gtluqejhip.html

[T60] Scala：折叠
来源：http://hz.316326.xyz/gtqngwohgb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.kuanghao11.cn/gtunvkeymh.html

================================================================================
来源：http://hz.yvedp.cn/gtpghtvrsv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.redwolf501.top/gtmjkdiqvj.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtaysbmfpr.html

[U01] Py：创建虚拟环境
来源：http://hz.mhx1999.top/gtnmegjanw.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.gaohongyu789.top/gthatxmrtd.html

[U02] Py：导出 / 安装依赖
来源：http://hz.xuanzx.com/gtilynjhpt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jyoumei.cn/gtiwivudnf.html

[U03] Py：加载 .env 配置
来源：http://hz.9152youxi.cn/gttzfvibsu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.shanyushiyangtech.top/gtgpoamwmg.html

[U04] Py：变量调试打印
来源：http://hz.sxryk.cn/gtdjxteyna.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.meibo888.top/gtpwryzmdd.html

[U05] Py：列表去重且保序
来源：http://hz.cdnleiting.top/gtwkbwnpkd.html

list(dict.fromkeys(arr))
来源：http://hz.sufxvd.cn/gtiendpjku.html

[U06] Py：合并两个字典
来源：http://hz.kuanghao11.cn/gtsdkoevls.html

{**a, **b}
来源：http://hz.xingfuxueyuan.xyz/gtmqoqeere.html

[U07] Py：反转字典键值
来源：http://hz.zhijiandao.cn/gtwjoujmpw.html

{v: k for k, v in d.items()}
来源：http://hz.guannengcc.top/gtrxbtrduv.html

[U08] Py：展平二维列表
来源：http://hz.gzhubu.top/gtfkvjkcvf.html

[y for x in nested for y in x]
来源：http://hz.tian-w.cn/gtnqoaukct.html

[U09] Py：字典取最大值的键
来源：http://hz.xuetiantiany.cn/gtjqywcofd.html

max(d, key=d.get)
来源：http://hz.shuidangran.top/gtfyjmjtsj.html

[U10] Py：按值排序字典
来源：http://hz.sxryk.cn/gtadyxefgc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yangfankeji.com/gthhcbwvpb.html

[U11] Py：生成器表达式
来源：http://hz.yuanzhike.top/gtbbnimjzb.html

(x * 2 for x in arr)
来源：http://hz.shzxlz.cn/gtwghktvfi.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.hnqzz.top/gtmructasf.html

Counter(arr).most_common(3)
来源：http://hz.jinghuilouyu.cn/gttwnpvqvc.html

[U13] Py：固定长度队列
来源：http://hz.shanyushiyangtech.top/gtchahrcpp.html

deque(maxlen=10)
来源：http://hz.vqdsnc.cn/gtadmzhxbb.html

[U14] Py：分组收集到列表
来源：http://hz.redwolf501.top/gtdmhycpku.html

defaultdict(list)
来源：http://hz.redwolf501.top/gtpnjfbcoh.html

[U15] Py：高精度计时
来源：http://hz.sufxvd.cn/gtmwhlwjgg.html

t = time.perf_counter()
来源：http://hz.sysykeji.top/gtthkjtuyr.html

[U16] Py：命令行参数解析
来源：http://hz.xuanzx.com/gthtksflsq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.ydjk.org.cn/gtoivpbmue.html

[U17] Py：初始化日志
来源：http://hz.c1oappe.top/gtdlkflhws.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yj20258.top/gtbagrahrn.html

[U18] Py：预编译正则
来源：http://hz.yueranfly.top/gtwejeetxs.html

pat = re.compile(r"\d+")
来源：http://hz.zhiwuduotai.top/gtqmsyffvt.html

[U19] Py：正则替换带回调
来源：http://hz.redwolf501.top/gtxdlmydeq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.ydjk.org.cn/gtqayamsan.html

[U20] Py：缓存函数结果
来源：http://hz.hnxiangtu.top/gthegflnnl.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yanxiufei.cn/gtxgzglcdd.html

[U21] Py：自定义上下文管理器
来源：http://hz.cqqwz.cn/gtnaartvzr.html

@contextlib.contextmanager
来源：http://hz.yj202588.top/gtyjjevtfa.html

[U22] Py：矩阵转置
来源：http://hz.daxiang520.top/gtawgaraks.html

list(zip(*m))
来源：http://hz.jiagoushi.top/gtdhujpoyu.html

[U23] Py：分块读取大文件
来源：http://hz.sxryk.cn/gthwrxsmte.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.zhengqikj.top/gtbogumyfz.html

[U24] Py：路径操作
来源：http://hz.zdqjudy.top/gtbdwevobe.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.cucudq.cn/gtvdntmeum.html

[U25] Py：CSV 按字典读
来源：http://hz.yangfankeji.com/gtpnmmbyxg.html

csv.DictReader(f)
来源：http://hz.ywan-chungtsiang.top/gtsemsyfjx.html

[U26] Py：并发下载
来源：http://hz.nanxuanxn.top/gtplnnurih.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.fzhhl.top/gtxrzkmodf.html

[U27] Py：异步 HTTP
来源：http://hz.daxiang520.top/gthxnxtmqe.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.cashguo.top/gthvbacxac.html

[U28] Py：类型别名
来源：http://hz.xuanzx.com/gtjqljvqjf.html

UserId = int
来源：http://hz.yuanzhike.top/gtjgmoncxy.html

[U29] Py：属性校验
来源：http://hz.yongpay.top/gtglgqbfyo.html

@property 与 @x.setter 配合
来源：http://hz.meibo888.top/gtzxsnijpo.html

[U30] Py：数据类
来源：http://hz.nanxinkj.top/gtqgqkbpzm.html

@dataclass(slots=True)
来源：http://hz.pengpengdd.cyou/gtbmbirric.html


<!-- 参考信息 -->