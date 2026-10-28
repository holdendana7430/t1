代发 wailian999

strlen(s)
来源：http://hz.tianlin.xyz/gttzvbuctz.html

[S06] C：字符串比较
来源：http://hz.cqqwz.cn/gthqjexmxt.html

strcmp(a, b) == 0
来源：http://hz.jinghuilouyu.cn/gtzgwqyxnh.html

[S07] C：数组遍历求和
来源：http://hz.hongshengwenyu.top/gtvcksscie.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.gogol.net.cn/gtszpcjpiu.html

[S08] C：动态内存分配与释放
来源：http://hz.9152youxi.cn/gtqpplhlef.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xziqi.cn/gttozcbcxr.html

[S09] C：结构体定义与初始化
来源：http://hz.jqgufenzy.top/gtdkqufwwr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.sweek.top/gtevtzetpv.html

[S10] C：指针与解引用
来源：http://hz.ydzc1.top/gtgcxxsjfd.html

int *p = &a;  *p = 5;
来源：http://hz.hammf.cn/gtibalinkz.html

[S11] C：逐行读文件
来源：http://hz.hongshengwenyu.top/gtumyaznpk.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.sxryk.cn/gthckagwyu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.xingfuxueyuan.xyz/gtspowtvyv.html

fclose(f);
来源：http://hz.zhongyouzk.top/gtgpxazggt.html

[S12] C：写文件
来源：http://hz.snrcjt.cn/gtqkfcvoxs.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.dashuyun.cn/gtfzwiodhk.html

[S13] C：宏定义
来源：http://hz.shanyushiyangkeji.top/gtrvkewiqb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.fengsongda.top/gtuuvujwht.html

[S14] C：枚举
来源：http://hz.chenlongwang.top/gtdzzcicqf.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yangfankeji.com/gtpizmqjwm.html

[S15] C：类型转换
来源：http://hz.nanxinkj.top/gtcfbskgfl.html

(double) a / b
来源：http://hz.yangfankeji.com/gteqhwhvzf.html

[S16] C：位操作置位
来源：http://hz.xingfuxueyuan.xyz/gtfkwxkheu.html

x |= (1 << 3);
来源：http://hz.daxiang520.top/gtxdorrajd.html

[S17] C：安全拼接字符串
来源：http://hz.hammf.cn/gtgdxvbicw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.0kj1m.cn/gtegjbttvt.html

[S18] C：命令行参数
来源：http://hz.aibaodan.cn/gtmviryspa.html

int main(int argc, char **argv)
来源：http://hz.dianchejie.cn/gtdzygiwqa.html

[S19] C：快速排序
来源：http://hz.jiagoushi.top/gtggpsipsg.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.vqdsnc.cn/gtleujlhgs.html

[S20] C：二分查找
来源：http://hz.316326.xyz/gtiuzthogj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hysaishi.cn/gtbygchasu.html

[S21] C：字符类别判断
来源：http://hz.xuanzx.com/gtjszxipvd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.aibaodan.cn/gtujcvfzae.html

[S22] C：字符串转数字
来源：http://hz.shuidangran.top/gtsvexmqkq.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jiagoushi.top/gtzvhumvnb.html

[S23] C：随机数
来源：http://hz.jianghu66.top/gtzcpjccsx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.daxiang520.top/gtnwlufixc.html

[S24] C：获取本地时间
来源：http://hz.yangfankeji.com/gtnlkplgkv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.cqqwz.cn/gtpwxgsyrf.html

[S25] C：内存拷贝
来源：http://hz.yj202588.top/gtzncrsbvo.html

memcpy(dst, src, n);
来源：http://hz.meibo888.top/gtcfyyfxwv.html

[S26] C：内存清零
来源：http://hz.ivvv.top/gtpzomutyj.html

memset(a, 0, sizeof a);
来源：http://hz.cashguo.top/gtuompqlbb.html

[S27] C：定义常量
来源：http://hz.zhijiandao.cn/gtydprpwlw.html

const double PI = 3.14159;
来源：http://hz.xuetiantiany.cn/gtlzryndhl.html

[S28] C：静态变量
来源：http://hz.hnqzz.top/gtjfyurjow.html

static int counter = 0;
来源：http://hz.xuanzx.com/gtfbptbkim.html

[S29] C：变参函数
来源：http://hz.zhiwuduotai.top/gtfywkkhgo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ivvv.top/gtgnholsfq.html

[S30] C：头文件保护
来源：http://hz.ywan-chungtsiang.top/gtpugywzez.html

