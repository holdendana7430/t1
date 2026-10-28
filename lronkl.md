代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.shangyingyoupin.top/gtyjgihfjf.html

[S10] C：指针与解引用
来源：http://hz.shanyushiyangtech.top/gtgupsczdg.html

int *p = &a;  *p = 5;
来源：http://hz.gotoacloud.top/gtaibbrpsr.html

[S11] C：逐行读文件
来源：http://hz.daria6918.cn/gtwysxloln.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yuanzhike.top/gtecbzclpr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ywan-chungtsiang.top/gtcwfzmeaq.html

fclose(f);
来源：http://hz.52xcode.cn/gtzjbquxpe.html

[S12] C：写文件
来源：http://hz.zhoulong.xyz/gtsxuvktgd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yj20258.top/gtygqainzj.html

[S13] C：宏定义
来源：http://hz.zhijiandao.cn/gtxnlzitkd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.guowangkeji.top/gthlaxclfj.html

[S14] C：枚举
来源：http://hz.havefunace.top/gtfxuteznu.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ivvv.top/gtwxulhbhw.html

[S15] C：类型转换
来源：http://hz.gotoacloud.top/gtiokanwgl.html

(double) a / b
来源：http://hz.xingfuxueyuan.xyz/gtfvibvaaj.html

[S16] C：位操作置位
来源：http://hz.316326.xyz/gtvnuxdwgp.html

x |= (1 << 3);
来源：http://hz.xuanzx.com/gtbjjfcsqk.html

[S17] C：安全拼接字符串
来源：http://hz.wangdashe.top/gtfkoizewl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.hfpthk.cn/gtypxwfnbl.html

[S18] C：命令行参数
来源：http://hz.gogol.net.cn/gtmkkipxbt.html

int main(int argc, char **argv)
来源：http://hz.ppjwa.cn/gtbnfumwhn.html

[S19] C：快速排序
来源：http://hz.feifeiyinyue.top/gtqivbzjql.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.havefunace.top/gtdmwzrdmr.html

[S20] C：二分查找
来源：http://hz.nanxuanxn.top/gtxvswgnqo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ydjk.org.cn/gtprqjzclf.html

[S21] C：字符类别判断
来源：http://hz.zhixingplan.top/gtsorqestv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.shuidangran.top/gtdgacwiyx.html

[S22] C：字符串转数字
来源：http://hz.mhx1999.top/gtoqrhjvmk.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zycfv.cn/gtjawvcluk.html

[S23] C：随机数
来源：http://hz.zhaomingkeji.xyz/gtuqdsuhfi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.fengsongda.top/gtpiojavaa.html

[S24] C：获取本地时间
来源：http://hz.ehwqpu.com/gtpjqenalf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xuanzx.com/gtcfudimvm.html

[S25] C：内存拷贝
来源：http://hz.9152youxi.cn/gtlrxldlbt.html

memcpy(dst, src, n);
来源：http://hz.cdnleiting.top/gtabqfblqe.html

[S26] C：内存清零
来源：http://hz.wangdashe.top/gtnlxortua.html

memset(a, 0, sizeof a);
来源：http://hz.sxryk.cn/gterkavuyw.html

[S27] C：定义常量
来源：http://hz.xylfe.cn/gteboeoixt.html

const double PI = 3.14159;
来源：http://hz.fengsongda.top/gttynleksh.html

[S28] C：静态变量
来源：http://hz.zhijiandao.cn/gtdavptvli.html

static int counter = 0;
来源：http://hz.vqdsnc.cn/gtpszpyzul.html

[S29] C：变参函数
来源：http://hz.mhx1999.top/gtehpqenlh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.shuidangran.top/gtsglbrdec.html

[S30] C：头文件保护
来源：http://hz.zhixingplan.top/gtzdjswsyx.html

#ifndef X_H
来源：http://hz.cheryme.top/gttgloiynu.html

