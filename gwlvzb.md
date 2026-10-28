代发 wailian999

strlen(s)
来源：http://hz.c1oappe.top/gttqtbtgly.html

[S06] C：字符串比较
来源：http://hz.xuetiantiany.cn/gtkzlsmkmo.html

strcmp(a, b) == 0
来源：http://hz.xuetiantiany.cn/gtnnnmgikn.html

[S07] C：数组遍历求和
来源：http://hz.hywenlv.cn/gtudqpnwts.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhoulong.xyz/gtjimgnjca.html

[S08] C：动态内存分配与释放
来源：http://hz.xuanzx.com/gtgqabnpzt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hongshengwenyu.top/gtbhabeiyt.html

[S09] C：结构体定义与初始化
来源：http://hz.vqdsnc.cn/gtziapfiza.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.tian-w.cn/gtdruisjvo.html

[S10] C：指针与解引用
来源：http://hz.hammf.cn/gtfgizjaon.html

int *p = &a;  *p = 5;
来源：http://hz.yj202588.top/gtyshpnrce.html

[S11] C：逐行读文件
来源：http://hz.yuanzhike.top/gtmhogtfck.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.c1oappe.top/gtdqqqzfxs.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.pycfn.com/gtvnrntnvi.html

fclose(f);
来源：http://hz.ydzc1.top/gtfrawupqi.html

[S12] C：写文件
来源：http://hz.zdqjudy.top/gtaqrmssfj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.dashuyun.cn/gtenlvuqrc.html

[S13] C：宏定义
来源：http://hz.guannengcc.top/gtsyldcibn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.cqqwz.cn/gtkbfpgtio.html

[S14] C：枚举
来源：http://hz.xinyue.icu/gtzujsktum.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.dianchejie.cn/gtnoqlgzsf.html

[S15] C：类型转换
来源：http://hz.zhixingplan.top/gthsxsgrah.html

(double) a / b
来源：http://hz.gaohongyu789.top/gtrnxfpsmz.html

[S16] C：位操作置位
来源：http://hz.feifeiyinyue.top/gtunbuqovj.html

x |= (1 << 3);
来源：http://hz.nanxuanxn.top/gtvwdqexuh.html

[S17] C：安全拼接字符串
来源：http://hz.zhiwuduotai.top/gtwksrqnzp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xuetiantiany.cn/gtnjsijmrb.html

[S18] C：命令行参数
来源：http://hz.zycfv.cn/gtloreikfc.html

int main(int argc, char **argv)
来源：http://hz.zhijiandao.cn/gtdjajuvwx.html

[S19] C：快速排序
来源：http://hz.bjfxy.top/gtbisplqet.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.xuanzx.com/gtjgytwuta.html

[S20] C：二分查找
来源：http://hz.ehwqpu.com/gtfsxlqybr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.fzhhl.top/gtagppbhto.html

[S21] C：字符类别判断
来源：http://hz.quarkkingdee.top/gtbvzzrsuk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.9152youxi.cn/gtkcdzblws.html

[S22] C：字符串转数字
来源：http://hz.ydzc1.top/gtbvwiszgt.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.svipenyu.cn/gtkdmwgsul.html

[S23] C：随机数
来源：http://hz.yangfankeji.com/gttuxygnam.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.cheryme.top/gtoxivzegs.html

[S24] C：获取本地时间
来源：http://hz.yuanzhike.top/gtjyhoiqkx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ywan-chungtsiang.top/gttctfmtvs.html

[S25] C：内存拷贝
来源：http://hz.yongpay.top/gtlkjepmxv.html

memcpy(dst, src, n);
来源：http://hz.aizwys.cn/gtevmjhutp.html

[S26] C：内存清零
来源：http://hz.jinyuanbaomall.cn/gtrvqsctdx.html

memset(a, 0, sizeof a);
来源：http://hz.sufxvd.cn/gtqrnuzvea.html

[S27] C：定义常量
来源：http://hz.wangdashe.top/gtjahyeain.html

const double PI = 3.14159;
来源：http://hz.ppjwa.cn/gtzfjnqnxm.html

[S28] C：静态变量
来源：http://hz.316326.xyz/gtfcrclpgy.html

static int counter = 0;
来源：http://hz.zhoulong.xyz/gtwpwvtfbc.html

[S29] C：变参函数
来源：http://hz.cdnleiting.top/gtjjlggqpl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jinqigfzy.top/gtwsgqxbxj.html

[S30] C：头文件保护
来源：http://hz.nanxuanxn.top/gteptwdtqg.html

