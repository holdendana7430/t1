代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yj202588.top/gtjauizuzy.html

[S08] C：动态内存分配与释放
来源：http://hz.meibo888.top/gttnajumpm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.daxiang520.top/gtlnefzhdw.html

[S09] C：结构体定义与初始化
来源：http://hz.hywenlv.cn/gtztdxmfvi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.shanyushiyangkeji.top/gtisazrmqt.html

[S10] C：指针与解引用
来源：http://hz.xingfuxueyuan.xyz/gtvexlzgqx.html

int *p = &a;  *p = 5;
来源：http://hz.redwolf501.top/gtknyqmwwn.html

[S11] C：逐行读文件
来源：http://hz.ywan-chungtsiang.top/gtwcifzjvw.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.xziqi.cn/gtqfpmspnc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.gogol.net.cn/gtwuapnyme.html

fclose(f);
来源：http://hz.xuetiantiany.cn/gtxhmrrjbq.html

[S12] C：写文件
来源：http://hz.ivvv.top/gtklinoyed.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.pycfn.com/gtgltuhiar.html

[S13] C：宏定义
来源：http://hz.gotoacloud.top/gttdwfisxx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.sxryk.cn/gtvhbhinmy.html

[S14] C：枚举
来源：http://hz.jlsjyb.cn/gtjmtlfzqf.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.cucudq.cn/gtsumnhpfo.html

[S15] C：类型转换
来源：http://hz.yongpay.top/gtmswrmxyh.html

(double) a / b
来源：http://hz.ehwqpu.com/gtgmtwpwyx.html

[S16] C：位操作置位
来源：http://hz.nanxinkj.top/gtrnjyijzn.html

x |= (1 << 3);
来源：http://hz.fzhhl.top/gtogpqcncy.html

[S17] C：安全拼接字符串
来源：http://hz.hongshengwenyu.top/gtuqfchnpo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jinghuilouyu.cn/gtclfwqmal.html

[S18] C：命令行参数
来源：http://hz.yuanzhike.top/gtsfkotwes.html

int main(int argc, char **argv)
来源：http://hz.dianchejie.cn/gtmwvzgbph.html

[S19] C：快速排序
来源：http://hz.ivvv.top/gtpgrntqme.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shuidangran.top/gtzovhvzqt.html

[S20] C：二分查找
来源：http://hz.pengpengdd.cyou/gtljhwhytk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.316326.xyz/gtjjopltuw.html

[S21] C：字符类别判断
来源：http://hz.zycfv.cn/gtumwzsnsl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.nanxuanxn.top/gthczlsorl.html

[S22] C：字符串转数字
来源：http://hz.yueranfly.top/gtvkoxfvah.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ywan-chungtsiang.top/gtlhevixsn.html

[S23] C：随机数
来源：http://hz.yueranfly.top/gtonscrcqk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.bjfxy.top/gtfssxkeyt.html

[S24] C：获取本地时间
来源：http://hz.yvedp.cn/gtyjweorop.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.shzxlz.cn/gtfsdmblki.html

[S25] C：内存拷贝
来源：http://hz.tanke756.top/gtjkuumvkx.html

memcpy(dst, src, n);
来源：http://hz.ydjk.org.cn/gtgjoibonq.html

[S26] C：内存清零
来源：http://hz.shanyushiyangtech.top/gtbeawvwcw.html

memset(a, 0, sizeof a);
来源：http://hz.cheryme.top/gtmuspkstz.html

[S27] C：定义常量
来源：http://hz.ybcxt.top/gthpopngwx.html

const double PI = 3.14159;
来源：http://hz.zhaomingkeji.xyz/gtteckzuie.html

[S28] C：静态变量
来源：http://hz.xziqi.cn/gtpnpvgxsr.html

static int counter = 0;
来源：http://hz.hongshengwenyu.top/gtgnqyngho.html

[S29] C：变参函数
来源：http://hz.gaohongyu789.top/gtpxbtwbyi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jinqigufen.top/gtpnvkqvsi.html

[S30] C：头文件保护
来源：http://hz.quarkkingdee.top/gtnljqqxei.html

#ifndef X_H
来源：http://hz.birdmap.top/gtyfeeuxgl.html

#define X_H
来源：http://hz.shanyushiyangkeji.top/gtuahoupsy.html

#endif
来源：http://hz.tanke756.top/gtbjetlxru.html

[S31] C++：Hello World
来源：http://hz.guowangkeji.top/gtjqvqeazb.html

