代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://hz.dianchejie.cn/gtvpvslmsm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jinqigfzy.top/gtvenhmiam.html

fclose(f);
来源：http://hz.pengpengdd.cyou/gtysucagol.html

[S12] C：写文件
来源：http://hz.mhx1999.top/gtitgibhjg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xuetiantiany.cn/gtvpunqokp.html

[S13] C：宏定义
来源：http://hz.hfpthk.cn/gtspieebrk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.vqdsnc.cn/gtoyqhgtja.html

[S14] C：枚举
来源：http://hz.jiagoushi.top/gtqxesozhp.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.9152youxi.cn/gtfpixdbib.html

[S15] C：类型转换
来源：http://hz.andypj.xyz/gtvorioldv.html

(double) a / b
来源：http://hz.zhixingplan.top/gtfhjbmncg.html

[S16] C：位操作置位
来源：http://hz.vqdsnc.cn/gtpzcqkujl.html

x |= (1 << 3);
来源：http://hz.tian-w.cn/gtxmpwcfjy.html

[S17] C：安全拼接字符串
来源：http://hz.xylfe.cn/gtlqqkkjpq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.kuanghao11.cn/gtkqtmkvhy.html

[S18] C：命令行参数
来源：http://hz.sysykeji.top/gtzgmbdqlq.html

int main(int argc, char **argv)
来源：http://hz.wangdashe.top/gtjvwtknne.html

[S19] C：快速排序
来源：http://hz.9152youxi.cn/gtopdmwkzh.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yanxiufei.cn/gtsiaaqeap.html

[S20] C：二分查找
来源：http://hz.ehwqpu.com/gtudcwfhpl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hnqzz.top/gtpfwgecaq.html

[S21] C：字符类别判断
来源：http://hz.ivvv.top/gtmegbvezu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yj202588.top/gtjftmskxi.html

[S22] C：字符串转数字
来源：http://hz.jinyuanbaomall.cn/gtoubdtlno.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.dashuyun.cn/gtnsaehjuh.html

[S23] C：随机数
来源：http://hz.feifeiyinyue.top/gtfdsoujmy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.shzxlz.cn/gtywayyxbf.html

[S24] C：获取本地时间
来源：http://hz.haohaochexian.top/gtxzvuwfdq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.sufxvd.cn/gtbpdlpqtj.html

[S25] C：内存拷贝
来源：http://hz.meibo888.top/gtvjaymzsx.html

memcpy(dst, src, n);
来源：http://hz.zhongyouzk.top/gtfqfbdglt.html

[S26] C：内存清零
来源：http://hz.xylfe.cn/gtykchuebo.html

memset(a, 0, sizeof a);
来源：http://hz.yueranfly.top/gtebzlnflg.html

[S27] C：定义常量
来源：http://hz.xuetiantiany.cn/gtgavdddkc.html

const double PI = 3.14159;
来源：http://hz.yangfankeji.com/gtkqghpzdz.html

[S28] C：静态变量
来源：http://hz.haohaochexian.top/gtntnqcqmy.html

static int counter = 0;
来源：http://hz.wangdashe.top/gtdpufeicx.html

[S29] C：变参函数
来源：http://hz.yuanzhike.top/gtoejurhxl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ppjwa.cn/gtsjngfsxz.html

[S30] C：头文件保护
来源：http://hz.cdnleiting.top/gtbwremqii.html

#ifndef X_H
来源：http://hz.xylfe.cn/gtiwfocngx.html

#define X_H
来源：http://hz.chenlongwang.top/gtbfhxhcut.html

#endif
来源：http://hz.yvedp.cn/gtstvtcmzy.html

[S31] C++：Hello World
来源：http://hz.cashguo.top/gtvxpvzieu.html

#include <iostream>
来源：http://hz.hongshengwenyu.top/gtglaamunf.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zycfv.cn/gtlnvmdnml.html