#ifndef X_H
来源：http://hz.sysykeji.top/gtaswcsjba.html

#define X_H
来源：http://hz.zhoulong.xyz/gtwjoycanf.html

#endif
来源：http://hz.guannengcc.top/gtyrvcljvr.html

[S31] C++：Hello World
来源：http://hz.daxiang520.top/gtkbqykpff.html

#include <iostream>
来源：http://hz.gzhubu.top/gthfzjwnol.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.cucudq.cn/gtptroigkp.html

[S32] C++：字符串
来源：http://hz.52xcode.cn/gtjkcmzkaw.html

std::string s = "hi";  s += "!";
来源：http://hz.zdqjudy.top/gtktdgzjgs.html

[S33] C++：vector 增删
来源：http://hz.yuanzhike.top/gtquvqancc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.dianchejie.cn/gtqndbtdla.html

[S34] C++：遍历 vector
来源：http://hz.cqqwz.cn/gthizbiazb.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yuxming.cn/gtwfopuegj.html

[S35] C++：map
来源：http://hz.sufxvd.cn/gtrkylrptn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jlsjyb.cn/gtfksrytgi.html

[S36] C++：unordered_map
来源：http://hz.ybcxt.top/gttffnjbmr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj202588.top/gtgyzejhrh.html

[S37] C++：set
来源：http://hz.hongshengwenyu.top/gtmfzfwkmz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xylfe.cn/gtxkxvjthl.html

[S38] C++：排序
来源：http://hz.dashuyun.cn/gttyqxltja.html

std::sort(v.begin(), v.end());
来源：http://hz.316326.xyz/gtdwcouyde.html

[S39] C++：自定义比较器排序
来源：http://hz.hongshengwenyu.top/gtdshtjatx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.fzhhl.top/gtqaluryer.html

[S40] C++：查找元素
来源：http://hz.gzhubu.top/gtwangenhn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.quarkkingdee.top/gthmnendxb.html

[S41] C++：类与构造函数
来源：http://hz.dashuyun.cn/gtskotymdc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.wangdashe.top/gtmgpvfcbv.html

[S42] C++：继承与虚函数
来源：http://hz.ivvv.top/gthdjvxzmi.html

class B : public Base { public: void f() override {} };
来源：http://hz.daxiang520.top/gtfumvgeky.html

[S43] C++：智能指针
来源：http://hz.chenjidiqi.icu/gtwhcpiqui.html

auto p = std::make_unique<int>(5);
来源：http://hz.hysaishi.cn/gtcdoxogsb.html

[S44] C++：引用传参
来源：http://hz.svipenyu.cn/gtjknrumle.html

void inc(int &x) { ++x; }
来源：http://hz.zhixingplan.top/gtpqhkfbps.html

[S45] C++：lambda
来源：http://hz.hywenlv.cn/gtetlyylpi.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.shuidangran.top/gtarrphgtz.html

[S46] C++：函数模板
来源：http://hz.jinqigfzy.top/gtbhugmrxd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.feifeiyinyue.top/gtuxxgykri.html

[S47] C++：结构化绑定遍历
来源：http://hz.jqgfzy.top/gtcxszhryh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.aizwys.cn/gtqportjhp.html

[S48] C++：逐行读文件
来源：http://hz.smart0.xyz/gtsreeuwym.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.wangshuangyany.cn/gtesuqveqj.html

while (std::getline(in, line)) { }
来源：http://hz.jianghu66.top/gthjmyefqj.html

[S49] C++：写文件
来源：http://hz.ywan-chungtsiang.top/gthttwqhhr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.shanyushiyangkeji.top/gtqzvawlts.html

[S50] C++：格式化数字
来源：http://hz.fzhhl.top/gtifxfkifp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yongpay.top/gtaugplnnw.html

[S51] C++：显式类型转换
来源：http://hz.yj202588.top/gteorslfal.html

static_cast<double>(a) / b
来源：http://hz.yonumen.top/gtwmyznbpv.html

[S52] C++：const 与 noexcept
来源：http://hz.shzxlz.cn/gtprdjeffu.html

int size() const noexcept { return n_; }
来源：http://hz.cheryme.top/gtcjmypdgi.html

[S53] C++：移动语义
来源：http://hz.bjfxy.top/gtxcrkvxgz.html

std::vector<int> w = std::move(v);
来源：http://hz.shanyushiyangkeji.top/gtebhrlxbx.html