#include <iostream>
来源：http://hz.yueranfly.top/gtmatlxvia.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.kuanghao11.cn/gtyrjsxcvy.html

[S32] C++：字符串
来源：http://hz.yj202588.top/gtfswnryss.html

std::string s = "hi";  s += "!";
来源：http://hz.gotoacloud.top/gtuoczmgkb.html

[S33] C++：vector 增删
来源：http://hz.sweek.top/gtgiewwjsq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.gaohongyu789.top/gtnivkgrhc.html

[S34] C++：遍历 vector
来源：http://hz.svipenyu.cn/gtlqpnpegx.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.snrcjt.cn/gtykyenqtx.html

[S35] C++：map
来源：http://hz.yj20258.top/gtibwvxmtq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.dianchejie.cn/gtkahhipqo.html

[S36] C++：unordered_map
来源：http://hz.yuanzhike.top/gtetxjqnrc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhijiandao.cn/gtlkbeobuf.html

[S37] C++：set
来源：http://hz.0kj1m.cn/gtryfeovdm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jianghu66.top/gtxoahgbce.html

[S38] C++：排序
来源：http://hz.hammf.cn/gtpxhsarwu.html

std::sort(v.begin(), v.end());
来源：http://hz.gaohongyu789.top/gtlhswuerf.html

[S39] C++：自定义比较器排序
来源：http://hz.nanxinkj.top/gtyyzwcyvj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.sweek.top/gtbenireub.html

[S40] C++：查找元素
来源：http://hz.nwbrower.top/gtetxwrvby.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.c1oappe.top/gtykfubudy.html

[S41] C++：类与构造函数
来源：http://hz.ydzc1.top/gttlxlzqoc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xziqi.cn/gtsoethpgs.html

[S42] C++：继承与虚函数
来源：http://hz.quarkkingdee.top/gtdpxpfiub.html

class B : public Base { public: void f() override {} };
来源：http://hz.chenjidiqi.icu/gtlzzwkepq.html

[S43] C++：智能指针
来源：http://hz.gzhubu.top/gtncqkruwm.html

auto p = std::make_unique<int>(5);
来源：http://hz.9152youxi.cn/gtxtwgnjxi.html

[S44] C++：引用传参
来源：http://hz.sweek.top/gtsnhksyty.html

void inc(int &x) { ++x; }
来源：http://hz.yj202588.top/gttuensotc.html

[S45] C++：lambda
来源：http://hz.jqgfzy.top/gtykjdsouz.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yuxming.cn/gtzaswynlc.html

[S46] C++：函数模板
来源：http://hz.xylfe.cn/gtfhkhppte.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhongyouzk.top/gtvwxjldjb.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhixingplan.top/gtrbycgucq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yj20258.top/gtofcfeaio.html

[S48] C++：逐行读文件
来源：http://hz.0kj1m.cn/gtaezkgyev.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yonumen.top/gtkfomfhzq.html

while (std::getline(in, line)) { }
来源：http://hz.fzhhl.top/gtuckbklfn.html

[S49] C++：写文件
来源：http://hz.jyoumei.cn/gttfikroet.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ppjwa.cn/gthwvcvsya.html

[S50] C++：格式化数字
来源：http://hz.bjfxy.top/gtxwfmpfyn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhongyouzk.top/gtqhngkgzd.html

[S51] C++：显式类型转换
来源：http://hz.guannengcc.top/gtgxubdrkz.html

static_cast<double>(a) / b
来源：http://hz.cheryme.top/gthnpebscm.html

[S52] C++：const 与 noexcept
来源：http://hz.jinyuanbaomall.cn/gtrpkygzpd.html

int size() const noexcept { return n_; }
来源：http://hz.cdnleiting.top/gtkuirjogy.html

[S53] C++：移动语义
来源：http://hz.gaohongyu789.top/gtuxqjeeig.html

std::vector<int> w = std::move(v);
来源：http://hz.bjfxy.top/gtokcqoygc.html

[S54] C++：异常处理
来源：http://hz.haohaochexian.top/gtbsjazikh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ywan-chungtsiang.top/gtbvktuayn.html

[S55] C++：结构化绑定
来源：http://hz.ywan-chungtsiang.top/gtyhlqfthw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.xziqi.cn/gtfcrdkhcw.html

[S56] C++：optional
来源：http://hz.feifeiyinyue.top/gtwgqmyzqv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.quarkkingdee.top/gtazlzldnq.html

