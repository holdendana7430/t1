代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.tianlin.xyz/gtgfdnoizi.html

[S13] C：宏定义
来源：http://hz.kuanghao11.cn/gtnnuwqlsx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.cashguo.top/gtjdzpymfx.html

[S14] C：枚举
来源：http://hz.cashguo.top/gtmupearho.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.fzhhl.top/gtozakpziv.html

[S15] C：类型转换
来源：http://hz.gotoacloud.top/gtzhqqelov.html

(double) a / b
来源：http://hz.andypj.xyz/gtyufugqtg.html

[S16] C：位操作置位
来源：http://hz.chenlongwang.top/gtqvsxvuze.html

x |= (1 << 3);
来源：http://hz.gzhubu.top/gtdpgeeoda.html

[S17] C：安全拼接字符串
来源：http://hz.jinqigfzy.top/gtpjubdcxg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhijiandao.cn/gtkusinbfc.html

[S18] C：命令行参数
来源：http://hz.chenzaomai.com/gtemeoqjtt.html

int main(int argc, char **argv)
来源：http://hz.kuanghao11.cn/gtfngeywnx.html

[S19] C：快速排序
来源：http://hz.jianghu66.top/gtwtpkhktz.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.ppjwa.cn/gthlchyywg.html

[S20] C：二分查找
来源：http://hz.c1oappe.top/gtncvruhtm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ivvv.top/gtxiftrlho.html

[S21] C：字符类别判断
来源：http://hz.shangyingyoupin.top/gtyxklypgv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.andypj.xyz/gttvtcprev.html

[S22] C：字符串转数字
来源：http://hz.pengpengdd.cyou/gtunfuwkyh.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xinyue.icu/gtzcaasezn.html

[S23] C：随机数
来源：http://hz.pycfn.com/gtqzfwrttr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.sweek.top/gtewjfebxr.html

[S24] C：获取本地时间
来源：http://hz.zycfv.cn/gtunnrbfpi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.dashuyun.cn/gtbqruxire.html

[S25] C：内存拷贝
来源：http://hz.ybcxt.top/gtgwukfuae.html

memcpy(dst, src, n);
来源：http://hz.sweek.top/gtljnffles.html

[S26] C：内存清零
来源：http://hz.ydjk.org.cn/gtwjykophc.html

memset(a, 0, sizeof a);
来源：http://hz.ydzc1.top/gtikfygcts.html

[S27] C：定义常量
来源：http://hz.jianghu66.top/gtuwzpajhq.html

const double PI = 3.14159;
来源：http://hz.cucudq.cn/gtrykmqrpl.html

[S28] C：静态变量
来源：http://hz.zhongyouzk.top/gtbhsfavip.html

static int counter = 0;
来源：http://hz.pengpengdd.cyou/gtcmquymnf.html

[S29] C：变参函数
来源：http://hz.xinyue.icu/gtjkufpyzq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.daxiang520.top/gtxkyylhcz.html

[S30] C：头文件保护
来源：http://hz.jiagoushi.top/gtezfarajs.html

#ifndef X_H
来源：http://hz.shanyushiyangkeji.top/gtwbyzuhhx.html

#define X_H
来源：http://hz.dashuyun.cn/gtmvdbmbal.html

#endif
来源：http://hz.jinyuanbaomall.cn/gtyjruaptb.html

[S31] C++：Hello World
来源：http://hz.zhoulong.xyz/gtqylsaouz.html

#include <iostream>
来源：http://hz.chenzaomai.com/gtiozvzecb.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.shanyushiyangtech.top/gtplkpesud.html

[S32] C++：字符串
来源：http://hz.yj202588.top/gtcjllctyh.html

std::string s = "hi";  s += "!";
来源：http://hz.xylfe.cn/gtayvdcsxb.html

[S33] C++：vector 增删
来源：http://hz.fengsongda.top/gtquwjfpic.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yangfankeji.com/gtywftiwqm.html

[S34] C++：遍历 vector
来源：http://hz.aibaodan.cn/gtbalmtvky.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.52xcode.cn/gtgweewhsf.html

[S35] C++：map
来源：http://hz.snrcjt.cn/gtdjmqxmhf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sufxvd.cn/gtqnkndiic.html

[S36] C++：unordered_map
来源：http://hz.jyoumei.cn/gttwjdrmkv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shuidangran.top/gtvexcfqka.html

[S37] C++：set
来源：http://hz.daria6918.cn/gthxjzggib.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hnxiangtu.top/gtarrdccni.html