[S54] C++：异常处理
来源：http://hz.smart0.xyz/gtpqgjobpd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.nwbrower.top/gtvjnuydhb.html

[S55] C++：结构化绑定
来源：http://hz.shzxlz.cn/gtkuquhnzd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.haohaochexian.top/gtqnycxjba.html

[S56] C++：optional
来源：http://hz.jlsjyb.cn/gtrihcexgc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.shangyingyoupin.top/gtlpnolhzl.html

[S57] C++：编译期常量
来源：http://hz.hywenlv.cn/gtucwqphsf.html

constexpr int N = 10;
来源：http://hz.ivvv.top/gtyyucnoqf.html

[S58] C++：命名空间
来源：http://hz.shuidangran.top/gtjftavecf.html

namespace ns { int f() { return 1; } }
来源：http://hz.gogol.net.cn/gtcpcmurxb.html

[S59] C++：静态断言
来源：http://hz.jianghu66.top/gtkierikyu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.pengpengdd.cyou/gtmwacodrn.html

[S60] C++：遍历并删除元素
来源：http://hz.zhoulong.xyz/gtthnoacqi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.smart0.xyz/gtfijqxqyy.html

================================================================================
来源：http://hz.ydjk.org.cn/gtcgleyuib.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhixingplan.top/gtvswakxyi.html

================================================================================
来源：http://hz.yanxiufei.cn/gtgtwlstqc.html

[T01] Kotlin：Hello World
来源：http://hz.quarkkingdee.top/gtltvjsxsi.html

println("Hello")
来源：http://hz.pycfn.com/gtopyiymuq.html

[T02] Kotlin：变量
来源：http://hz.pengpengdd.cyou/gtujfzryub.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yj202588.top/gtpdbyggwz.html

[T03] Kotlin：字符串模板
来源：http://hz.aibaodan.cn/gtysbecxnu.html

"值: $b"
来源：http://hz.sysykeji.top/gtxgkngmdo.html

[T04] Kotlin：空安全
来源：http://hz.zhaomingkeji.xyz/gthnsyxsnx.html

val n: String? = null;  n?.length
来源：http://hz.zhaomingkeji.xyz/gteknmqhtj.html

[T05] Kotlin：when 表达式
来源：http://hz.tian-w.cn/gtallwluax.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.aizwys.cn/gtmffxkzzj.html

[T06] Kotlin：集合映射
来源：http://hz.tanke756.top/gtbaufmvma.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yj20258.top/gtabhkgiow.html

[T07] Kotlin：集合过滤
来源：http://hz.yanxiufei.cn/gtipafjfwv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jinqigufen.top/gthyzfpbof.html

[T08] Kotlin：数据类
来源：http://hz.yj20258888.top/gtdutehaqo.html

data class User(val name: String, val age: Int)
来源：http://hz.zhaomingkeji.xyz/gtcxetkbbj.html

[T09] Kotlin：扩展函数
来源：http://hz.cdnleiting.top/gtctgrozfh.html

fun String.exclaim() = this + "!"
来源：http://hz.yj20258.top/gtqgkzbvgz.html

[T10] Kotlin：默认参数
来源：http://hz.yvedp.cn/gtvrmpcbrb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zhengqikj.top/gtcwdbbuqo.html

[T11] Kotlin：协程
来源：http://hz.jianghu66.top/gtczcnupsi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.kuanghao11.cn/gtjzlvvzma.html

[T12] Kotlin：解构声明
来源：http://hz.zhixingplan.top/gtitsnoaby.html

val (a, b) = Pair(1, 2)
来源：http://hz.sysykeji.top/gtyljylzjw.html

[T13] Kotlin：只读 Map
来源：http://hz.daxiang520.top/gtdihlzits.html

val m = mapOf("a" to 1)
来源：http://hz.yj202588.top/gtqxpccskt.html

[T14] Kotlin：循环
来源：http://hz.vqdsnc.cn/gtksxxavhd.html

for (i in 1..10) println(i)
来源：http://hz.hnqzz.top/gtcxklmwvp.html

[T15] Kotlin：接口
来源：http://hz.meibo888.top/gtzvopcwov.html

interface Shape { fun area(): Double }
来源：http://hz.chenlongwang.top/gtwohwashp.html

[T16] Swift：Hello World
来源：http://hz.dashuyun.cn/gttubelufp.html

print("Hello")
来源：http://hz.cheryme.top/gttwhmzfme.html

[T17] Swift：变量与常量
来源：http://hz.dianchejie.cn/gtcmoexgte.html