#define X_H
来源：http://hz.sxryk.cn/gtdgppcwfx.html

#endif
来源：http://hz.xinyue.icu/gtwbyxsseg.html

[S31] C++：Hello World
来源：http://hz.nanxinkj.top/gttllsvzoc.html

#include <iostream>
来源：http://hz.yj202588.top/gtmtcosjzz.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jinqigfzy.top/gtinykpmwy.html

[S32] C++：字符串
来源：http://hz.svipenyu.cn/gtyzsfliqz.html

std::string s = "hi";  s += "!";
来源：http://hz.sxryk.cn/gttizouryb.html

[S33] C++：vector 增删
来源：http://hz.ehwqpu.com/gtceheikgt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.pycfn.com/gtqpduhfav.html

[S34] C++：遍历 vector
来源：http://hz.quarkkingdee.top/gtdkmvgfmc.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yueranfly.top/gtuexlylia.html

[S35] C++：map
来源：http://hz.yonumen.top/gtltmnbnrh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nanxuanxn.top/gtdpkaxfyo.html

[S36] C++：unordered_map
来源：http://hz.gzhubu.top/gtrhkeuffn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.birdmap.top/gtnqfbyycq.html

[S37] C++：set
来源：http://hz.chenjidiqi.icu/gtizrnmzwe.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.tianlin.xyz/gthivpkaqq.html

[S38] C++：排序
来源：http://hz.wangshuangyany.cn/gtnujrslnr.html

std::sort(v.begin(), v.end());
来源：http://hz.hysaishi.cn/gtqdnuszkn.html

[S39] C++：自定义比较器排序
来源：http://hz.ywan-chungtsiang.top/gtwtnjhwen.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yj20258.top/gtitldznwy.html

[S40] C++：查找元素
来源：http://hz.c1oappe.top/gtsoahsuve.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yj202588.top/gtdrrkbuzz.html

[S41] C++：类与构造函数
来源：http://hz.snrcjt.cn/gtvhplcmur.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhengqikj.top/gtlleflgba.html

[S42] C++：继承与虚函数
来源：http://hz.mhx1999.top/gtqrnacwbt.html

class B : public Base { public: void f() override {} };
来源：http://hz.xinyue.icu/gtbauwbynz.html

[S43] C++：智能指针
来源：http://hz.yueranfly.top/gthviaptgb.html

auto p = std::make_unique<int>(5);
来源：http://hz.jinqigfzy.top/gtqicfxorw.html

[S44] C++：引用传参
来源：http://hz.yvedp.cn/gtrwbjobbi.html

void inc(int &x) { ++x; }
来源：http://hz.hysaishi.cn/gtgmrcnyur.html

[S45] C++：lambda
来源：http://hz.dianchejie.cn/gtczqwolfx.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.birdmap.top/gtccqmfvar.html

[S46] C++：函数模板
来源：http://hz.ydzc1.top/gtigvrtysh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shanyushiyangkeji.top/gtzhbudjec.html

[S47] C++：结构化绑定遍历
来源：http://hz.316326.xyz/gtxguwdjra.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jinqigfzy.top/gtgbcikxsw.html

[S48] C++：逐行读文件
来源：http://hz.shangyingyoupin.top/gtmbrijtqr.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.daxiang520.top/gtqmafeehi.html

while (std::getline(in, line)) { }
来源：http://hz.zhiwuduotai.top/gtecjujxwh.html

[S49] C++：写文件
来源：http://hz.guannengcc.top/gtubzpdglp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.xingfuxueyuan.xyz/gtynaiyteb.html

[S50] C++：格式化数字
来源：http://hz.xingfuxueyuan.xyz/gtqrkmnmim.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.smart0.xyz/gtjcaqjyju.html

[S51] C++：显式类型转换
来源：http://hz.ydjk.org.cn/gtusoahmjg.html