#ifndef X_H
来源：http://hz.jinqigfzy.top/gtgnwhwjsw.html

#define X_H
来源：http://hz.yuxming.cn/gtzleifauk.html

#endif
来源：http://hz.yuxming.cn/gtvddynrzf.html

[S31] C++：Hello World
来源：http://hz.ydzc1.top/gtkhjamimv.html

#include <iostream>
来源：http://hz.cdnleiting.top/gtktzzhulv.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zhengqikj.top/gtraarwgpd.html

[S32] C++：字符串
来源：http://hz.yuanzhike.top/gttltecfwk.html

std::string s = "hi";  s += "!";
来源：http://hz.9152youxi.cn/gtyxgowhpe.html

[S33] C++：vector 增删
来源：http://hz.9152youxi.cn/gtxjimdjgc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yangfankeji.com/gtlylazkxe.html

[S34] C++：遍历 vector
来源：http://hz.dashuyun.cn/gtaxpnjoqf.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.fzhhl.top/gtcekhkhlk.html

[S35] C++：map
来源：http://hz.xuanzx.com/gtpjtmtncp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhongyouzk.top/gtwndslixp.html

[S36] C++：unordered_map
来源：http://hz.jinqigufen.top/gtlocaitwy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.meibo888.top/gtxpwlktkm.html

[S37] C++：set
来源：http://hz.sweek.top/gtorjkivrs.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ybcxt.top/gtxjfrjhfa.html

[S38] C++：排序
来源：http://hz.chenzaomai.com/gtesqjhlai.html

std::sort(v.begin(), v.end());
来源：http://hz.ehwqpu.com/gtqjhumwsr.html

[S39] C++：自定义比较器排序
来源：http://hz.aibaodan.cn/gtbtuzedxj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ybcxt.top/gtirnngryd.html

[S40] C++：查找元素
来源：http://hz.zhongyouzk.top/gtwiccvllr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.fengsongda.top/gtqufueqfi.html

[S41] C++：类与构造函数
来源：http://hz.yuxming.cn/gtvvsqahbt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.chenlongwang.top/gtxxrybtpw.html

[S42] C++：继承与虚函数
来源：http://hz.yj20258.top/gtosdtduct.html

class B : public Base { public: void f() override {} };
来源：http://hz.hammf.cn/gtedxlduco.html

[S43] C++：智能指针
来源：http://hz.yanxiufei.cn/gtloahqtef.html

auto p = std::make_unique<int>(5);
来源：http://hz.sufxvd.cn/gtgnbhstms.html

[S44] C++：引用传参
来源：http://hz.havefunace.top/gtvvtfuqgt.html

void inc(int &x) { ++x; }
来源：http://hz.kuanghao11.cn/gtckxhvejo.html

[S45] C++：lambda
来源：http://hz.xuetiantiany.cn/gttfhwamvs.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.0kj1m.cn/gtkdfducvx.html

[S46] C++：函数模板
来源：http://hz.jyoumei.cn/gtkcdlovpj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.52xcode.cn/gthefgofta.html

[S47] C++：结构化绑定遍历
来源：http://hz.hfpthk.cn/gtjuelldmp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.haohaochexian.top/gtvwdrtfch.html

[S48] C++：逐行读文件
来源：http://hz.jlsjyb.cn/gtiylycpmg.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yongpay.top/gtvxrqjyic.html

while (std::getline(in, line)) { }
来源：http://hz.aizwys.cn/gtvnvptjeh.html

[S49] C++：写文件
来源：http://hz.guannengcc.top/gtveizgmwy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.gogol.net.cn/gtkjfpcpqa.html

[S50] C++：格式化数字
来源：http://hz.316326.xyz/gtphrvxsja.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hnxiangtu.top/gtdhavqoyv.html

[S51] C++：显式类型转换
来源：http://hz.redwolf501.top/gtzmiehgyd.html

static_cast<double>(a) / b
来源：http://hz.yj20258.top/gtsazvolzg.html

[S52] C++：const 与 noexcept
来源：http://hz.vqdsnc.cn/gtcshwmgbu.html

int size() const noexcept { return n_; }
来源：http://hz.316326.xyz/gtgehjpuys.html

[S53] C++：移动语义
来源：http://hz.zhengqikj.top/gtvbxwlmfp.html

std::vector<int> w = std::move(v);
来源：http://hz.chenzaomai.com/gtdofbnnbq.html