var a = 1;  let b = 2
来源：http://hz.wangdashe.top/gtdfcldbvl.html

[T18] Swift：字符串插值
来源：http://hz.hammf.cn/gtfxcfkkyi.html

"值: \(b)"
来源：http://hz.tian-w.cn/gtqfkrrfnq.html

[T19] Swift：可选绑定
来源：http://hz.jinghuilouyu.cn/gteblevzbr.html

if let n = opt { print(n) }
来源：http://hz.jinghuilouyu.cn/gtvposhnty.html

[T20] Swift：数组操作
来源：http://hz.52xcode.cn/gtdtygmysd.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.feifeiyinyue.top/gtosknulek.html

[T21] Swift：遍历
来源：http://hz.xuetiantiany.cn/gtmubocqdt.html

for x in a { print(x) }
来源：http://hz.yuxming.cn/gtppvjtsyc.html

[T22] Swift：字典
来源：http://hz.kuanghao11.cn/gtmexwatht.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.dashuyun.cn/gtwtpfpgfq.html

[T23] Swift：函数
来源：http://hz.shangyingyoupin.top/gtqcbbdloj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.gogol.net.cn/gtpdbstdrf.html

[T24] Swift：闭包
来源：http://hz.fzhhl.top/gtqubwwkyc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.0kj1m.cn/gtsydrkmyx.html

[T25] Swift：结构体
来源：http://hz.tianlin.xyz/gteigotqcu.html

struct P { var x: Int }
来源：http://hz.zhiwuduotai.top/gtpgwsvtpj.html

[T26] Swift：类与重写
来源：http://hz.sufxvd.cn/gtzroyuunh.html

class A: Base { override func f() {} }
来源：http://hz.hongshengwenyu.top/gtmaevwzss.html

[T27] Swift：错误处理
来源：http://hz.andypj.xyz/gtubvfzynq.html

do { try f() } catch { print(error) }
来源：http://hz.ywan-chungtsiang.top/gtbtlmumzl.html

[T28] Swift：枚举
来源：http://hz.zhaomingkeji.xyz/gtjjamrviu.html

enum Color { case red, green }
来源：http://hz.xziqi.cn/gtnnnvzgka.html

[T29] Swift：guard 提前返回
来源：http://hz.yuanzhike.top/gtpdxmruwq.html

guard let x = opt else { return }
来源：http://hz.hnxiangtu.top/gtcubclryx.html

[T30] Swift：协议
来源：http://hz.xinyue.icu/gtyfajsbyv.html

protocol Shape { func area() -> Double }
来源：http://hz.redwolf501.top/gtypygkujc.html

[T31] Lua：Hello World
来源：http://hz.zycfv.cn/gttrogjsbx.html

print("Hello")
来源：http://hz.wangdashe.top/gtusibptpo.html

[T32] Lua：局部变量
来源：http://hz.feifeiyinyue.top/gtbhywwhzf.html

local a = 1
来源：http://hz.zhengqikj.top/gtyvnorhek.html

[T33] Lua：表（数组）
来源：http://hz.nanxinkj.top/gtonmwavts.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jinqigufen.top/gtiyvqjfrv.html

[T34] Lua：遍历表
来源：http://hz.hywenlv.cn/gtvwgkdxzc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jinyuanbaomall.cn/gtzizettye.html

[T35] Lua：字典表
来源：http://hz.ywan-chungtsiang.top/gtxkwqisuw.html

local d = { a = 1 };  d.b = 2
来源：http://hz.hnqzz.top/gtcusiygdd.html

[T36] Lua：函数
来源：http://hz.dianchejie.cn/gtddpamshh.html

function add(a, b) return a + b end
来源：http://hz.jqgfzy.top/gthxgfpfpu.html

[T37] Lua：字符串拼接
来源：http://hz.dashuyun.cn/gttunqyath.html

"a" .. "b"
来源：http://hz.cdnleiting.top/gtllhsphwn.html

[T38] Lua：条件
来源：http://hz.yonumen.top/gtkhxzrtbm.html

if x > 0 then print("正") end
来源：http://hz.nwbrower.top/gttmylhhyk.html

[T39] Lua：模式匹配
来源：http://hz.yanxiufei.cn/gtnagdolpx.html

string.find(s, "%d+")
来源：http://hz.gotoacloud.top/gtqxvuroge.html

[T40] Lua：元表
来源：http://hz.316326.xyz/gtrhoycten.html

setmetatable({}, { __index = base })
来源：http://hz.bjfxy.top/gtbinyeplu.html