[S57] C++：编译期常量
来源：http://hz.jqgfzy.top/gthhaisyts.html

constexpr int N = 10;
来源：http://hz.tian-w.cn/gtlecfhjmi.html

[S58] C++：命名空间
来源：http://hz.feifeiyinyue.top/gthhohmjox.html

namespace ns { int f() { return 1; } }
来源：http://hz.hnqzz.top/gtftldemxk.html

[S59] C++：静态断言
来源：http://hz.hnxiangtu.top/gtulrpleib.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ywan-chungtsiang.top/gtknusnsrr.html

[S60] C++：遍历并删除元素
来源：http://hz.feifeiyinyue.top/gtopmbgoop.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.pycfn.com/gtbuxbzmea.html

================================================================================
来源：http://hz.ydjk.org.cn/gtslqkjcae.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.fzhhl.top/gtfjosofek.html

================================================================================
来源：http://hz.yueranfly.top/gtyyakkuko.html

[T01] Kotlin：Hello World
来源：http://hz.fzhhl.top/gtpkeifzqa.html

println("Hello")
来源：http://hz.gotoacloud.top/gtplynhjga.html

[T02] Kotlin：变量
来源：http://hz.sufxvd.cn/gtzjqygzay.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jinqigfzy.top/gtqjolvslp.html

[T03] Kotlin：字符串模板
来源：http://hz.zhaomingkeji.xyz/gthlxsxliq.html

"值: $b"
来源：http://hz.shanyushiyangtech.top/gtwdomuely.html

[T04] Kotlin：空安全
来源：http://hz.shanyushiyangtech.top/gtzumlrzkl.html

val n: String? = null;  n?.length
来源：http://hz.c1oappe.top/gtqxmjxiob.html

[T05] Kotlin：when 表达式
来源：http://hz.jyoumei.cn/gtdjhnxwrx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jianghu66.top/gtkhndgxsw.html

[T06] Kotlin：集合映射
来源：http://hz.zdqjudy.top/gthmvwbnpu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hnqzz.top/gtpfwxhtfl.html

[T07] Kotlin：集合过滤
来源：http://hz.dianchejie.cn/gtjupnpnws.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.cashguo.top/gtqfhjtxpw.html

[T08] Kotlin：数据类
来源：http://hz.pycfn.com/gtvbfheljg.html

data class User(val name: String, val age: Int)
来源：http://hz.ydjk.org.cn/gtbxvydsmg.html

[T09] Kotlin：扩展函数
来源：http://hz.quarkkingdee.top/gtttdstweo.html

fun String.exclaim() = this + "!"
来源：http://hz.jianghu66.top/gtaemsesvw.html

[T10] Kotlin：默认参数
来源：http://hz.xziqi.cn/gtrohdvsea.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.quarkkingdee.top/gtufspqwcs.html

[T11] Kotlin：协程
来源：http://hz.quarkkingdee.top/gtbwmkfqgs.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.pycfn.com/gtfuxxlsyp.html

[T12] Kotlin：解构声明
来源：http://hz.yanxiufei.cn/gtapbvajdx.html

val (a, b) = Pair(1, 2)
来源：http://hz.yanxiufei.cn/gtntjevqme.html

[T13] Kotlin：只读 Map
来源：http://hz.zhoulong.xyz/gtmgivqewc.html

val m = mapOf("a" to 1)
来源：http://hz.snrcjt.cn/gtyebpzwmw.html

[T14] Kotlin：循环
来源：http://hz.ehwqpu.com/gtsgkflani.html

for (i in 1..10) println(i)
来源：http://hz.tian-w.cn/gtreutkppw.html

[T15] Kotlin：接口
来源：http://hz.haohaochexian.top/gtolpacfbc.html

interface Shape { fun area(): Double }
来源：http://hz.gogol.net.cn/gtljkylwdh.html

[T16] Swift：Hello World
来源：http://hz.c1oappe.top/gtjozlmbvk.html

print("Hello")
来源：http://hz.pycfn.com/gtifluqofb.html

[T17] Swift：变量与常量
来源：http://hz.cucudq.cn/gtdakyoupa.html

var a = 1;  let b = 2
来源：http://hz.xylfe.cn/gtayupjhle.html

[T18] Swift：字符串插值
来源：http://hz.kuanghao11.cn/gtdzeuaozr.html

"值: \(b)"
来源：http://hz.shzxlz.cn/gthtgfwrmj.html

[T19] Swift：可选绑定
来源：http://hz.tianlin.xyz/gtjkfgjtmp.html