[S38] C++：排序
来源：http://hz.gotoacloud.top/gtzlnruzti.html

std::sort(v.begin(), v.end());
来源：http://hz.0kj1m.cn/gtsizhitxn.html

[S39] C++：自定义比较器排序
来源：http://hz.shangyingyoupin.top/gtcgtuflqe.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ydzc1.top/gtolprewcc.html

[S40] C++：查找元素
来源：http://hz.hfpthk.cn/gtkjwanvio.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.ehwqpu.com/gtgznzetsv.html

[S41] C++：类与构造函数
来源：http://hz.xuetiantiany.cn/gtatqvgbhg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.sufxvd.cn/gtdjadsshx.html

[S42] C++：继承与虚函数
来源：http://hz.chenzaomai.com/gtukbbbqnl.html

class B : public Base { public: void f() override {} };
来源：http://hz.havefunace.top/gtfzlbxpkk.html

[S43] C++：智能指针
来源：http://hz.ppjwa.cn/gtoyhlsfso.html

auto p = std::make_unique<int>(5);
来源：http://hz.shanyushiyangkeji.top/gtwypclzru.html

[S44] C++：引用传参
来源：http://hz.zhongyouzk.top/gtmoctzwut.html

void inc(int &x) { ++x; }
来源：http://hz.chenjidiqi.icu/gtvwjnjcdt.html

[S45] C++：lambda
来源：http://hz.shuidangran.top/gtacrwfwle.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.redwolf501.top/gtoksjnwfc.html

[S46] C++：函数模板
来源：http://hz.vqdsnc.cn/gtmlnqagjh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jqgufenzy.top/gttsduaiqk.html

[S47] C++：结构化绑定遍历
来源：http://hz.xinyue.icu/gtwdndlpwc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.pengpengdd.cyou/gtgearhbrt.html

[S48] C++：逐行读文件
来源：http://hz.zhiwuduotai.top/gtxcchcfbs.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.hnqzz.top/gtxujmkizy.html

while (std::getline(in, line)) { }
来源：http://hz.52xcode.cn/gtimwczhia.html

[S49] C++：写文件
来源：http://hz.havefunace.top/gtdhkhhkud.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.xylfe.cn/gtxzfiezwa.html

[S50] C++：格式化数字
来源：http://hz.quarkkingdee.top/gtfsgxqbnl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jyoumei.cn/gtemurkrke.html

[S51] C++：显式类型转换
来源：http://hz.sxryk.cn/gtfeorkgnb.html

static_cast<double>(a) / b
来源：http://hz.aibaodan.cn/gtvjgzopia.html

[S52] C++：const 与 noexcept
来源：http://hz.zhengqikj.top/gtacflofna.html

int size() const noexcept { return n_; }
来源：http://hz.jinqigfzy.top/gtgaatexmr.html

[S53] C++：移动语义
来源：http://hz.cdnleiting.top/gtfhogeycn.html

std::vector<int> w = std::move(v);
来源：http://hz.mhx1999.top/gtpdrncwfk.html

[S54] C++：异常处理
来源：http://hz.yueranfly.top/gtuomytdgd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.havefunace.top/gtgbgrbkyb.html

[S55] C++：结构化绑定
来源：http://hz.shanyushiyangtech.top/gtqshqbsuh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.havefunace.top/gtajqfiame.html

[S56] C++：optional
来源：http://hz.snrcjt.cn/gtmqdtvipm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yvedp.cn/gtlejldfta.html

[S57] C++：编译期常量
来源：http://hz.sysykeji.top/gtbvvejxsr.html

constexpr int N = 10;
来源：http://hz.jqgfzy.top/gtvivjoexr.html

[S58] C++：命名空间
来源：http://hz.shzxlz.cn/gtoajfeytj.html

namespace ns { int f() { return 1; } }
来源：http://hz.hysaishi.cn/gtyfdrivez.html

[S59] C++：静态断言
来源：http://hz.cashguo.top/gtllsycayb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ybcxt.top/gticesnqpr.html

[S60] C++：遍历并删除元素
来源：http://hz.shangyingyoupin.top/gtevfqsscp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.quarkkingdee.top/gtfvdtnazm.html

================================================================================
来源：http://hz.gotoacloud.top/gtevpydffb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.fengsongda.top/gtxbnyzdfn.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtdrngmicx.html

[T01] Kotlin：Hello World
来源：http://hz.mhx1999.top/gthwodwtlh.html