[T41] Perl：Hello World
来源：http://hz.yangfankeji.com/gtzsmtcwnp.html

print "Hello\n";
来源：http://hz.sxryk.cn/gtdgtvzgpy.html

[T42] Perl：变量类型
来源：http://hz.wangshuangyany.cn/gtmisdcccn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.xingfuxueyuan.xyz/gtflynyzqn.html

[T43] Perl：字符串插值
来源：http://hz.sxryk.cn/gtmmmlorij.html

"值: $a"
来源：http://hz.shanyushiyangkeji.top/gtbawuogue.html

[T44] Perl：条件
来源：http://hz.hysaishi.cn/gtatbspyyx.html

if ($a > 0) { print "正"; }
来源：http://hz.shanyushiyangtech.top/gtcnbujoyb.html

[T45] Perl：数组遍历
来源：http://hz.daria6918.cn/gtxkqubvsl.html

for my $x (@arr) { print $x; }
来源：http://hz.shangyingyoupin.top/gtwtacjpka.html

[T46] Perl：哈希操作
来源：http://hz.zycfv.cn/gtprvlqkbn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.wangshuangyany.cn/gtgfioiimh.html

[T47] Perl：正则捕获
来源：http://hz.yueranfly.top/gtnuifmzou.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yvedp.cn/gtrzlcteig.html

[T48] Perl：正则替换
来源：http://hz.cdnleiting.top/gtxiylztan.html

$s =~ s/old/new/g;
来源：http://hz.sysykeji.top/gtkjbbyjle.html

[T49] Perl：函数
来源：http://hz.ybcxt.top/gtbgdecevr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.guannengcc.top/gtjtbrchhs.html

[T50] Perl：逐行读文件
来源：http://hz.yangfankeji.com/gtsetlybfc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.wangdashe.top/gtqyrxlroc.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.shzxlz.cn/gtwjyypdyo.html

[T51] Scala：Hello World
来源：http://hz.pengpengdd.cyou/gtlpgllmjo.html

println("Hello")
来源：http://hz.nanxinkj.top/gtsolwudcg.html

[T52] Scala：变量
来源：http://hz.fengsongda.top/gtwoopgqsz.html

val a = 1;  var b = 2
来源：http://hz.ydzc1.top/gtjufarphv.html

[T53] Scala：字符串插值
来源：http://hz.xinyue.icu/gttctakmtk.html

s"值: $b"
来源：http://hz.sweek.top/gtpwwgvvrc.html

[T54] Scala：集合映射
来源：http://hz.hfpthk.cn/gtjtsrveas.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.9152youxi.cn/gtqummopgg.html

[T55] Scala：集合过滤
来源：http://hz.daxiang520.top/gtqszcxtfq.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.316326.xyz/gtdrusqhmr.html

[T56] Scala：样例类
来源：http://hz.9152youxi.cn/gtmhbojqge.html

case class User(name: String, age: Int)
来源：http://hz.jinqigfzy.top/gtcfuxrtld.html

[T57] Scala：模式匹配
来源：http://hz.hysaishi.cn/gtzuifmcfh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.svipenyu.cn/gtwanswggc.html

[T58] Scala：函数定义
来源：http://hz.gzhubu.top/gthualshnn.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.shanyushiyangkeji.top/gtsprpcvqv.html

[T59] Scala：循环
来源：http://hz.ydjk.org.cn/gtkzfkdzka.html

for (i <- 1 to 10) println(i)
来源：http://hz.tianlin.xyz/gtkmmlgyam.html

[T60] Scala：折叠
来源：http://hz.jqgufenzy.top/gttqaccxqp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.ydzc1.top/gtoaiyvkug.html

================================================================================
来源：http://hz.quarkkingdee.top/gtrvungrfv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.hnqzz.top/gtmzokyjwd.html

================================================================================
来源：http://hz.ehwqpu.com/gtxfevihxv.html

[U01] Py：创建虚拟环境
来源：http://hz.pengpengdd.cyou/gtwvehqiyn.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.cdnleiting.top/gtghvglzow.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jlsjyb.cn/gtazdzdadi.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yongpay.top/gtybscnuoe.html

[U03] Py：加载 .env 配置
来源：http://hz.meibo888.top/gtmlojpsww.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.hongshengwenyu.top/gtoykbdnxc.html

[U04] Py：变量调试打印
来源：http://hz.zhijiandao.cn/gtfuxtjakr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.pengpengdd.cyou/gtgmhlgwer.html

[U05] Py：列表去重且保序
来源：http://hz.jyoumei.cn/gtmahobxmp.html