if let n = opt { print(n) }
来源：http://hz.vqdsnc.cn/gteglcpovd.html

[T20] Swift：数组操作
来源：http://hz.guannengcc.top/gtqaphqwvt.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.ivvv.top/gtlrvrpkqg.html

[T21] Swift：遍历
来源：http://hz.ydzc1.top/gtxpfxnont.html

for x in a { print(x) }
来源：http://hz.yuxming.cn/gtnkfnojiw.html

[T22] Swift：字典
来源：http://hz.birdmap.top/gtwuxknqng.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ywan-chungtsiang.top/gtzduekogj.html

[T23] Swift：函数
来源：http://hz.ivvv.top/gtlwyimjtt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.chenjidiqi.icu/gtekxzjets.html

[T24] Swift：闭包
来源：http://hz.nanxuanxn.top/gtsfoacugl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.wangshuangyany.cn/gtqqalfgci.html

[T25] Swift：结构体
来源：http://hz.chenzaomai.com/gtuhonyqxa.html

struct P { var x: Int }
来源：http://hz.havefunace.top/gtjeppfgxu.html

[T26] Swift：类与重写
来源：http://hz.dianchejie.cn/gtdmggxmpt.html

class A: Base { override func f() {} }
来源：http://hz.kuanghao11.cn/gtwbyxqpzw.html

[T27] Swift：错误处理
来源：http://hz.gogol.net.cn/gtikqwilwi.html

do { try f() } catch { print(error) }
来源：http://hz.fengsongda.top/gtetdrypbs.html

[T28] Swift：枚举
来源：http://hz.yvedp.cn/gtilmdwpsy.html

enum Color { case red, green }
来源：http://hz.pycfn.com/gtelrvweig.html

[T29] Swift：guard 提前返回
来源：http://hz.iojbl.cn/gtsilndwmz.html

guard let x = opt else { return }
来源：http://hz.zhiwuduotai.top/gttrtezbik.html

[T30] Swift：协议
来源：http://hz.jqgufenzy.top/gtcekewpna.html

protocol Shape { func area() -> Double }
来源：http://hz.guannengcc.top/gtchtkohbj.html

[T31] Lua：Hello World
来源：http://hz.ybcxt.top/gtkonuxrgb.html

print("Hello")
来源：http://hz.hammf.cn/gtjycoiniv.html

[T32] Lua：局部变量
来源：http://hz.daxiang520.top/gtjazqnxxt.html

local a = 1
来源：http://hz.ppjwa.cn/gtkgljsuzz.html

[T33] Lua：表（数组）
来源：http://hz.bjfxy.top/gtvqskzomk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jlsjyb.cn/gtymxkbvkl.html

[T34] Lua：遍历表
来源：http://hz.sxryk.cn/gtwmuglajj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.ydzc1.top/gtzvdtuvpv.html

[T35] Lua：字典表
来源：http://hz.jqgfzy.top/gtuuhleehw.html

local d = { a = 1 };  d.b = 2
来源：http://hz.zycfv.cn/gtqdtxayxy.html

[T36] Lua：函数
来源：http://hz.andypj.xyz/gtvhifbrkg.html

function add(a, b) return a + b end
来源：http://hz.chenlongwang.top/gtwjsjzgrn.html

[T37] Lua：字符串拼接
来源：http://hz.shuidangran.top/gtnsswsvbr.html

"a" .. "b"
来源：http://hz.havefunace.top/gtdqlcmnpy.html

[T38] Lua：条件
来源：http://hz.mhx1999.top/gtbgsghofk.html

if x > 0 then print("正") end
来源：http://hz.yuxming.cn/gtcyjoemmy.html

[T39] Lua：模式匹配
来源：http://hz.shangyingyoupin.top/gtzyhtxwes.html

string.find(s, "%d+")
来源：http://hz.ppjwa.cn/gtxksffzcs.html

[T40] Lua：元表
来源：http://hz.gzhubu.top/gtuayhpzrc.html

setmetatable({}, { __index = base })
来源：http://hz.ivvv.top/gtazwtllzi.html

[T41] Perl：Hello World
来源：http://hz.52xcode.cn/gtaqduaiqu.html

print "Hello\n";
来源：http://hz.gzhubu.top/gtdhcrwxty.html

[T42] Perl：变量类型
来源：http://hz.shanyushiyangkeji.top/gtslrdsooi.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.daxiang520.top/gtuiahflgk.html