println("Hello")
来源：http://hz.iojbl.cn/gtjkcbufgu.html

[T02] Kotlin：变量
来源：http://hz.kuanghao11.cn/gtzpgencmm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.fzhhl.top/gtqxamkjlm.html

[T03] Kotlin：字符串模板
来源：http://hz.xylfe.cn/gtxusrvtuc.html

"值: $b"
来源：http://hz.yuanzhike.top/gtrskyemzs.html

[T04] Kotlin：空安全
来源：http://hz.vqdsnc.cn/gtkpwykdhi.html

val n: String? = null;  n?.length
来源：http://hz.jqgfzy.top/gtoqpfaqpv.html

[T05] Kotlin：when 表达式
来源：http://hz.chenlongwang.top/gtieylnjep.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.xinyue.icu/gtjmhfexkc.html

[T06] Kotlin：集合映射
来源：http://hz.zhengqikj.top/gtmhfbopte.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yonumen.top/gtfvbdflpb.html

[T07] Kotlin：集合过滤
来源：http://hz.shuidangran.top/gtnuigtafv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.andypj.xyz/gtlihzzjrq.html

[T08] Kotlin：数据类
来源：http://hz.hysaishi.cn/gtddifhbda.html

data class User(val name: String, val age: Int)
来源：http://hz.yongpay.top/gtkmgcbnfn.html

[T09] Kotlin：扩展函数
来源：http://hz.gzhubu.top/gtlgjpusth.html

fun String.exclaim() = this + "!"
来源：http://hz.yj20258.top/gtsmhgonqj.html

[T10] Kotlin：默认参数
来源：http://hz.tanke756.top/gtgmjvqlkk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.redwolf501.top/gtgicogxuj.html

[T11] Kotlin：协程
来源：http://hz.zycfv.cn/gttyaqrapj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.bjfxy.top/gtgoqryiay.html

[T12] Kotlin：解构声明
来源：http://hz.quarkkingdee.top/gtzbsorgkm.html

val (a, b) = Pair(1, 2)
来源：http://hz.jinyuanbaomall.cn/gtxnlewgat.html

[T13] Kotlin：只读 Map
来源：http://hz.ywan-chungtsiang.top/gttvyazxkk.html

val m = mapOf("a" to 1)
来源：http://hz.9152youxi.cn/gttqshsexm.html

[T14] Kotlin：循环
来源：http://hz.zhiwuduotai.top/gtqzkadfxs.html

for (i in 1..10) println(i)
来源：http://hz.ydjk.org.cn/gtqosbklmn.html

[T15] Kotlin：接口
来源：http://hz.haohaochexian.top/gtbccjfhyo.html

interface Shape { fun area(): Double }
来源：http://hz.iojbl.cn/gtwkyypysz.html

[T16] Swift：Hello World
来源：http://hz.jinghuilouyu.cn/gtlmktmuvd.html

print("Hello")
来源：http://hz.jinqigufen.top/gtfgtwqvsh.html

[T17] Swift：变量与常量
来源：http://hz.sweek.top/gtmbsdiwwy.html

var a = 1;  let b = 2
来源：http://hz.cdnleiting.top/gtxxefrjid.html

[T18] Swift：字符串插值
来源：http://hz.sweek.top/gtunhxndpq.html

"值: \(b)"
来源：http://hz.yj202588.top/gtvbssgicq.html

[T19] Swift：可选绑定
来源：http://hz.fzhhl.top/gtoylxedmu.html

if let n = opt { print(n) }
来源：http://hz.zhoulong.xyz/gtqremczmi.html

[T20] Swift：数组操作
来源：http://hz.iojbl.cn/gtlcimteiy.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.quarkkingdee.top/gtnsinpakc.html

[T21] Swift：遍历
来源：http://hz.jinghuilouyu.cn/gtbkfbctbq.html

for x in a { print(x) }
来源：http://hz.dianchejie.cn/gtnlkanldp.html

[T22] Swift：字典
来源：http://hz.pycfn.com/gtnbqaxplf.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.aibaodan.cn/gtrbsmhufr.html

[T23] Swift：函数
来源：http://hz.yongpay.top/gtsieghfxy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zhixingplan.top/gtpttbfruz.html

[T24] Swift：闭包
来源：http://hz.zhongyouzk.top/gtkdxlzlov.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.mhx1999.top/gtjifjssnc.html

[T25] Swift：结构体
来源：http://hz.yj20258888.top/gtuhhwrago.html