list(dict.fromkeys(arr))
来源：http://hz.xinyue.icu/gtnwkpwpes.html

[U06] Py：合并两个字典
来源：http://hz.zycfv.cn/gtypvpvran.html

{**a, **b}
来源：http://hz.fengsongda.top/gttdkagqlu.html

[U07] Py：反转字典键值
来源：http://hz.zhongyouzk.top/gtrqgljfzj.html

{v: k for k, v in d.items()}
来源：http://hz.yj202588.top/gtonfrqddg.html

[U08] Py：展平二维列表
来源：http://hz.jinghuilouyu.cn/gtxiygttvp.html

[y for x in nested for y in x]
来源：http://hz.hammf.cn/gtxbjwizhn.html

[U09] Py：字典取最大值的键
来源：http://hz.haohaochexian.top/gtsngoauzr.html

max(d, key=d.get)
来源：http://hz.vqdsnc.cn/gtkrximtpm.html

[U10] Py：按值排序字典
来源：http://hz.hysaishi.cn/gtlndybhqm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.cashguo.top/gtlubglprf.html

[U11] Py：生成器表达式
来源：http://hz.birdmap.top/gtdapgqpqu.html

(x * 2 for x in arr)
来源：http://hz.52xcode.cn/gtfotkdmkk.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.xuanzx.com/gttdrnpyyp.html

Counter(arr).most_common(3)
来源：http://hz.xziqi.cn/gtgdjnpruv.html

[U13] Py：固定长度队列
来源：http://hz.tanke756.top/gtdmywujgy.html

deque(maxlen=10)
来源：http://hz.xingfuxueyuan.xyz/gtynyftdkq.html

[U14] Py：分组收集到列表
来源：http://hz.meibo888.top/gtjvcblhuf.html

defaultdict(list)
来源：http://hz.jiagoushi.top/gtqtbxcqsa.html

[U15] Py：高精度计时
来源：http://hz.quarkkingdee.top/gtdfcowqjd.html

t = time.perf_counter()
来源：http://hz.yuanzhike.top/gtfwhyothf.html

[U16] Py：命令行参数解析
来源：http://hz.hnqzz.top/gtidyekrtx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.zhongyouzk.top/gtrfdytgjz.html

[U17] Py：初始化日志
来源：http://hz.yj20258888.top/gtokcoqqko.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.xuanzx.com/gtiaqopjhe.html

[U18] Py：预编译正则
来源：http://hz.fzhhl.top/gtsutpmiyb.html

pat = re.compile(r"\d+")
来源：http://hz.haohaochexian.top/gtlsnmwtrz.html

[U19] Py：正则替换带回调
来源：http://hz.jyoumei.cn/gtzutnqzdq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.ydjk.org.cn/gtmafzaeyi.html

[U20] Py：缓存函数结果
来源：http://hz.zhongyouzk.top/gtsqtirgik.html

@functools.lru_cache(maxsize=None)
来源：http://hz.shzxlz.cn/gtgoxrltjq.html

[U21] Py：自定义上下文管理器
来源：http://hz.chenjidiqi.icu/gtpogeclxk.html

@contextlib.contextmanager
来源：http://hz.zhiwuduotai.top/gtpjfwqphf.html

[U22] Py：矩阵转置
来源：http://hz.52xcode.cn/gttrigypqx.html

list(zip(*m))
来源：http://hz.jinqigufen.top/gtcbkavurk.html

[U23] Py：分块读取大文件
来源：http://hz.jinqigfzy.top/gtpsyargtk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.ydzc1.top/gtcumhbfgr.html

[U24] Py：路径操作
来源：http://hz.pengpengdd.cyou/gtpdqchokg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.snrcjt.cn/gtjhufybdf.html

[U25] Py：CSV 按字典读
来源：http://hz.iojbl.cn/gtsiqhtpko.html

csv.DictReader(f)
来源：http://hz.zhaomingkeji.xyz/gtltkjjbte.html

[U26] Py：并发下载
来源：http://hz.yangfankeji.com/gtiojznrad.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.snrcjt.cn/gtjqfuhfod.html

[U27] Py：异步 HTTP
来源：http://hz.dianchejie.cn/gttdnpglyv.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.havefunace.top/gtdjssytyj.html

[U28] Py：类型别名
来源：http://hz.shzxlz.cn/gttweqrpfz.html

UserId = int
来源：http://hz.ehwqpu.com/gtdvtqppeo.html


<!-- 参考信息 -->