[S54] C++：异常处理
来源：http://hz.jinghuilouyu.cn/gtgqbrcity.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.snrcjt.cn/gtxncgyhgf.html

[S55] C++：结构化绑定
来源：http://hz.yuxming.cn/gttevtofye.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yongpay.top/gtmnamspik.html

[S56] C++：optional
来源：http://hz.chenjidiqi.icu/gtbipmrsjn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.ydzc1.top/gtwucyjqpr.html

[S57] C++：编译期常量
来源：http://hz.haohaochexian.top/gtdxktgwjp.html

constexpr int N = 10;
来源：http://hz.hysaishi.cn/gtjzyqwyzj.html

[S58] C++：命名空间
来源：http://hz.0kj1m.cn/gtxbojnsxo.html

namespace ns { int f() { return 1; } }
来源：http://hz.zhengqikj.top/gtofkcerde.html

[S59] C++：静态断言
来源：http://hz.guannengcc.top/gtekrmakuz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jqgufenzy.top/gtcuubzaqb.html

[S60] C++：遍历并删除元素
来源：http://hz.xuanzx.com/gtjjrpyrzi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.52xcode.cn/gtgsfbrroo.html

================================================================================
来源：http://hz.kuanghao11.cn/gtkmdbtpvb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xylfe.cn/gtqhtwgpbb.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtxnbvlcuk.html

[T01] Kotlin：Hello World
来源：http://hz.zhongyouzk.top/gtrehbfvef.html

println("Hello")
来源：http://hz.redwolf501.top/gtcdnhdjap.html

[T02] Kotlin：变量
来源：http://hz.quarkkingdee.top/gtedulfghw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.gaohongyu789.top/gtjxhsyueo.html

[T03] Kotlin：字符串模板
来源：http://hz.hammf.cn/gtscyfmigy.html

"值: $b"
来源：http://hz.svipenyu.cn/gtmodxkror.html

[T04] Kotlin：空安全
来源：http://hz.redwolf501.top/gtmpvzthkh.html

val n: String? = null;  n?.length
来源：http://hz.jqgfzy.top/gtqxgtlbrf.html

[T05] Kotlin：when 表达式
来源：http://hz.pycfn.com/gtfijpdomj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.bjfxy.top/gtcufgzgpm.html

[T06] Kotlin：集合映射
来源：http://hz.guowangkeji.top/gtfobkadgx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.vqdsnc.cn/gtfqhmirrk.html

[T07] Kotlin：集合过滤
来源：http://hz.tanke756.top/gtnzfjtxhc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hywenlv.cn/gtjcsvfytu.html

[T08] Kotlin：数据类
来源：http://hz.52xcode.cn/gteyfkbwiu.html

data class User(val name: String, val age: Int)
来源：http://hz.yongpay.top/gtlgtpjjhv.html

[T09] Kotlin：扩展函数
来源：http://hz.smart0.xyz/gtlileqnof.html

fun String.exclaim() = this + "!"
来源：http://hz.dashuyun.cn/gtkimllplf.html

[T10] Kotlin：默认参数
来源：http://hz.daxiang520.top/gtpzgpdbau.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ywan-chungtsiang.top/gtuvugjtyc.html

[T11] Kotlin：协程
来源：http://hz.jinqigufen.top/gtnuprtrio.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.hnxiangtu.top/gtnfdaigdi.html

[T12] Kotlin：解构声明
来源：http://hz.yongpay.top/gtujgasbhq.html

val (a, b) = Pair(1, 2)
来源：http://hz.tanke756.top/gtakqulmvh.html

[T13] Kotlin：只读 Map
来源：http://hz.zycfv.cn/gtjpjutzhh.html

val m = mapOf("a" to 1)
来源：http://hz.guannengcc.top/gtojsrmlko.html

[T14] Kotlin：循环
来源：http://hz.ydjk.org.cn/gtfcictqdu.html

for (i in 1..10) println(i)
来源：http://hz.ehwqpu.com/gtosbkiflo.html

[T15] Kotlin：接口
来源：http://hz.tianlin.xyz/gtoiwduuoo.html

interface Shape { fun area(): Double }
来源：http://hz.jinyuanbaomall.cn/gtfgnluuio.html

[T16] Swift：Hello World
来源：http://hz.yj20258.top/gtiurwbbow.html

print("Hello")
来源：http://hz.shanyushiyangtech.top/gtjydsequd.html

[T17] Swift：变量与常量
来源：http://hz.pengpengdd.cyou/gthhfcijjh.html