static_cast<double>(a) / b
来源：http://hz.jianghu66.top/gtamxgkywi.html

[S52] C++：const 与 noexcept
来源：http://hz.shangyingyoupin.top/gtkmfjtidu.html

int size() const noexcept { return n_; }
来源：http://hz.cashguo.top/gtgxeaxscr.html

[S53] C++：移动语义
来源：http://hz.wangdashe.top/gtksddsmpi.html

std::vector<int> w = std::move(v);
来源：http://hz.sweek.top/gtmvtuxlcb.html

[S54] C++：异常处理
来源：http://hz.hnqzz.top/gtomcvdwsv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhijiandao.cn/gtaezfplzq.html

[S55] C++：结构化绑定
来源：http://hz.wangdashe.top/gtzvjebqqw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhaomingkeji.xyz/gtsdurtkwi.html

[S56] C++：optional
来源：http://hz.gzhubu.top/gtvujkoxue.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.chenlongwang.top/gtvidgztxj.html

[S57] C++：编译期常量
来源：http://hz.xinyue.icu/gtsranhtbo.html

constexpr int N = 10;
来源：http://hz.cashguo.top/gtgzlganrs.html

[S58] C++：命名空间
来源：http://hz.fzhhl.top/gtbllixcwe.html

namespace ns { int f() { return 1; } }
来源：http://hz.xylfe.cn/gtecipywab.html

[S59] C++：静态断言
来源：http://hz.aibaodan.cn/gtmwsljbgt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jyoumei.cn/gtnezvgelq.html

[S60] C++：遍历并删除元素
来源：http://hz.xuetiantiany.cn/gtweyqgznb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.cucudq.cn/gtnkhrchqr.html

================================================================================
来源：http://hz.chenlongwang.top/gtorvsprgm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ydjk.org.cn/gtwowsickd.html

================================================================================
来源：http://hz.yueranfly.top/gttsxnugcu.html

[T01] Kotlin：Hello World
来源：http://hz.xingfuxueyuan.xyz/gthahhmwln.html

println("Hello")
来源：http://hz.hfpthk.cn/gtfbcmggma.html

[T02] Kotlin：变量
来源：http://hz.hongshengwenyu.top/gtulccryav.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhixingplan.top/gtgqhyafop.html

[T03] Kotlin：字符串模板
来源：http://hz.wangdashe.top/gtarzuuqxx.html

"值: $b"
来源：http://hz.svipenyu.cn/gtuwhxykrs.html

[T04] Kotlin：空安全
来源：http://hz.jinghuilouyu.cn/gtkapaukuf.html

val n: String? = null;  n?.length
来源：http://hz.fzhhl.top/gtpwkpmwct.html

[T05] Kotlin：when 表达式
来源：http://hz.xuanzx.com/gtqimngqeo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.cdnleiting.top/gtqcilwuko.html

[T06] Kotlin：集合映射
来源：http://hz.smart0.xyz/gtpulzvhqt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yanxiufei.cn/gtvvcwfzfx.html

[T07] Kotlin：集合过滤
来源：http://hz.hywenlv.cn/gtsyjejarp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.shanyushiyangtech.top/gtsleqfwyn.html

[T08] Kotlin：数据类
来源：http://hz.yanxiufei.cn/gtlejjhhxg.html

data class User(val name: String, val age: Int)
来源：http://hz.smart0.xyz/gtnyriiqgp.html

[T09] Kotlin：扩展函数
来源：http://hz.hnxiangtu.top/gtcgmitlnz.html

fun String.exclaim() = this + "!"
来源：http://hz.aibaodan.cn/gtnbdxqaoo.html

[T10] Kotlin：默认参数
来源：http://hz.vqdsnc.cn/gtzzlqazen.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ivvv.top/gtiizbmecx.html

[T11] Kotlin：协程
来源：http://hz.zhixingplan.top/gtaedbvqcq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zhengqikj.top/gtfubozisg.html