struct P { var x: Int }
来源：http://hz.sweek.top/gtyekkviuh.html

[T26] Swift：类与重写
来源：http://hz.cheryme.top/gtjakvrtfm.html

class A: Base { override func f() {} }
来源：http://hz.gzhubu.top/gtebaysrkv.html

[T27] Swift：错误处理
来源：http://hz.redwolf501.top/gtwsbdtohf.html

do { try f() } catch { print(error) }
来源：http://hz.shuidangran.top/gtrjkymtqu.html

[T28] Swift：枚举
来源：http://hz.iojbl.cn/gtmqgzilxh.html

enum Color { case red, green }
来源：http://hz.xziqi.cn/gtweuehjrc.html

[T29] Swift：guard 提前返回
来源：http://hz.shzxlz.cn/gtdnanfvyi.html

guard let x = opt else { return }
来源：http://hz.wangshuangyany.cn/gtocqldvva.html

[T30] Swift：协议
来源：http://hz.wangdashe.top/gtmjcfgcjl.html

protocol Shape { func area() -> Double }
来源：http://hz.hywenlv.cn/gtpbsgokil.html

[T31] Lua：Hello World
来源：http://hz.svipenyu.cn/gtxvuogfjq.html

print("Hello")
来源：http://hz.iojbl.cn/gtagzyawxd.html

[T32] Lua：局部变量
来源：http://hz.sxryk.cn/gtwnakjxwt.html

local a = 1
来源：http://hz.cdnleiting.top/gtwgpisgbk.html

[T33] Lua：表（数组）
来源：http://hz.iojbl.cn/gteqohslwo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.pycfn.com/gtakzsucxx.html

[T34] Lua：遍历表
来源：http://hz.redwolf501.top/gtbxaxpbpw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.gaohongyu789.top/gtayzixkgv.html

[T35] Lua：字典表
来源：http://hz.cqqwz.cn/gtepdmbgvr.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yj20258888.top/gtkzcuavsm.html

[T36] Lua：函数
来源：http://hz.zhongyouzk.top/gtlqqmfyra.html

function add(a, b) return a + b end
来源：http://hz.ybcxt.top/gtltxcgnun.html

[T37] Lua：字符串拼接
来源：http://hz.quarkkingdee.top/gtmlpemzoh.html

"a" .. "b"
来源：http://hz.yangfankeji.com/gtrnlnojjb.html

[T38] Lua：条件
来源：http://hz.hnqzz.top/gtikywwvgj.html

if x > 0 then print("正") end
来源：http://hz.jqgufenzy.top/gtwhbxhtun.html

[T39] Lua：模式匹配
来源：http://hz.feifeiyinyue.top/gtbahmmyif.html

string.find(s, "%d+")
来源：http://hz.sysykeji.top/gtmeymnxig.html

[T40] Lua：元表
来源：http://hz.pycfn.com/gtcrgaykhn.html

setmetatable({}, { __index = base })
来源：http://hz.yuanzhike.top/gtucgqwaag.html

[T41] Perl：Hello World
来源：http://hz.shzxlz.cn/gtiwzamxuc.html

print "Hello\n";
来源：http://hz.jinqigfzy.top/gtcblqpdgn.html

[T42] Perl：变量类型
来源：http://hz.yj202588.top/gtscceybhp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.gotoacloud.top/gtbicagcfe.html

[T43] Perl：字符串插值
来源：http://hz.ppjwa.cn/gtzseugath.html

"值: $a"
来源：http://hz.hammf.cn/gtdyxjpnxc.html

[T44] Perl：条件
来源：http://hz.hywenlv.cn/gtevvletml.html

if ($a > 0) { print "正"; }
来源：http://hz.xuanzx.com/gtcqdjyomq.html

[T45] Perl：数组遍历
来源：http://hz.tanke756.top/gtlpnxesdq.html

for my $x (@arr) { print $x; }
来源：http://hz.tianlin.xyz/gtntfhhnll.html

[T46] Perl：哈希操作
来源：http://hz.hysaishi.cn/gtsgezkmcx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.gzhubu.top/gtxsnqqxwd.html

[T47] Perl：正则捕获
来源：http://hz.shzxlz.cn/gtbolftwya.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.ybcxt.top/gtxivgouwh.html

[T48] Perl：正则替换
来源：http://hz.9152youxi.cn/gtlbjkxbnd.html

$s =~ s/old/new/g;
来源：http://hz.ivvv.top/gtdsqdiafc.html