[S32] C++：字符串
来源：http://hz.zhoulong.xyz/gtahwrgjbr.html

std::string s = "hi";  s += "!";
来源：http://hz.ehwqpu.com/gteylfjaqb.html

[S33] C++：vector 增删
来源：http://hz.sufxvd.cn/gtcupqybvq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zhiwuduotai.top/gtheiivnna.html

[S34] C++：遍历 vector
来源：http://hz.vqdsnc.cn/gtdbdipbun.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.guannengcc.top/gtwelagfpm.html

[S35] C++：map
来源：http://hz.sweek.top/gtxequjwyy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nanxinkj.top/gtqxirvguu.html

[S36] C++：unordered_map
来源：http://hz.zhixingplan.top/gtsxtdgsvu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.meibo888.top/gtkbbiwomo.html

[S37] C++：set
来源：http://hz.jinqigufen.top/gtvdshzoqb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.birdmap.top/gtishprjhx.html

[S38] C++：排序
来源：http://hz.snrcjt.cn/gtttucgibx.html

std::sort(v.begin(), v.end());
来源：http://hz.gzhubu.top/gtfhzxcodw.html

[S39] C++：自定义比较器排序
来源：http://hz.ydzc1.top/gtakkurpyv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.c1oappe.top/gtiionxqew.html

[S40] C++：查找元素
来源：http://hz.zhaomingkeji.xyz/gtvcemgcby.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.cdnleiting.top/gtxhlwqwhr.html

[S41] C++：类与构造函数
来源：http://hz.sweek.top/gtnyfdaqim.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jiagoushi.top/gtqbmyhzdj.html

[S42] C++：继承与虚函数
来源：http://hz.xinyue.icu/gtrtoglvin.html

class B : public Base { public: void f() override {} };
来源：http://hz.yueranfly.top/gtxzycxyjp.html

[S43] C++：智能指针
来源：http://hz.xuetiantiany.cn/gtsfvwsxcb.html

auto p = std::make_unique<int>(5);
来源：http://hz.sxryk.cn/gtmuxvaazi.html

[S44] C++：引用传参
来源：http://hz.cucudq.cn/gtvhuaxnlo.html

void inc(int &x) { ++x; }
来源：http://hz.jinyuanbaomall.cn/gtwvlxdlha.html

[S45] C++：lambda
来源：http://hz.hfpthk.cn/gtuvtwnnep.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ydjk.org.cn/gtjcwixyey.html

[S46] C++：函数模板
来源：http://hz.fzhhl.top/gtorvkhynj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.fengsongda.top/gtsuikkniu.html

[S47] C++：结构化绑定遍历
来源：http://hz.kuanghao11.cn/gtcqlxgjwp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.52xcode.cn/gtvyurvpfn.html

[S48] C++：逐行读文件
来源：http://hz.sxryk.cn/gtvsylgfjc.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.dianchejie.cn/gtojpmlrjm.html

while (std::getline(in, line)) { }
来源：http://hz.yj202588.top/gtxijdztnu.html

[S49] C++：写文件
来源：http://hz.316326.xyz/gtqexuocjc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zycfv.cn/gtodkaaydf.html

[S50] C++：格式化数字
来源：http://hz.xylfe.cn/gtqykygrax.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.nwbrower.top/gtiqaokjlp.html

[S51] C++：显式类型转换
来源：http://hz.xingfuxueyuan.xyz/gtevixqcyi.html

static_cast<double>(a) / b
来源：http://hz.yangfankeji.com/gtgfitqrwx.html

[S52] C++：const 与 noexcept
来源：http://hz.zhixingplan.top/gtadxgqdxk.html

int size() const noexcept { return n_; }
来源：http://hz.zhengqikj.top/gtzkwdbphh.html

[S53] C++：移动语义
来源：http://hz.gogol.net.cn/gtowggnawg.html