[T12] Kotlin：解构声明
来源：http://hz.redwolf501.top/gttnvlloyj.html

val (a, b) = Pair(1, 2)
来源：http://hz.haohaochexian.top/gtwdgzjdch.html

[T13] Kotlin：只读 Map
来源：http://hz.nwbrower.top/gtmkvbhves.html

val m = mapOf("a" to 1)
来源：http://hz.ivvv.top/gtqxuyoypd.html

[T14] Kotlin：循环
来源：http://hz.jlsjyb.cn/gtqvzapmct.html

for (i in 1..10) println(i)
来源：http://hz.wangshuangyany.cn/gtyfgajcli.html

[T15] Kotlin：接口
来源：http://hz.xinyue.icu/gtatpjdtxs.html

interface Shape { fun area(): Double }
来源：http://hz.nanxinkj.top/gtiltwytdv.html

[T16] Swift：Hello World
来源：http://hz.ehwqpu.com/gtcubgnrog.html

print("Hello")
来源：http://hz.birdmap.top/gtkmizoifz.html

[T17] Swift：变量与常量
来源：http://hz.jinqigfzy.top/gtnfojqrxn.html

var a = 1;  let b = 2
来源：http://hz.shzxlz.cn/gtpxwjvesm.html

[T18] Swift：字符串插值
来源：http://hz.chenzaomai.com/gtyycjtzry.html

"值: \(b)"
来源：http://hz.xinyue.icu/gtxdhvnumx.html

[T19] Swift：可选绑定
来源：http://hz.hnqzz.top/gtyagihmuh.html

if let n = opt { print(n) }
来源：http://hz.hnxiangtu.top/gtlddxlkxq.html

[T20] Swift：数组操作
来源：http://hz.hysaishi.cn/gtvwnmcdgt.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.sweek.top/gtmwsmordz.html

[T21] Swift：遍历
来源：http://hz.quarkkingdee.top/gttdcrpfzs.html

for x in a { print(x) }
来源：http://hz.vqdsnc.cn/gtbbwnlrke.html

[T22] Swift：字典
来源：http://hz.hywenlv.cn/gtbiesgvpg.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.shuidangran.top/gtaiuplpql.html

[T23] Swift：函数
来源：http://hz.yuxming.cn/gtoyjjpuvm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ehwqpu.com/gtabaipljm.html

[T24] Swift：闭包
来源：http://hz.zhaomingkeji.xyz/gteaqerlbf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.xylfe.cn/gttlmpximi.html

[T25] Swift：结构体
来源：http://hz.chenjidiqi.icu/gtahfjetrj.html

struct P { var x: Int }
来源：http://hz.yvedp.cn/gtlxybaaya.html

[T26] Swift：类与重写
来源：http://hz.iojbl.cn/gtuhlsktlb.html

class A: Base { override func f() {} }
来源：http://hz.bjfxy.top/gtfqqhkkxm.html

[T27] Swift：错误处理
来源：http://hz.shzxlz.cn/gtmebqbqts.html

do { try f() } catch { print(error) }
来源：http://hz.hfpthk.cn/gtgsqflpax.html

[T28] Swift：枚举
来源：http://hz.52xcode.cn/gtqhfpkkwk.html

enum Color { case red, green }
来源：http://hz.hongshengwenyu.top/gtgzjiqsiz.html

[T29] Swift：guard 提前返回
来源：http://hz.chenjidiqi.icu/gttxoupdqc.html

guard let x = opt else { return }
来源：http://hz.tian-w.cn/gtbioklvfk.html

[T30] Swift：协议
来源：http://hz.ehwqpu.com/gtziylghkk.html

protocol Shape { func area() -> Double }
来源：http://hz.yvedp.cn/gtywykqopc.html

[T31] Lua：Hello World
来源：http://hz.pengpengdd.cyou/gttkovzrzh.html