[T49] Perl：函数
来源：http://hz.zhongyouzk.top/gtqovndtik.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.svipenyu.cn/gtgqfzucpu.html

[T50] Perl：逐行读文件
来源：http://hz.chenzaomai.com/gtvkxlubpg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.sweek.top/gtiwyirmfj.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.guowangkeji.top/gtjpzwbjnx.html

[T51] Scala：Hello World
来源：http://hz.pengpengdd.cyou/gtueqdsxbi.html

println("Hello")
来源：http://hz.havefunace.top/gtzcjenysu.html

[T52] Scala：变量
来源：http://hz.nanxuanxn.top/gtretltmxq.html

val a = 1;  var b = 2
来源：http://hz.nanxinkj.top/gtuhvtrogy.html

[T53] Scala：字符串插值
来源：http://hz.fzhhl.top/gtqvwegjtg.html

s"值: $b"
来源：http://hz.zhengqikj.top/gtaituamfj.html

[T54] Scala：集合映射
来源：http://hz.iojbl.cn/gttldgfded.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.nanxuanxn.top/gtvpcjsawv.html

[T55] Scala：集合过滤
来源：http://hz.chenjidiqi.icu/gtqubugfmc.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.andypj.xyz/gthqmpwwsl.html

[T56] Scala：样例类
来源：http://hz.meibo888.top/gthxkqjqeq.html

case class User(name: String, age: Int)
来源：http://hz.tanke756.top/gtgyieizks.html

[T57] Scala：模式匹配
来源：http://hz.zhiwuduotai.top/gtkqswylxe.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.c1oappe.top/gtihhnestl.html

[T58] Scala：函数定义
来源：http://hz.hnxiangtu.top/gtukqkdxue.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.cqqwz.cn/gtzcoeftyp.html

[T59] Scala：循环
来源：http://hz.zhengqikj.top/gtvydkmqrl.html

for (i <- 1 to 10) println(i)
来源：http://hz.yonumen.top/gtzsuvpbgn.html

[T60] Scala：折叠
来源：http://hz.316326.xyz/gtskbhoslm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.tanke756.top/gtnpaqyuwc.html

================================================================================
来源：http://hz.wangdashe.top/gtpnmcvtdl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.0kj1m.cn/gtvwplzyle.html

================================================================================
来源：http://hz.shzxlz.cn/gtxrwijkyl.html

[U01] Py：创建虚拟环境
来源：http://hz.dashuyun.cn/gttssudyww.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yueranfly.top/gtlyvfewrh.html

[U02] Py：导出 / 安装依赖
来源：http://hz.sufxvd.cn/gtfuzllihj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.c1oappe.top/gtakxndpcw.html

[U03] Py：加载 .env 配置
来源：http://hz.shanyushiyangkeji.top/gtewwgcfwa.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.hysaishi.cn/gtiqfplogb.html

[U04] Py：变量调试打印
来源：http://hz.sufxvd.cn/gtpnqppwip.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jqgfzy.top/gtapmnaivz.html

[U05] Py：列表去重且保序
来源：http://hz.bjfxy.top/gttjomdybp.html

list(dict.fromkeys(arr))
来源：http://hz.chenjidiqi.icu/gtyqaodjgh.html

[U06] Py：合并两个字典
来源：http://hz.cheryme.top/gtlgxgpsmr.html

{**a, **b}
来源：http://hz.dianchejie.cn/gtgpqjpoew.html

[U07] Py：反转字典键值
来源：http://hz.xuanzx.com/gtviduyctj.html

{v: k for k, v in d.items()}
来源：http://hz.zhongyouzk.top/gtxycrdjmd.html

[U08] Py：展平二维列表
来源：http://hz.xylfe.cn/gtyelumzri.html

[y for x in nested for y in x]
来源：http://hz.sysykeji.top/gtspufudme.html

[U09] Py：字典取最大值的键
来源：http://hz.zhengqikj.top/gtzxuhiprs.html

max(d, key=d.get)
来源：http://hz.jqgufenzy.top/gtstvauzcw.html

[U10] Py：按值排序字典
来源：http://hz.fengsongda.top/gtjyqdvtah.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yj202588.top/gtubcxwscd.html

[U11] Py：生成器表达式
来源：http://hz.jianghu66.top/gtaktqgudj.html

(x * 2 for x in arr)
来源：http://hz.ydjk.org.cn/gthrsqqckh.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.xinyue.icu/gttsapcvzl.html

Counter(arr).most_common(3)
来源：http://hz.hongshengwenyu.top/gtoixofftv.html