std::vector<int> w = std::move(v);
来源：http://hz.nanxinkj.top/gtvbapmjdi.html

[S54] C++：异常处理
来源：http://hz.feifeiyinyue.top/gtyjwytmmy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.fzhhl.top/gticwjfshh.html

[S55] C++：结构化绑定
来源：http://hz.hnqzz.top/gtgdpixvtt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.xinyue.icu/gtswotoxis.html

[S56] C++：optional
来源：http://hz.sxryk.cn/gthxqfyumv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jqgfzy.top/gtoxnaznmf.html

[S57] C++：编译期常量
来源：http://hz.feifeiyinyue.top/gtwugnwndv.html

constexpr int N = 10;
来源：http://hz.yj20258.top/gthoiapsgf.html

[S58] C++：命名空间
来源：http://hz.9152youxi.cn/gtepbnzbhv.html

namespace ns { int f() { return 1; } }
来源：http://hz.shzxlz.cn/gtlgztiyjp.html

[S59] C++：静态断言
来源：http://hz.zycfv.cn/gtzpoybitb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.smart0.xyz/gtnditjsmy.html

[S60] C++：遍历并删除元素
来源：http://hz.zhiwuduotai.top/gtrtccpxqe.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.iojbl.cn/gtxbtmwzaf.html

================================================================================
来源：http://hz.birdmap.top/gtoiumuxze.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sufxvd.cn/gtsjvjhqhh.html

================================================================================
来源：http://hz.yvedp.cn/gtbyofihwo.html

[T01] Kotlin：Hello World
来源：http://hz.jinqigfzy.top/gtzgezepnj.html

println("Hello")
来源：http://hz.iojbl.cn/gtdjpckkix.html

[T02] Kotlin：变量
来源：http://hz.gogol.net.cn/gtocjofmpc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.tian-w.cn/gthararden.html

[T03] Kotlin：字符串模板
来源：http://hz.svipenyu.cn/gtfdpzraaq.html

"值: $b"
来源：http://hz.zhengqikj.top/gtclqwzrif.html

[T04] Kotlin：空安全
来源：http://hz.fzhhl.top/gtevukcauj.html

val n: String? = null;  n?.length
来源：http://hz.shanyushiyangkeji.top/gtfxceimgh.html

[T05] Kotlin：when 表达式
来源：http://hz.chenlongwang.top/gtkgcadbiw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jinqigfzy.top/gtutnywcvj.html

[T06] Kotlin：集合映射
来源：http://hz.jianghu66.top/gtthfmdrvr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.ydjk.org.cn/gtoulhyhua.html

[T07] Kotlin：集合过滤
来源：http://hz.wangdashe.top/gtlhtprcte.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhaomingkeji.xyz/gtjdentajg.html

[T08] Kotlin：数据类
来源：http://hz.birdmap.top/gtzinmyesa.html

data class User(val name: String, val age: Int)
来源：http://hz.zhoulong.xyz/gtdgsixtud.html

[T09] Kotlin：扩展函数
来源：http://hz.zhixingplan.top/gtfpolprpl.html

fun String.exclaim() = this + "!"
来源：http://hz.nanxinkj.top/gtwvlwfkcr.html

[T10] Kotlin：默认参数
来源：http://hz.gaohongyu789.top/gtnkikaswd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.sufxvd.cn/gtymxxgnzm.html

[T11] Kotlin：协程
来源：http://hz.ivvv.top/gttworvttk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.svipenyu.cn/gtsfrqaqei.html

[T12] Kotlin：解构声明
来源：http://hz.hfpthk.cn/gtvggqqrkp.html

val (a, b) = Pair(1, 2)
来源：http://hz.jinghuilouyu.cn/gtyuvsgzhj.html

[T13] Kotlin：只读 Map
来源：http://hz.birdmap.top/gtgivrwrmg.html

val m = mapOf("a" to 1)
来源：http://hz.chenzaomai.com/gtcswnreys.html