print("Hello")
来源：http://hz.0kj1m.cn/gtumqiimha.html

[T32] Lua：局部变量
来源：http://hz.dianchejie.cn/gtlwclviwk.html

local a = 1
来源：http://hz.ydjk.org.cn/gtdfugenpk.html

[T33] Lua：表（数组）
来源：http://hz.52xcode.cn/gtemkkwwhn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.xziqi.cn/gtkqaeiugm.html

[T34] Lua：遍历表
来源：http://hz.cdnleiting.top/gtqzyyprwa.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.gzhubu.top/gtrkhytoss.html

[T35] Lua：字典表
来源：http://hz.havefunace.top/gtbvlvawdl.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jinghuilouyu.cn/gtwppdbgkc.html

[T36] Lua：函数
来源：http://hz.mhx1999.top/gttiuqwokr.html

function add(a, b) return a + b end
来源：http://hz.mhx1999.top/gtaqewryrz.html

[T37] Lua：字符串拼接
来源：http://hz.gotoacloud.top/gtdwednzvx.html

"a" .. "b"
来源：http://hz.gogol.net.cn/gtorkmnnjz.html

[T38] Lua：条件
来源：http://hz.tianlin.xyz/gtgepwhrww.html

if x > 0 then print("正") end
来源：http://hz.c1oappe.top/gtptvgbriq.html

[T39] Lua：模式匹配
来源：http://hz.cqqwz.cn/gtwftisalg.html

string.find(s, "%d+")
来源：http://hz.shangyingyoupin.top/gtwbgmitbg.html

[T40] Lua：元表
来源：http://hz.pycfn.com/gtjfckoaxc.html

setmetatable({}, { __index = base })
来源：http://hz.yvedp.cn/gtpbkknlwg.html

[T41] Perl：Hello World
来源：http://hz.gaohongyu789.top/gtqmiesjay.html

print "Hello\n";
来源：http://hz.yongpay.top/gtbrtpwmuy.html

[T42] Perl：变量类型
来源：http://hz.zhijiandao.cn/gtmdarfbqj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.smart0.xyz/gtssdhvjgz.html

[T43] Perl：字符串插值
来源：http://hz.yongpay.top/gtlzelxkca.html

"值: $a"
来源：http://hz.ybcxt.top/gtxykkissq.html

[T44] Perl：条件
来源：http://hz.yanxiufei.cn/gtpcpdzcof.html

if ($a > 0) { print "正"; }
来源：http://hz.0kj1m.cn/gtgwyzrbaq.html

[T45] Perl：数组遍历
来源：http://hz.ivvv.top/gtmitsbadt.html

for my $x (@arr) { print $x; }
来源：http://hz.snrcjt.cn/gttikwomij.html

[T46] Perl：哈希操作
来源：http://hz.yangfankeji.com/gtcqugcudc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.daria6918.cn/gtfnfaqjzi.html

[T47] Perl：正则捕获
来源：http://hz.gaohongyu789.top/gtgifecehy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.zhijiandao.cn/gthxkoaedu.html

[T48] Perl：正则替换
来源：http://hz.0kj1m.cn/gtmlskadwf.html

$s =~ s/old/new/g;
来源：http://hz.chenlongwang.top/gtwqlwziwe.html

[T49] Perl：函数
来源：http://hz.yvedp.cn/gtkcetezdo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.52xcode.cn/gtmvwjlwbk.html

[T50] Perl：逐行读文件
来源：http://hz.aibaodan.cn/gtvdepbkxg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.chenlongwang.top/gtfmedyjfo.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.xuanzx.com/gtzeeavtac.html

[T51] Scala：Hello World
来源：http://hz.snrcjt.cn/gtwzqtcuwc.html

println("Hello")
来源：http://hz.xziqi.cn/gtwuqaokzc.html

[T52] Scala：变量
来源：http://hz.cucudq.cn/gtivudrzrk.html