[T43] Perl：字符串插值
来源：http://hz.iojbl.cn/gttvjmmcqy.html

"值: $a"
来源：http://hz.daria6918.cn/gtvaljhcmk.html

[T44] Perl：条件
来源：http://hz.mhx1999.top/gtkutxqevc.html

if ($a > 0) { print "正"; }
来源：http://hz.jianghu66.top/gtxsvxqgxu.html

[T45] Perl：数组遍历
来源：http://hz.ehwqpu.com/gtdsehhzrn.html

for my $x (@arr) { print $x; }
来源：http://hz.svipenyu.cn/gtvtgmklec.html

[T46] Perl：哈希操作
来源：http://hz.hywenlv.cn/gtskcslqhl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jinyuanbaomall.cn/gtkrvzhrcb.html

[T47] Perl：正则捕获
来源：http://hz.jiagoushi.top/gtzooldedq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.fzhhl.top/gteaenldag.html

[T48] Perl：正则替换
来源：http://hz.smart0.xyz/gtkyzjmgwd.html

$s =~ s/old/new/g;
来源：http://hz.zhiwuduotai.top/gtuvejqrjq.html

[T49] Perl：函数
来源：http://hz.fengsongda.top/gtszxsugct.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.pengpengdd.cyou/gtuworehci.html

[T50] Perl：逐行读文件
来源：http://hz.cheryme.top/gtxwheyuam.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.hnqzz.top/gtwjvmzvjk.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.daria6918.cn/gtpxtxexmp.html

[T51] Scala：Hello World
来源：http://hz.ydzc1.top/gtnikshxnm.html

println("Hello")
来源：http://hz.shzxlz.cn/gtlhgdcmzz.html

[T52] Scala：变量
来源：http://hz.ppjwa.cn/gtyrfjmsqw.html

val a = 1;  var b = 2
来源：http://hz.pengpengdd.cyou/gtfqoedgrp.html

[T53] Scala：字符串插值
来源：http://hz.ivvv.top/gtugwpyzcl.html

s"值: $b"
来源：http://hz.shangyingyoupin.top/gtknjvnzch.html

[T54] Scala：集合映射
来源：http://hz.hongshengwenyu.top/gthqkjalno.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yangfankeji.com/gttbohmlhx.html

[T55] Scala：集合过滤
来源：http://hz.52xcode.cn/gtlycpranv.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.tian-w.cn/gtywdgmlgd.html

[T56] Scala：样例类
来源：http://hz.zhongyouzk.top/gtlrbfknwl.html

case class User(name: String, age: Int)
来源：http://hz.hammf.cn/gtzpkddfbr.html

[T57] Scala：模式匹配
来源：http://hz.xingfuxueyuan.xyz/gtvfslgadj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.havefunace.top/gtsxszebcm.html

[T58] Scala：函数定义
来源：http://hz.iojbl.cn/gtpiguiscb.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yj202588.top/gtoxdgzaxf.html

[T59] Scala：循环
来源：http://hz.hammf.cn/gtichbxrxw.html

for (i <- 1 to 10) println(i)
来源：http://hz.fengsongda.top/gtmvoljdmh.html

[T60] Scala：折叠
来源：http://hz.ehwqpu.com/gtrfqgdgur.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.cdnleiting.top/gtkiqusvxx.html

================================================================================
来源：http://hz.xylfe.cn/gtpdytlqru.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jinqigfzy.top/gtphvwroel.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtvamtwcif.html

[U01] Py：创建虚拟环境
来源：http://hz.chenlongwang.top/gtebslewoj.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.zhoulong.xyz/gtrldjlbho.html

[U02] Py：导出 / 安装依赖
来源：http://hz.gogol.net.cn/gtzwmfzszn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yvedp.cn/gtbbxpfije.html

[U03] Py：加载 .env 配置
来源：http://hz.xziqi.cn/gtayhlksvg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.guowangkeji.top/gtpjpgsnog.html

[U04] Py：变量调试打印
来源：http://hz.vqdsnc.cn/gtlyishpbt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.316326.xyz/gtqwjomteq.html

[U05] Py：列表去重且保序
来源：http://hz.zhijiandao.cn/gtywmqtlvb.html

list(dict.fromkeys(arr))
来源：http://hz.hywenlv.cn/gtbssjuewu.html

[U06] Py：合并两个字典
来源：http://hz.9152youxi.cn/gtswbkgrlm.html

{**a, **b}
来源：http://hz.gogol.net.cn/gtfzndbehl.html