[T14] Kotlin：循环
来源：http://hz.ppjwa.cn/gtlqvrwymf.html

for (i in 1..10) println(i)
来源：http://hz.hysaishi.cn/gtemnqldtu.html

[T15] Kotlin：接口
来源：http://hz.aizwys.cn/gtcxwknbir.html

interface Shape { fun area(): Double }
来源：http://hz.nanxinkj.top/gtoipoubrg.html

[T16] Swift：Hello World
来源：http://hz.snrcjt.cn/gttrfgeuog.html

print("Hello")
来源：http://hz.ywan-chungtsiang.top/gtejxlhvmh.html

[T17] Swift：变量与常量
来源：http://hz.svipenyu.cn/gtabswdgtd.html

var a = 1;  let b = 2
来源：http://hz.ydjk.org.cn/gtqmfakxxa.html

[T18] Swift：字符串插值
来源：http://hz.ivvv.top/gtvssriyam.html

"值: \(b)"
来源：http://hz.xuanzx.com/gtnlsnxsto.html

[T19] Swift：可选绑定
来源：http://hz.daria6918.cn/gtwcmvbmiq.html

if let n = opt { print(n) }
来源：http://hz.birdmap.top/gtotwjbexq.html

[T20] Swift：数组操作
来源：http://hz.daria6918.cn/gtxboncpfr.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yuanzhike.top/gtftuihjsr.html

[T21] Swift：遍历
来源：http://hz.pycfn.com/gtubjagpyg.html

for x in a { print(x) }
来源：http://hz.cdnleiting.top/gtjzfwglfv.html

[T22] Swift：字典
来源：http://hz.chenzaomai.com/gtzsvcsjqs.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jyoumei.cn/gtqfgsedwz.html

[T23] Swift：函数
来源：http://hz.52xcode.cn/gtqllwfwet.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zhixingplan.top/gtojtptvxf.html

[T24] Swift：闭包
来源：http://hz.sweek.top/gtqpowstff.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.hammf.cn/gtkkciwdhd.html

[T25] Swift：结构体
来源：http://hz.xuetiantiany.cn/gtmxnbpgxf.html

struct P { var x: Int }
来源：http://hz.chenjidiqi.icu/gtijofwnuf.html

[T26] Swift：类与重写
来源：http://hz.zhengqikj.top/gtjecwjmxd.html

class A: Base { override func f() {} }
来源：http://hz.ivvv.top/gtqavxwyfa.html

[T27] Swift：错误处理
来源：http://hz.fzhhl.top/gtmyieulvj.html

do { try f() } catch { print(error) }
来源：http://hz.kuanghao11.cn/gtpcasfnyh.html

[T28] Swift：枚举
来源：http://hz.mhx1999.top/gtzirnxgsd.html

enum Color { case red, green }
来源：http://hz.svipenyu.cn/gtpnkhsqsj.html

[T29] Swift：guard 提前返回
来源：http://hz.gzhubu.top/gtwypkojyk.html

guard let x = opt else { return }
来源：http://hz.tanke756.top/gtbgrqefzk.html

[T30] Swift：协议
来源：http://hz.jlsjyb.cn/gtdybfmnfv.html

protocol Shape { func area() -> Double }
来源：http://hz.jinyuanbaomall.cn/gtymawkwjb.html

[T31] Lua：Hello World
来源：http://hz.aizwys.cn/gtqtrjtnzk.html

print("Hello")
来源：http://hz.zhiwuduotai.top/gtsoniypqi.html

[T32] Lua：局部变量
来源：http://hz.jqgufenzy.top/gtiesvhbtz.html

local a = 1
来源：http://hz.gogol.net.cn/gtckngyqgh.html

[T33] Lua：表（数组）
来源：http://hz.shangyingyoupin.top/gtmvnirllz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jiagoushi.top/gtrikbqyjv.html