val a = 1;  var b = 2
来源：http://hz.andypj.xyz/gtzrnzjztf.html

[T53] Scala：字符串插值
来源：http://hz.wangdashe.top/gtteiyfmos.html

s"值: $b"
来源：http://hz.shanyushiyangkeji.top/gtuskslvzy.html

[T54] Scala：集合映射
来源：http://hz.jiagoushi.top/gtfrwtewuf.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.bjfxy.top/gtbzydqcka.html

[T55] Scala：集合过滤
来源：http://hz.fzhhl.top/gtghbaxsrb.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jqgufenzy.top/gtyyfdnqyt.html

[T56] Scala：样例类
来源：http://hz.hysaishi.cn/gtfwuqsjqt.html

case class User(name: String, age: Int)
来源：http://hz.jinqigfzy.top/gtzvdueacl.html

[T57] Scala：模式匹配
来源：http://hz.zhaomingkeji.xyz/gtfynwphzr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zhoulong.xyz/gtogdhwngl.html

[T58] Scala：函数定义
来源：http://hz.zhengqikj.top/gthdjuratc.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.shzxlz.cn/gtauyslsoh.html

[T59] Scala：循环
来源：http://hz.feifeiyinyue.top/gtumcrqebq.html

for (i <- 1 to 10) println(i)
来源：http://hz.cashguo.top/gtrqenduht.html

[T60] Scala：折叠
来源：http://hz.nanxuanxn.top/gtfsygkfgs.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.zycfv.cn/gthoyuondc.html

================================================================================
来源：http://hz.xziqi.cn/gtgskybnek.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.52xcode.cn/gtkpjtnylg.html

================================================================================
来源：http://hz.52xcode.cn/gtzxilfmek.html

[U01] Py：创建虚拟环境
来源：http://hz.0kj1m.cn/gtrapjxesp.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.jinghuilouyu.cn/gtqlojlqve.html

[U02] Py：导出 / 安装依赖
来源：http://hz.chenlongwang.top/gtgkspoxhs.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.shanyushiyangkeji.top/gtecdseitq.html

[U03] Py：加载 .env 配置
来源：http://hz.dashuyun.cn/gtasalsxpj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.ydjk.org.cn/gtcmkvajzb.html

[U04] Py：变量调试打印
来源：http://hz.jlsjyb.cn/gtrajnkvbd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jinghuilouyu.cn/gttwgylhps.html

[U05] Py：列表去重且保序
来源：http://hz.redwolf501.top/gtczjkfmkn.html

list(dict.fromkeys(arr))
来源：http://hz.daria6918.cn/gtfwlpnsnu.html

[U06] Py：合并两个字典
来源：http://hz.haohaochexian.top/gtedyamujk.html

{**a, **b}
来源：http://hz.cqqwz.cn/gtwfzbqczf.html

[U07] Py：反转字典键值
来源：http://hz.yj20258.top/gtwbhdkvap.html

{v: k for k, v in d.items()}
来源：http://hz.zhixingplan.top/gtnkgxffcc.html

[U08] Py：展平二维列表
来源：http://hz.bjfxy.top/gtsjaxsexk.html

[y for x in nested for y in x]
来源：http://hz.shangyingyoupin.top/gtxanivmwv.html

[U09] Py：字典取最大值的键
来源：http://hz.0kj1m.cn/gtinwvicji.html

max(d, key=d.get)
来源：http://hz.nanxinkj.top/gthwruxoot.html

[U10] Py：按值排序字典
来源：http://hz.yonumen.top/gtibwxvfan.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.gotoacloud.top/gtmsnzbnnr.html

[U11] Py：生成器表达式
来源：http://hz.shanyushiyangtech.top/gtzgfadwjo.html

(x * 2 for x in arr)
来源：http://hz.xylfe.cn/gtwkaevfde.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.cheryme.top/gtffnrbemw.html