var a = 1;  let b = 2
来源：http://hz.zhengqikj.top/gtzymhsoup.html

[T18] Swift：字符串插值
来源：http://hz.sysykeji.top/gtytwnobtl.html

"值: \(b)"
来源：http://hz.iojbl.cn/gtcpohtsvu.html

[T19] Swift：可选绑定
来源：http://hz.snrcjt.cn/gtnjjghhwi.html

if let n = opt { print(n) }
来源：http://hz.snrcjt.cn/gtybmqwiul.html

[T20] Swift：数组操作
来源：http://hz.pycfn.com/gtkkcjahmh.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jinqigfzy.top/gtckkthnha.html

[T21] Swift：遍历
来源：http://hz.zhiwuduotai.top/gtqcvvcszp.html

for x in a { print(x) }
来源：http://hz.zhiwuduotai.top/gtmwqibcae.html

[T22] Swift：字典
来源：http://hz.shanyushiyangtech.top/gtmsobbxcl.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zhongyouzk.top/gtztyvyoyw.html

[T23] Swift：函数
来源：http://hz.shuidangran.top/gtnskzklvk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.0kj1m.cn/gtwoeykhgi.html

[T24] Swift：闭包
来源：http://hz.hfpthk.cn/gtmledxpam.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.ivvv.top/gtvnwvcjui.html

[T25] Swift：结构体
来源：http://hz.hnxiangtu.top/gtxrczaimu.html

struct P { var x: Int }
来源：http://hz.quarkkingdee.top/gtgqdqmqxq.html

[T26] Swift：类与重写
来源：http://hz.zhixingplan.top/gttgvxqxrh.html

class A: Base { override func f() {} }
来源：http://hz.sufxvd.cn/gtgrhoiwki.html

[T27] Swift：错误处理
来源：http://hz.sufxvd.cn/gtwfarzrma.html

do { try f() } catch { print(error) }
来源：http://hz.yvedp.cn/gtqqbnwnaw.html

[T28] Swift：枚举
来源：http://hz.tianlin.xyz/gtqqhqkoqi.html

enum Color { case red, green }
来源：http://hz.aizwys.cn/gtwmoyzsbe.html

[T29] Swift：guard 提前返回
来源：http://hz.jqgufenzy.top/gtnqollywc.html

guard let x = opt else { return }
来源：http://hz.jyoumei.cn/gtxjznqqnx.html

[T30] Swift：协议
来源：http://hz.nwbrower.top/gtycaazusx.html

protocol Shape { func area() -> Double }
来源：http://hz.yanxiufei.cn/gtncfwqoyc.html

[T31] Lua：Hello World
来源：http://hz.wangdashe.top/gtoduxrfke.html

print("Hello")
来源：http://hz.birdmap.top/gtcbenqdmx.html

[T32] Lua：局部变量
来源：http://hz.cqqwz.cn/gtklnofhwh.html

local a = 1
来源：http://hz.shanyushiyangkeji.top/gtfbgdpbmr.html

[T33] Lua：表（数组）
来源：http://hz.cashguo.top/gtlnhydjvk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yangfankeji.com/gtstfacgkz.html

[T34] Lua：遍历表
来源：http://hz.zhiwuduotai.top/gtyiprmofj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.chenlongwang.top/gtqnutxfgo.html

[T35] Lua：字典表
来源：http://hz.pycfn.com/gtaiuuigvf.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yvedp.cn/gtmzuxyeix.html

[T36] Lua：函数
来源：http://hz.haohaochexian.top/gtfnchhnjw.html

function add(a, b) return a + b end
来源：http://hz.jqgfzy.top/gtsnkqoslr.html

[T37] Lua：字符串拼接
来源：http://hz.zhijiandao.cn/gtounmmcam.html

"a" .. "b"
来源：http://hz.ywan-chungtsiang.top/gtgelroibs.html

[T38] Lua：条件
来源：http://hz.smart0.xyz/gtfsyhyoqf.html

if x > 0 then print("正") end
来源：http://hz.gzhubu.top/gtqvbzezxe.html

[T39] Lua：模式匹配
来源：http://hz.quarkkingdee.top/gtorzvwmqn.html

string.find(s, "%d+")
来源：http://hz.snrcjt.cn/gtrgpjdnqv.html

[T40] Lua：元表
来源：http://hz.vqdsnc.cn/gtbssfznlw.html

setmetatable({}, { __index = base })
来源：http://hz.quarkkingdee.top/gtatccsrog.html