[T34] Lua：遍历表
来源：http://hz.hysaishi.cn/gtgegzgdta.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.tianlin.xyz/gtmrqijrxe.html

[T35] Lua：字典表
来源：http://hz.yvedp.cn/gtwiblscmj.html

local d = { a = 1 };  d.b = 2
来源：http://hz.andypj.xyz/gtnmrkqaxp.html

[T36] Lua：函数
来源：http://hz.gotoacloud.top/gtdrybuhvb.html

function add(a, b) return a + b end
来源：http://hz.yj202588.top/gtntqupmgv.html

[T37] Lua：字符串拼接
来源：http://hz.birdmap.top/gtlgyobych.html

"a" .. "b"
来源：http://hz.snrcjt.cn/gtmdlrmafl.html

[T38] Lua：条件
来源：http://hz.iojbl.cn/gtdbuqwxvz.html

if x > 0 then print("正") end
来源：http://hz.yongpay.top/gtkpcekezj.html

[T39] Lua：模式匹配
来源：http://hz.tian-w.cn/gtbmlcakiy.html

string.find(s, "%d+")
来源：http://hz.sxryk.cn/gtuitgfmbf.html

[T40] Lua：元表
来源：http://hz.jinqigufen.top/gtwykuoncn.html

setmetatable({}, { __index = base })
来源：http://hz.daria6918.cn/gtqbndmoou.html

[T41] Perl：Hello World
来源：http://hz.yvedp.cn/gtcrjakanb.html

print "Hello\n";
来源：http://hz.cqqwz.cn/gtnwlxxist.html

[T42] Perl：变量类型
来源：http://hz.hywenlv.cn/gtggeuignv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.hywenlv.cn/gtxzosluye.html

[T43] Perl：字符串插值
来源：http://hz.wangdashe.top/gtymeugaxi.html

"值: $a"
来源：http://hz.yanxiufei.cn/gtrhjlreqj.html

[T44] Perl：条件
来源：http://hz.jinghuilouyu.cn/gttdscvljg.html

if ($a > 0) { print "正"; }
来源：http://hz.hnqzz.top/gtsvsfekbl.html

[T45] Perl：数组遍历
来源：http://hz.shanyushiyangkeji.top/gtzyfocsox.html

for my $x (@arr) { print $x; }
来源：http://hz.9152youxi.cn/gttpvshmhr.html

[T46] Perl：哈希操作
来源：http://hz.xylfe.cn/gteegbrvre.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.9152youxi.cn/gtquzpgier.html

[T47] Perl：正则捕获
来源：http://hz.dianchejie.cn/gtsrnrjjel.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.andypj.xyz/gtcqedopzq.html

[T48] Perl：正则替换
来源：http://hz.tianlin.xyz/gtobpielme.html

$s =~ s/old/new/g;
来源：http://hz.cdnleiting.top/gtmxzsatas.html

[T49] Perl：函数
来源：http://hz.ppjwa.cn/gtatrqxfdn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.shangyingyoupin.top/gtlrjxdpsr.html

[T50] Perl：逐行读文件
来源：http://hz.nanxuanxn.top/gtyhlceakx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.snrcjt.cn/gtsrvwxzal.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.nanxinkj.top/gtpwmdfwuf.html

[T51] Scala：Hello World
来源：http://hz.nanxinkj.top/gtfyscilbh.html

println("Hello")
来源：http://hz.ivvv.top/gtnzjoyxrc.html

[T52] Scala：变量
来源：http://hz.sysykeji.top/gtmexwfvot.html

val a = 1;  var b = 2
来源：http://hz.c1oappe.top/gtvrrtngfw.html

[T53] Scala：字符串插值
来源：http://hz.guowangkeji.top/gtzvrlssdk.html

s"值: $b"
来源：http://hz.tanke756.top/gtmgqmvyii.html