[U07] Py：反转字典键值
来源：http://hz.jianghu66.top/gtfycrsfif.html

{v: k for k, v in d.items()}
来源：http://hz.c1oappe.top/gtfwunygeg.html

[U08] Py：展平二维列表
来源：http://hz.chenjidiqi.icu/gtcpcuiymf.html

[y for x in nested for y in x]
来源：http://hz.dashuyun.cn/gtxzpqeuwo.html

[U09] Py：字典取最大值的键
来源：http://hz.gzhubu.top/gtvaszqkzc.html

max(d, key=d.get)
来源：http://hz.jiagoushi.top/gteylymqsf.html

[U10] Py：按值排序字典
来源：http://hz.mhx1999.top/gtvdtturbv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yongpay.top/gtjhvgmyvg.html

[U11] Py：生成器表达式
来源：http://hz.shanyushiyangkeji.top/gtwwfcgnpf.html

(x * 2 for x in arr)
来源：http://hz.bjfxy.top/gtahqebmga.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yj20258888.top/gtqctmxnhm.html

Counter(arr).most_common(3)
来源：http://hz.nanxinkj.top/gtxpskatuo.html

[U13] Py：固定长度队列
来源：http://hz.sufxvd.cn/gtvyrmpvhj.html

deque(maxlen=10)
来源：http://hz.shanyushiyangtech.top/gtsgahocig.html

[U14] Py：分组收集到列表
来源：http://hz.nwbrower.top/gtjyjptrev.html

defaultdict(list)
来源：http://hz.pycfn.com/gtilqaqdgu.html

[U15] Py：高精度计时
来源：http://hz.jqgfzy.top/gtqscfbfwt.html

t = time.perf_counter()
来源：http://hz.yj20258.top/gtvdbxuxto.html

[U16] Py：命令行参数解析
来源：http://hz.nanxuanxn.top/gtjsjtxiek.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.feifeiyinyue.top/gtyqfkqhax.html

[U17] Py：初始化日志
来源：http://hz.ywan-chungtsiang.top/gtrzfgopgw.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.ivvv.top/gtwmzmjorc.html

[U18] Py：预编译正则
来源：http://hz.jinqigufen.top/gtpftyzmed.html

pat = re.compile(r"\d+")
来源：http://hz.hongshengwenyu.top/gtqagbwepi.html

[U19] Py：正则替换带回调
来源：http://hz.0kj1m.cn/gtkvexsbhi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yangfankeji.com/gtyhxkxrwc.html

[U20] Py：缓存函数结果
来源：http://hz.cashguo.top/gtuvlzuomj.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zhengqikj.top/gtjhiwatld.html

[U21] Py：自定义上下文管理器
来源：http://hz.birdmap.top/gtitoaiimi.html

@contextlib.contextmanager
来源：http://hz.tanke756.top/gtmwxfdqts.html

[U22] Py：矩阵转置
来源：http://hz.yj20258.top/gtbkhyufnv.html

list(zip(*m))
来源：http://hz.wangdashe.top/gtbxeehejd.html

[U23] Py：分块读取大文件
来源：http://hz.sysykeji.top/gtatoqjpsi.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.jiagoushi.top/gtjghzalbb.html

[U24] Py：路径操作
来源：http://hz.sxryk.cn/gtmeoyxlrk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.cashguo.top/gthnolisco.html

[U25] Py：CSV 按字典读
来源：http://hz.c1oappe.top/gtykvhndaq.html

csv.DictReader(f)
来源：http://hz.zycfv.cn/gtrljmvego.html

[U26] Py：并发下载
来源：http://hz.yvedp.cn/gtxvjdkgqb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.yongpay.top/gtdwggujso.html

[U27] Py：异步 HTTP
来源：http://hz.hysaishi.cn/gtxpyelvpu.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.52xcode.cn/gtcqbzgxdz.html

[U28] Py：类型别名
来源：http://hz.bjfxy.top/gtzjgketoi.html

UserId = int
来源：http://hz.daxiang520.top/gtvxeyotyg.html

[U29] Py：属性校验
来源：http://hz.cashguo.top/gtxlymuxbl.html

@property 与 @x.setter 配合
来源：http://hz.feifeiyinyue.top/gtbokvknrg.html

[U30] Py：数据类
来源：http://hz.hnqzz.top/gtwiavsrvs.html

@dataclass(slots=True)
来源：http://hz.sweek.top/gtvehpqony.html


<!-- 参考信息 -->