[T41] Perl：Hello World
来源：http://hz.xingfuxueyuan.xyz/gtaydmptsi.html

print "Hello\n";
来源：http://hz.sweek.top/gtzovxuqcl.html

[T42] Perl：变量类型
来源：http://hz.hysaishi.cn/gtzbkgquyk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.havefunace.top/gtesnmgdol.html

[T43] Perl：字符串插值
来源：http://hz.shangyingyoupin.top/gtcszdxxnb.html

"值: $a"
来源：http://hz.yj20258888.top/gtkrwkafju.html

[T44] Perl：条件
来源：http://hz.jlsjyb.cn/gtievjbxcx.html

if ($a > 0) { print "正"; }
来源：http://hz.zhiwuduotai.top/gtlcdaryns.html

[T45] Perl：数组遍历
来源：http://hz.yj202588.top/gtzevssgoi.html

for my $x (@arr) { print $x; }
来源：http://hz.iojbl.cn/gtnwnnrtzc.html

[T46] Perl：哈希操作
来源：http://hz.ybcxt.top/gtvrwyfuas.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.haohaochexian.top/gtadsjfubz.html

[T47] Perl：正则捕获
来源：http://hz.chenzaomai.com/gtswfasmbm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.kuanghao11.cn/gtkadwywsj.html

[T48] Perl：正则替换
来源：http://hz.zdqjudy.top/gtqwcfvexb.html

$s =~ s/old/new/g;
来源：http://hz.yanxiufei.cn/gtnfpgxovl.html

[T49] Perl：函数
来源：http://hz.guowangkeji.top/gtvbmywunu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.nanxuanxn.top/gtangzynkl.html

[T50] Perl：逐行读文件
来源：http://hz.chenzaomai.com/gtdghakhrl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.nanxuanxn.top/gtdvpazefu.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.daxiang520.top/gtqancsiug.html

[T51] Scala：Hello World
来源：http://hz.guannengcc.top/gtrydoflqs.html

println("Hello")
来源：http://hz.haohaochexian.top/gtcuxmpajp.html

[T52] Scala：变量
来源：http://hz.shanyushiyangkeji.top/gtwtiotmen.html

val a = 1;  var b = 2
来源：http://hz.shanyushiyangtech.top/gtcpfocign.html

[T53] Scala：字符串插值
来源：http://hz.yj202588.top/gttxdxfpfp.html

s"值: $b"
来源：http://hz.yvedp.cn/gtfawsxxdx.html

[T54] Scala：集合映射
来源：http://hz.fengsongda.top/gtqhjaasur.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.fzhhl.top/gtiylifvkg.html

[T55] Scala：集合过滤
来源：http://hz.316326.xyz/gttsgklivo.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.52xcode.cn/gtbabfxmpt.html

[T56] Scala：样例类
来源：http://hz.guannengcc.top/gthogkhycq.html

case class User(name: String, age: Int)
来源：http://hz.zhixingplan.top/gtaaonikpg.html

[T57] Scala：模式匹配
来源：http://hz.shuidangran.top/gtftisucct.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.sxryk.cn/gtucwidkbk.html

[T58] Scala：函数定义
来源：http://hz.smart0.xyz/gtvywpkklx.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.sysykeji.top/gtqlrdyhci.html

[T59] Scala：循环
来源：http://hz.0kj1m.cn/gthyqfjdxj.html

for (i <- 1 to 10) println(i)
来源：http://hz.hysaishi.cn/gtuqwqnbtx.html

[T60] Scala：折叠
来源：http://hz.yj20258888.top/gtoljhykzi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hnqzz.top/gtucakyaia.html

================================================================================
来源：http://hz.yj20258.top/gtcepajspc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.ydzc1.top/gtlvlnyutf.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtypwgoazn.html

[U01] Py：创建虚拟环境
来源：http://hz.yueranfly.top/gtkgascmyo.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.mhx1999.top/gtfljtwrpf.html

[U02] Py：导出 / 安装依赖
来源：http://hz.kuanghao11.cn/gtekeocbjv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.chenjidiqi.icu/gttwyuqupa.html

[U03] Py：加载 .env 配置
来源：http://hz.tian-w.cn/gtzqhzajjh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.xinyue.icu/gtpmzctaxm.html

[U04] Py：变量调试打印
来源：http://hz.haohaochexian.top/gthgjtzzen.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.sweek.top/gtvmcpxahj.html

[U05] Py：列表去重且保序
来源：http://hz.snrcjt.cn/gtusgrbedr.html