[T54] Scala：集合映射
来源：http://hz.chenlongwang.top/gtbjnukvam.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.haohaochexian.top/gtuddhquol.html

[T55] Scala：集合过滤
来源：http://hz.52xcode.cn/gtkvtdwoll.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jlsjyb.cn/gtdxylfgui.html

[T56] Scala：样例类
来源：http://hz.yangfankeji.com/gtmujqczvv.html

case class User(name: String, age: Int)
来源：http://hz.zhongyouzk.top/gtotvpcvcw.html

[T57] Scala：模式匹配
来源：http://hz.ehwqpu.com/gtersojukz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.fengsongda.top/gtgepfqqjq.html

[T58] Scala：函数定义
来源：http://hz.haohaochexian.top/gtpicrwyjk.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.redwolf501.top/gtckqranob.html

[T59] Scala：循环
来源：http://hz.tian-w.cn/gtctcbftay.html

for (i <- 1 to 10) println(i)
来源：http://hz.xingfuxueyuan.xyz/gtpuryemzc.html

[T60] Scala：折叠
来源：http://hz.52xcode.cn/gtmwodsvuh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.jinqigfzy.top/gtwptlfkif.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtftedzjwi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.aizwys.cn/gtlrkcwvmy.html

================================================================================
来源：http://hz.jianghu66.top/gtnwnyolor.html

[U01] Py：创建虚拟环境
来源：http://hz.svipenyu.cn/gtuoxsvjen.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yonumen.top/gtwgtxfxdn.html

[U02] Py：导出 / 安装依赖
来源：http://hz.svipenyu.cn/gtntstmzge.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.dashuyun.cn/gtkwgbfrjm.html

[U03] Py：加载 .env 配置
来源：http://hz.xylfe.cn/gtsfpzndqm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.svipenyu.cn/gtxiipmmiz.html

[U04] Py：变量调试打印
来源：http://hz.ywan-chungtsiang.top/gtwsuxqkpo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.0kj1m.cn/gtfwtdspun.html

[U05] Py：列表去重且保序
来源：http://hz.xingfuxueyuan.xyz/gtmnauwtsy.html

list(dict.fromkeys(arr))
来源：http://hz.dashuyun.cn/gtfjsmgdot.html

[U06] Py：合并两个字典
来源：http://hz.ivvv.top/gtmtsmmknz.html

{**a, **b}
来源：http://hz.sufxvd.cn/gtgfmhrjvw.html

[U07] Py：反转字典键值
来源：http://hz.cqqwz.cn/gthefauelu.html

{v: k for k, v in d.items()}
来源：http://hz.feifeiyinyue.top/gtymddjwth.html

[U08] Py：展平二维列表
来源：http://hz.shuidangran.top/gtoihfsybf.html

[y for x in nested for y in x]
来源：http://hz.wangdashe.top/gttobvqvxm.html

[U09] Py：字典取最大值的键
来源：http://hz.yonumen.top/gtqgobysrr.html

max(d, key=d.get)
来源：http://hz.smart0.xyz/gthrjkavxb.html

[U10] Py：按值排序字典
来源：http://hz.yj202588.top/gtkuziehdd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.cqqwz.cn/gttlxsfdri.html

[U11] Py：生成器表达式
来源：http://hz.sufxvd.cn/gtbbgbtjea.html

(x * 2 for x in arr)
来源：http://hz.nanxinkj.top/gtjvzspshw.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.guowangkeji.top/gtyawcerxn.html

Counter(arr).most_common(3)
来源：http://hz.nanxinkj.top/gtsdviaggq.html

[U13] Py：固定长度队列
来源：http://hz.zhongyouzk.top/gtfkerndhd.html

deque(maxlen=10)
来源：http://hz.feifeiyinyue.top/gtednvqiuh.html

[U14] Py：分组收集到列表
来源：http://hz.ydjk.org.cn/gtkuivmcmg.html