[U13] Py：固定长度队列
来源：http://hz.yonumen.top/gtjflgjbhv.html

deque(maxlen=10)
来源：http://hz.zhengqikj.top/gtlmxsaldh.html

[U14] Py：分组收集到列表
来源：http://hz.gzhubu.top/gtckoxzfod.html

defaultdict(list)
来源：http://hz.guowangkeji.top/gtivovfvnd.html

[U15] Py：高精度计时
来源：http://hz.sufxvd.cn/gtmakhvldg.html

t = time.perf_counter()
来源：http://hz.ybcxt.top/gtsswpexnd.html

[U16] Py：命令行参数解析
来源：http://hz.jinqigfzy.top/gtbrnjnknb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.chenjidiqi.icu/gtmmtzxyyj.html

[U17] Py：初始化日志
来源：http://hz.sufxvd.cn/gtqefilamb.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.jinqigufen.top/gtmuompowc.html

[U18] Py：预编译正则
来源：http://hz.yueranfly.top/gtsjhzslmd.html

pat = re.compile(r"\d+")
来源：http://hz.zhongyouzk.top/gtcsmtqjiy.html

[U19] Py：正则替换带回调
来源：http://hz.aibaodan.cn/gtwyiagqln.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.smart0.xyz/gtsprhiamm.html

[U20] Py：缓存函数结果
来源：http://hz.hammf.cn/gtebasyvbx.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zdqjudy.top/gtrojdelui.html

[U21] Py：自定义上下文管理器
来源：http://hz.aibaodan.cn/gthvztbyfw.html

@contextlib.contextmanager
来源：http://hz.daxiang520.top/gtlxmeuhlq.html

[U22] Py：矩阵转置
来源：http://hz.9152youxi.cn/gtslrcuygf.html

list(zip(*m))
来源：http://hz.sysykeji.top/gtxkwiifsw.html

[U23] Py：分块读取大文件
来源：http://hz.yvedp.cn/gtcqbtjirx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.c1oappe.top/gtxlwsyssa.html

[U24] Py：路径操作
来源：http://hz.jyoumei.cn/gtqfqfcrci.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.jqgfzy.top/gtfyflqqzl.html

[U25] Py：CSV 按字典读
来源：http://hz.yj20258.top/gtnwypfwbu.html

csv.DictReader(f)
来源：http://hz.zhengqikj.top/gtwoopjncd.html

[U26] Py：并发下载
来源：http://hz.guowangkeji.top/gtmhoyfcry.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.dianchejie.cn/gtwzjlgbfi.html

[U27] Py：异步 HTTP
来源：http://hz.nwbrower.top/gtntwcfmbn.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.cheryme.top/gtocwnaiay.html

[U28] Py：类型别名
来源：http://hz.sysykeji.top/gtocbnjefl.html

UserId = int
来源：http://hz.bjfxy.top/gtztksqfzh.html

[U29] Py：属性校验
来源：http://hz.redwolf501.top/gtgwtdkjxl.html

@property 与 @x.setter 配合
来源：http://hz.nwbrower.top/gtmazladik.html

[U30] Py：数据类
来源：http://hz.gzhubu.top/gtgngiqvtp.html

@dataclass(slots=True)
来源：http://hz.zhijiandao.cn/gtyunqqihd.html

[U31] Py：单测
来源：http://hz.xingfuxueyuan.xyz/gtbcrnpplu.html

python -m pytest -q
来源：http://hz.sweek.top/gtmzdsotvp.html

[U32] Py：代码格式化
来源：http://hz.quarkkingdee.top/gtzpjigqwe.html

ruff format . && ruff check --fix .
来源：http://hz.yanxiufei.cn/gtzbnzfzlb.html

[U33] Py：打包发布
来源：http://hz.daxiang520.top/gtjqhxlegi.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.zhixingplan.top/gtgroaxdfm.html

[U34] Py：判断编码
来源：http://hz.xingfuxueyuan.xyz/gtbwnlallr.html

chardet.detect(raw)
来源：http://hz.nwbrower.top/gtajvawnhq.html

[U35] Py：发送邮件
来源：http://hz.meibo888.top/gtsdphhjjd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.dianchejie.cn/gtadzwigch.html

[U36] Py：定时任务
来源：http://hz.c1oappe.top/gtebsepssd.html

schedule.every(10).minutes.do(job)
来源：http://hz.tanke756.top/gtpacuupsp.html


<!-- 参考信息 -->