Counter(arr).most_common(3)
来源：http://hz.zhoulong.xyz/gtorbntylo.html

[U13] Py：固定长度队列
来源：http://hz.andypj.xyz/gtqrnfhnwl.html

deque(maxlen=10)
来源：http://hz.jqgfzy.top/gtvzvlkoow.html

[U14] Py：分组收集到列表
来源：http://hz.dianchejie.cn/gtwtyjonwz.html

defaultdict(list)
来源：http://hz.chenlongwang.top/gtyrlynocp.html

[U15] Py：高精度计时
来源：http://hz.daxiang520.top/gtdzjluvjb.html

t = time.perf_counter()
来源：http://hz.jinyuanbaomall.cn/gtwuevayxn.html

[U16] Py：命令行参数解析
来源：http://hz.9152youxi.cn/gtistgcyef.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jqgufenzy.top/gtgbqjznvv.html

[U17] Py：初始化日志
来源：http://hz.shanyushiyangtech.top/gtjazzlbad.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yuanzhike.top/gtknjlzrfk.html

[U18] Py：预编译正则
来源：http://hz.zdqjudy.top/gtiiiukzov.html

pat = re.compile(r"\d+")
来源：http://hz.shuidangran.top/gtrlewsnfm.html

[U19] Py：正则替换带回调
来源：http://hz.tianlin.xyz/gthnucpfzs.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.tanke756.top/gtnepdnsbe.html

[U20] Py：缓存函数结果
来源：http://hz.iojbl.cn/gtnnrrkuyb.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jinghuilouyu.cn/gtlwssnsxc.html

[U21] Py：自定义上下文管理器
来源：http://hz.jiagoushi.top/gtkwdsklaf.html

@contextlib.contextmanager
来源：http://hz.xuanzx.com/gtbdakggsd.html

[U22] Py：矩阵转置
来源：http://hz.fzhhl.top/gthingfpva.html

list(zip(*m))
来源：http://hz.zhijiandao.cn/gtpjczuzwq.html

[U23] Py：分块读取大文件
来源：http://hz.shanyushiyangkeji.top/gtvlzzxziy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.tian-w.cn/gtyzyvnxdb.html

[U24] Py：路径操作
来源：http://hz.gzhubu.top/gtqdlziouq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.cqqwz.cn/gtjeqwgteu.html

[U25] Py：CSV 按字典读
来源：http://hz.jyoumei.cn/gtbxmykadm.html

csv.DictReader(f)
来源：http://hz.aibaodan.cn/gthelpdtyt.html

[U26] Py：并发下载
来源：http://hz.xylfe.cn/gtlwrtdhvd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.dianchejie.cn/gtevfqeaot.html

[U27] Py：异步 HTTP
来源：http://hz.zhiwuduotai.top/gttvksdprw.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.vqdsnc.cn/gtnpqnnset.html

[U28] Py：类型别名
来源：http://hz.hfpthk.cn/gtbaefbpfs.html

UserId = int
来源：http://hz.jianghu66.top/gtjkxkbfwz.html

[U29] Py：属性校验
来源：http://hz.shanyushiyangkeji.top/gtjcnqsmqc.html

@property 与 @x.setter 配合
来源：http://hz.yuxming.cn/gthdvlthnn.html

[U30] Py：数据类
来源：http://hz.yj20258888.top/gtdxilynnm.html

@dataclass(slots=True)
来源：http://hz.cqqwz.cn/gtysbjcuiy.html

[U31] Py：单测
来源：http://hz.ybcxt.top/gtfxfqtmvr.html

python -m pytest -q
来源：http://hz.316326.xyz/gthrgqdvou.html

[U32] Py：代码格式化
来源：http://hz.smart0.xyz/gteqkvnlst.html

ruff format . && ruff check --fix .
来源：http://hz.yuanzhike.top/gtkjqfvitd.html


<!-- 参考信息 -->