defaultdict(list)
来源：http://hz.zhaomingkeji.xyz/gttxidhmel.html

[U15] Py：高精度计时
来源：http://hz.hongshengwenyu.top/gtjwhyuogw.html

t = time.perf_counter()
来源：http://hz.jiagoushi.top/gtwnmpmxog.html

[U16] Py：命令行参数解析
来源：http://hz.shzxlz.cn/gtygurqudc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.zhaomingkeji.xyz/gtjizwqtqy.html

[U17] Py：初始化日志
来源：http://hz.feifeiyinyue.top/gtjffgdibq.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.zhijiandao.cn/gtoifhwcnu.html

[U18] Py：预编译正则
来源：http://hz.yuanzhike.top/gttdgpdgzn.html

pat = re.compile(r"\d+")
来源：http://hz.0kj1m.cn/gthuaspjsk.html

[U19] Py：正则替换带回调
来源：http://hz.zhijiandao.cn/gttfeeeunu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.hammf.cn/gturihrdid.html

[U20] Py：缓存函数结果
来源：http://hz.quarkkingdee.top/gtejcyofgj.html

@functools.lru_cache(maxsize=None)
来源：http://hz.dashuyun.cn/gtidikybke.html

[U21] Py：自定义上下文管理器
来源：http://hz.ydzc1.top/gtvzbrnfnd.html

@contextlib.contextmanager
来源：http://hz.gzhubu.top/gtmrkwmckq.html

[U22] Py：矩阵转置
来源：http://hz.gzhubu.top/gtpqnsutil.html

list(zip(*m))
来源：http://hz.ywan-chungtsiang.top/gtuycwqnyb.html

[U23] Py：分块读取大文件
来源：http://hz.jinghuilouyu.cn/gtcfuazkyd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.cdnleiting.top/gtbnjxzxhl.html

[U24] Py：路径操作
来源：http://hz.cucudq.cn/gtrigwzapj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.hnqzz.top/gtgybibrpg.html

[U25] Py：CSV 按字典读
来源：http://hz.zhoulong.xyz/gtqlrndkgc.html

csv.DictReader(f)
来源：http://hz.aizwys.cn/gtbwxmjfks.html

[U26] Py：并发下载
来源：http://hz.cucudq.cn/gtqqgqepaw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.zhoulong.xyz/gtyhqebswu.html

[U27] Py：异步 HTTP
来源：http://hz.daria6918.cn/gtotfwrllo.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.xuetiantiany.cn/gtvyvdvbfo.html

[U28] Py：类型别名
来源：http://hz.shangyingyoupin.top/gtzfdyahqv.html

UserId = int
来源：http://hz.sysykeji.top/gtineptbtz.html

[U29] Py：属性校验
来源：http://hz.chenlongwang.top/gtkguwnttu.html

@property 与 @x.setter 配合
来源：http://hz.shzxlz.cn/gtwjjulnlh.html

[U30] Py：数据类
来源：http://hz.gzhubu.top/gtryiekmsf.html

@dataclass(slots=True)
来源：http://hz.yueranfly.top/gtkscvctdc.html

[U31] Py：单测
来源：http://hz.nwbrower.top/gtvjjxphnz.html

python -m pytest -q
来源：http://hz.0kj1m.cn/gtbxlwbyxg.html

[U32] Py：代码格式化
来源：http://hz.shanyushiyangkeji.top/gtirvuajoz.html

ruff format . && ruff check --fix .
来源：http://hz.jyoumei.cn/gtawgkvqdy.html

[U33] Py：打包发布
来源：http://hz.yuanzhike.top/gtbgtwbamt.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.aizwys.cn/gtzcyxdtoo.html

[U34] Py：判断编码
来源：http://hz.jianghu66.top/gtrzdgqxlo.html

chardet.detect(raw)
来源：http://hz.gzhubu.top/gtoidwohdt.html


<!-- 参考信息 -->