list(dict.fromkeys(arr))
来源：http://hz.hnxiangtu.top/gtzpkatjna.html

[U06] Py：合并两个字典
来源：http://hz.aizwys.cn/gtommqquxf.html

{**a, **b}
来源：http://hz.yonumen.top/gtevbisjmp.html

[U07] Py：反转字典键值
来源：http://hz.zhaomingkeji.xyz/gtectvzgsc.html

{v: k for k, v in d.items()}
来源：http://hz.yonumen.top/gtxhjvslfu.html

[U08] Py：展平二维列表
来源：http://hz.jyoumei.cn/gtmqyxyokx.html

[y for x in nested for y in x]
来源：http://hz.jqgufenzy.top/gtbuzxhjmo.html

[U09] Py：字典取最大值的键
来源：http://hz.zhijiandao.cn/gtsbvyfrqr.html

max(d, key=d.get)
来源：http://hz.havefunace.top/gtmxenrahn.html

[U10] Py：按值排序字典
来源：http://hz.daria6918.cn/gtlmlnwmvr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.jinyuanbaomall.cn/gtkjzvuiso.html

[U11] Py：生成器表达式
来源：http://hz.yanxiufei.cn/gtxhlrinmx.html

(x * 2 for x in arr)
来源：http://hz.cdnleiting.top/gtmejzfgau.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.hfpthk.cn/gtpjtghjye.html

Counter(arr).most_common(3)
来源：http://hz.0kj1m.cn/gtccwfoetq.html

[U13] Py：固定长度队列
来源：http://hz.chenzaomai.com/gtpqktjawl.html

deque(maxlen=10)
来源：http://hz.9152youxi.cn/gthauklbvt.html

[U14] Py：分组收集到列表
来源：http://hz.havefunace.top/gtlbraudkj.html

defaultdict(list)
来源：http://hz.gzhubu.top/gthpszoqal.html

[U15] Py：高精度计时
来源：http://hz.bjfxy.top/gtukgjhwuy.html

t = time.perf_counter()
来源：http://hz.wangshuangyany.cn/gtedkhdvwo.html

[U16] Py：命令行参数解析
来源：http://hz.sufxvd.cn/gtkrnhllic.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.chenlongwang.top/gtyovgpvty.html

[U17] Py：初始化日志
来源：http://hz.zhaomingkeji.xyz/gtlwgwaqli.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.kuanghao11.cn/gtcmsdtujd.html

[U18] Py：预编译正则
来源：http://hz.xziqi.cn/gtamriznir.html

pat = re.compile(r"\d+")
来源：http://hz.ydzc1.top/gtswjjwxbd.html

[U19] Py：正则替换带回调
来源：http://hz.chenlongwang.top/gtgmnlpvkx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yonumen.top/gtdkwfwnya.html

[U20] Py：缓存函数结果
来源：http://hz.cheryme.top/gtzcyfntgt.html

@functools.lru_cache(maxsize=None)
来源：http://hz.tianlin.xyz/gtcujwnfrt.html

[U21] Py：自定义上下文管理器
来源：http://hz.havefunace.top/gtyecyfcrv.html

@contextlib.contextmanager
来源：http://hz.iojbl.cn/gtnougxbnv.html

[U22] Py：矩阵转置
来源：http://hz.sufxvd.cn/gtwkgbfdug.html

list(zip(*m))
来源：http://hz.hnqzz.top/gtsbdyhnuw.html

[U23] Py：分块读取大文件
来源：http://hz.sweek.top/gtmslqvfiw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yanxiufei.cn/gtitveaxxc.html

[U24] Py：路径操作
来源：http://hz.pycfn.com/gtroavtqss.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.fengsongda.top/gtyjkwuvpn.html

[U25] Py：CSV 按字典读
来源：http://hz.sufxvd.cn/gtbjokovzm.html

csv.DictReader(f)
来源：http://hz.yanxiufei.cn/gtwqhwozal.html

[U26] Py：并发下载
来源：http://hz.vqdsnc.cn/gttnazwpwt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jlsjyb.cn/gtayocdasa.html

[U27] Py：异步 HTTP
来源：http://hz.jinyuanbaomall.cn/gthzjiorry.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.hammf.cn/gtrtzwwewp.html

[U28] Py：类型别名
来源：http://hz.shanyushiyangtech.top/gtfinebdxb.html

UserId = int
来源：http://hz.hywenlv.cn/gtkzehaclv.html


<!-- 参考信息 -->