代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://hz.jlsjyb.cn/gtwsrjesin.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.shanyushiyangkeji.top/gtorikmyqt.html

fclose(f);
来源：http://hz.snrcjt.cn/gtvdlnvngo.html

[S12] C：写文件
来源：http://hz.andypj.xyz/gtfczsiidf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.birdmap.top/gttyhwdckw.html

[S13] C：宏定义
来源：http://hz.316326.xyz/gtwlkvwjqw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jinqigufen.top/gtvxwsgjps.html

[S14] C：枚举
来源：http://hz.ppjwa.cn/gtxkxszesk.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.wangshuangyany.cn/gttgdyrbrz.html

[S15] C：类型转换
来源：http://hz.gogol.net.cn/gtmuybufxb.html

(double) a / b
来源：http://hz.yuxming.cn/gtgckohhtr.html

[S16] C：位操作置位
来源：http://hz.havefunace.top/gtmfgjtxtx.html

x |= (1 << 3);
来源：http://hz.ydjk.org.cn/gtoncdwgsy.html

[S17] C：安全拼接字符串
来源：http://hz.cucudq.cn/gtabsnccbb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xingfuxueyuan.xyz/gtegmjvyie.html

[S18] C：命令行参数
来源：http://hz.hywenlv.cn/gtrfczsscf.html

int main(int argc, char **argv)
来源：http://hz.hfpthk.cn/gtfonerqat.html

[S19] C：快速排序
来源：http://hz.fengsongda.top/gtpgojapqe.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.cheryme.top/gtfgfmzlgr.html

[S20] C：二分查找
来源：http://hz.xingfuxueyuan.xyz/gtcebwqvsg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hfpthk.cn/gtdtxpvaki.html

[S21] C：字符类别判断
来源：http://hz.redwolf501.top/gtulffhsus.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.birdmap.top/gtxltfvudi.html

[S22] C：字符串转数字
来源：http://hz.xinyue.icu/gtxvtzoegx.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.chenlongwang.top/gtcsjiyqmf.html

[S23] C：随机数
来源：http://hz.jiagoushi.top/gtkczcmosu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhaomingkeji.xyz/gteglbbbsm.html

[S24] C：获取本地时间
来源：http://hz.gotoacloud.top/gtbinamtid.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yj20258.top/gtusombdrb.html

[S25] C：内存拷贝
来源：http://hz.shuidangran.top/gtzyfirxmq.html

memcpy(dst, src, n);
来源：http://hz.hongshengwenyu.top/gtmmcektvc.html

[S26] C：内存清零
来源：http://hz.sufxvd.cn/gtxgvqgstw.html

memset(a, 0, sizeof a);
来源：http://hz.xuetiantiany.cn/gtwzhvttub.html

[S27] C：定义常量
来源：http://hz.hammf.cn/gtqzjsrnln.html

const double PI = 3.14159;
来源：http://hz.jinghuilouyu.cn/gtbrnvrful.html

[S28] C：静态变量
来源：http://hz.ydzc1.top/gtgmbtmcpw.html

static int counter = 0;
来源：http://hz.hysaishi.cn/gtwkquvexb.html

[S29] C：变参函数
来源：http://hz.zhiwuduotai.top/gtevxwgxcl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.snrcjt.cn/gtnvndrdll.html

[S30] C：头文件保护
来源：http://hz.ydjk.org.cn/gtxuhzydpd.html

#ifndef X_H
来源：http://hz.ivvv.top/gtzbctfbpm.html

#define X_H
来源：http://hz.shzxlz.cn/gtgkamhegf.html

#endif
来源：http://hz.chenlongwang.top/gtzqpxvced.html

[S31] C++：Hello World
来源：http://hz.xingfuxueyuan.xyz/gtsbwveagn.html

#include <iostream>
来源：http://hz.vqdsnc.cn/gtrodagknh.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.tian-w.cn/gtagvklsim.html

[S32] C++：字符串
来源：http://hz.xziqi.cn/gtelmkuory.html

std::string s = "hi";  s += "!";
来源：http://hz.sweek.top/gtipnewqxo.html

[S33] C++：vector 增删
来源：http://hz.9152youxi.cn/gtxgbytkkj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.dianchejie.cn/gteokxnics.html

[S34] C++：遍历 vector
来源：http://hz.xziqi.cn/gtgzzizzkh.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jinqigufen.top/gtsbvtrlyu.html

[S35] C++：map
来源：http://hz.ydzc1.top/gtrpukvcwp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xuanzx.com/gtovskklvm.html

[S36] C++：unordered_map
来源：http://hz.wangshuangyany.cn/gtwtrvyiij.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hammf.cn/gtdkdhnkzb.html

[S37] C++：set
来源：http://hz.ehwqpu.com/gtfcdfwkas.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.52xcode.cn/gtegmcfjyh.html

[S38] C++：排序
来源：http://hz.wangdashe.top/gtfsygkvop.html

std::sort(v.begin(), v.end());
来源：http://hz.nanxinkj.top/gtudetizkc.html

[S39] C++：自定义比较器排序
来源：http://hz.xinyue.icu/gtsxrttihu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.shuidangran.top/gtibevlydf.html

[S40] C++：查找元素
来源：http://hz.xinyue.icu/gtxltiavfv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jqgufenzy.top/gtyjfdyaqf.html

[S41] C++：类与构造函数
来源：http://hz.quarkkingdee.top/gtlvtnnswi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yj20258888.top/gtzrpgrigi.html

[S42] C++：继承与虚函数
来源：http://hz.xinyue.icu/gtoadlwdlf.html

class B : public Base { public: void f() override {} };
来源：http://hz.smart0.xyz/gthawxhxdm.html

[S43] C++：智能指针
来源：http://hz.wangdashe.top/gtigiyelve.html

auto p = std::make_unique<int>(5);
来源：http://hz.316326.xyz/gtuzcvvfdt.html

[S44] C++：引用传参
来源：http://hz.quarkkingdee.top/gtajknrsae.html

void inc(int &x) { ++x; }
来源：http://hz.nanxinkj.top/gttvqzylyo.html

[S45] C++：lambda
来源：http://hz.xylfe.cn/gtrysvzjfq.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhaomingkeji.xyz/gtehysyvbg.html

[S46] C++：函数模板
来源：http://hz.xuanzx.com/gtqojewtbp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.haohaochexian.top/gtjmqejmno.html

[S47] C++：结构化绑定遍历
来源：http://hz.ivvv.top/gtmykeqzyw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.daria6918.cn/gtzavurrns.html

[S48] C++：逐行读文件
来源：http://hz.gaohongyu789.top/gtqdysmmhb.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.cucudq.cn/gtthlyqatl.html

while (std::getline(in, line)) { }
来源：http://hz.sxryk.cn/gtzrfawbcg.html

[S49] C++：写文件
来源：http://hz.shangyingyoupin.top/gtcuprtuqi.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.mhx1999.top/gtnhozohhg.html

[S50] C++：格式化数字
来源：http://hz.haohaochexian.top/gttkmecrst.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.cashguo.top/gtbeyenlam.html

[S51] C++：显式类型转换
来源：http://hz.dashuyun.cn/gtnnjieopo.html

static_cast<double>(a) / b
来源：http://hz.havefunace.top/gtmpyyfdhl.html

[S52] C++：const 与 noexcept
来源：http://hz.smart0.xyz/gtvrkkvwjw.html

int size() const noexcept { return n_; }
来源：http://hz.sysykeji.top/gtctaguruw.html

[S53] C++：移动语义
来源：http://hz.xziqi.cn/gthljooccn.html

std::vector<int> w = std::move(v);
来源：http://hz.nwbrower.top/gthispcelo.html

[S54] C++：异常处理
来源：http://hz.52xcode.cn/gtzbylcyvy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yongpay.top/gtojqhyscy.html

[S55] C++：结构化绑定
来源：http://hz.hfpthk.cn/gtibhfxpmw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.chenjidiqi.icu/gtmciolwjc.html

[S56] C++：optional
来源：http://hz.redwolf501.top/gtlfkvgljr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.gzhubu.top/gtwzhmaptc.html

[S57] C++：编译期常量
来源：http://hz.xylfe.cn/gtrdytlhka.html

constexpr int N = 10;
来源：http://hz.zhiwuduotai.top/gtcadugcha.html

[S58] C++：命名空间
来源：http://hz.shanyushiyangkeji.top/gtjwjuzagy.html

namespace ns { int f() { return 1; } }
来源：http://hz.0kj1m.cn/gtylncylqk.html

[S59] C++：静态断言
来源：http://hz.xylfe.cn/gtkwwacryz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ybcxt.top/gtamwitlof.html

[S60] C++：遍历并删除元素
来源：http://hz.chenjidiqi.icu/gtvfkgbsrm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zdqjudy.top/gtoqtofful.html

================================================================================
来源：http://hz.ydjk.org.cn/gtwbamuyai.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.9152youxi.cn/gtltcvycjq.html

================================================================================
来源：http://hz.andypj.xyz/gtzbefbujm.html

[T01] Kotlin：Hello World
来源：http://hz.bjfxy.top/gtiodjttgr.html

println("Hello")
来源：http://hz.andypj.xyz/gtynzrclah.html

[T02] Kotlin：变量
来源：http://hz.xingfuxueyuan.xyz/gtybrgwwow.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.wangshuangyany.cn/gtyjdgtyor.html

[T03] Kotlin：字符串模板
来源：http://hz.ppjwa.cn/gtcnzmoapo.html

"值: $b"
来源：http://hz.nanxinkj.top/gtmkoztrsx.html

[T04] Kotlin：空安全
来源：http://hz.birdmap.top/gtiywogcnz.html

val n: String? = null;  n?.length
来源：http://hz.yuxming.cn/gtucrfdfia.html

[T05] Kotlin：when 表达式
来源：http://hz.shanyushiyangkeji.top/gtxnnfxdwm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.guowangkeji.top/gtbrrdenqu.html

[T06] Kotlin：集合映射
来源：http://hz.smart0.xyz/gtelzgfuvp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.gotoacloud.top/gthwijdbhc.html

[T07] Kotlin：集合过滤
来源：http://hz.pycfn.com/gthderdutk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.sufxvd.cn/gttmhoavwv.html

[T08] Kotlin：数据类
来源：http://hz.9152youxi.cn/gtlddujpin.html

data class User(val name: String, val age: Int)
来源：http://hz.haohaochexian.top/gtlcinwfvr.html

[T09] Kotlin：扩展函数
来源：http://hz.kuanghao11.cn/gttuaksfrt.html

fun String.exclaim() = this + "!"
来源：http://hz.gaohongyu789.top/gtxpumhqjb.html

[T10] Kotlin：默认参数
来源：http://hz.sxryk.cn/gtbiacohce.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.xuanzx.com/gtibxjzhgr.html

[T11] Kotlin：协程
来源：http://hz.pycfn.com/gtdbxxsexc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jinqigufen.top/gtmbooebue.html

[T12] Kotlin：解构声明
来源：http://hz.jianghu66.top/gtziducozw.html

val (a, b) = Pair(1, 2)
来源：http://hz.ydzc1.top/gthimuteiy.html

[T13] Kotlin：只读 Map
来源：http://hz.yj202588.top/gtoahekrlv.html

val m = mapOf("a" to 1)
来源：http://hz.cdnleiting.top/gtalpruxhg.html

[T14] Kotlin：循环
来源：http://hz.guowangkeji.top/gtiedullzu.html

for (i in 1..10) println(i)
来源：http://hz.zhixingplan.top/gtubmfeygm.html

[T15] Kotlin：接口
来源：http://hz.yueranfly.top/gtqnjwmpbe.html

interface Shape { fun area(): Double }
来源：http://hz.jyoumei.cn/gtjikhjowx.html

[T16] Swift：Hello World
来源：http://hz.shzxlz.cn/gtuvitonis.html

print("Hello")
来源：http://hz.meibo888.top/gtnlzfwqxv.html

[T17] Swift：变量与常量
来源：http://hz.iojbl.cn/gtwnlzdjer.html

var a = 1;  let b = 2
来源：http://hz.ehwqpu.com/gtdrzzlvfv.html

[T18] Swift：字符串插值
来源：http://hz.quarkkingdee.top/gtgisapnzl.html

"值: \(b)"
来源：http://hz.chenjidiqi.icu/gtumasbvwh.html

[T19] Swift：可选绑定
来源：http://hz.gogol.net.cn/gtvpadyaza.html

if let n = opt { print(n) }
来源：http://hz.hywenlv.cn/gtjyuxnlla.html

[T20] Swift：数组操作
来源：http://hz.0kj1m.cn/gtwwhskcdg.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.bjfxy.top/gtiouygjwb.html

[T21] Swift：遍历
来源：http://hz.zhixingplan.top/gtvzuirgvm.html

for x in a { print(x) }
来源：http://hz.ivvv.top/gtqtbnwdrq.html

[T22] Swift：字典
来源：http://hz.sysykeji.top/gtmfumlnqc.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.shangyingyoupin.top/gtfaiwdrax.html

[T23] Swift：函数
来源：http://hz.yuxming.cn/gttwtvmwan.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.sysykeji.top/gtphwciyno.html

[T24] Swift：闭包
来源：http://hz.havefunace.top/gtpbspeqew.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.shanyushiyangkeji.top/gtnycpuesc.html

[T25] Swift：结构体
来源：http://hz.kuanghao11.cn/gtvzizoacb.html

struct P { var x: Int }
来源：http://hz.yj20258.top/gtzdolxyjj.html

[T26] Swift：类与重写
来源：http://hz.gzhubu.top/gtiivrittv.html

class A: Base { override func f() {} }
来源：http://hz.cheryme.top/gtauufmfzd.html

[T27] Swift：错误处理
来源：http://hz.zhijiandao.cn/gtfnxsffcq.html

do { try f() } catch { print(error) }
来源：http://hz.hnqzz.top/gtfantdsts.html

[T28] Swift：枚举
来源：http://hz.xylfe.cn/gtfyqxszbu.html

enum Color { case red, green }
来源：http://hz.yj20258888.top/gtduwdvznh.html

[T29] Swift：guard 提前返回
来源：http://hz.shanyushiyangkeji.top/gtudscpnzl.html

guard let x = opt else { return }
来源：http://hz.yueranfly.top/gtfinhbuom.html

[T30] Swift：协议
来源：http://hz.wangshuangyany.cn/gtdvkqklaq.html

protocol Shape { func area() -> Double }
来源：http://hz.shanyushiyangtech.top/gtkjrvpgbo.html

[T31] Lua：Hello World
来源：http://hz.hysaishi.cn/gtaxiiknzv.html

print("Hello")
来源：http://hz.yj202588.top/gtdfhklifc.html

[T32] Lua：局部变量
来源：http://hz.sysykeji.top/gttfsnshvj.html

local a = 1
来源：http://hz.xinyue.icu/gtvnzbkkoo.html

[T33] Lua：表（数组）
来源：http://hz.feifeiyinyue.top/gtyszrffqe.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yangfankeji.com/gtcocqwgkc.html

[T34] Lua：遍历表
来源：http://hz.cqqwz.cn/gtjtzsllgw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.gotoacloud.top/gttiulsekj.html

[T35] Lua：字典表
来源：http://hz.guowangkeji.top/gtdxoezvou.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yanxiufei.cn/gtozzuyzfj.html

[T36] Lua：函数
来源：http://hz.kuanghao11.cn/gtbfvqvvxh.html

function add(a, b) return a + b end
来源：http://hz.yvedp.cn/gtwjfdjsgg.html

[T37] Lua：字符串拼接
来源：http://hz.ydzc1.top/gtsuvnrsvk.html

"a" .. "b"
来源：http://hz.hnqzz.top/gthkycadbf.html

[T38] Lua：条件
来源：http://hz.birdmap.top/gtfceegfxo.html

if x > 0 then print("正") end
来源：http://hz.xylfe.cn/gtrmtsjxtj.html

[T39] Lua：模式匹配
来源：http://hz.quarkkingdee.top/gtlllxcpaa.html

string.find(s, "%d+")
来源：http://hz.ydjk.org.cn/gtfjcptkaq.html

[T40] Lua：元表
来源：http://hz.jiagoushi.top/gtzdlmzlxq.html

setmetatable({}, { __index = base })
来源：http://hz.shangyingyoupin.top/gtdgqbzxum.html

[T41] Perl：Hello World
来源：http://hz.hammf.cn/gtpoausrgb.html

print "Hello\n";
来源：http://hz.cashguo.top/gtytwhjugt.html

[T42] Perl：变量类型
来源：http://hz.316326.xyz/gtitvzotnz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zhijiandao.cn/gtwtylmndu.html

[T43] Perl：字符串插值
来源：http://hz.sysykeji.top/gtqetgxfah.html

"值: $a"
来源：http://hz.chenjidiqi.icu/gtmnzviewa.html

[T44] Perl：条件
来源：http://hz.hfpthk.cn/gtfrldbwyy.html

if ($a > 0) { print "正"; }
来源：http://hz.yuxming.cn/gtrcugkbhc.html

[T45] Perl：数组遍历
来源：http://hz.gaohongyu789.top/gthiewwume.html

for my $x (@arr) { print $x; }
来源：http://hz.shuidangran.top/gtvuvyjusi.html

[T46] Perl：哈希操作
来源：http://hz.yonumen.top/gtuqvjqxrf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yueranfly.top/gtmilpchbu.html

[T47] Perl：正则捕获
来源：http://hz.nanxinkj.top/gtjbyymwjg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.daxiang520.top/gtmtksmkhk.html

[T48] Perl：正则替换
来源：http://hz.daria6918.cn/gtjjhcyesm.html

$s =~ s/old/new/g;
来源：http://hz.52xcode.cn/gtjhfytdin.html

[T49] Perl：函数
来源：http://hz.wangdashe.top/gtbxktibeo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zhongyouzk.top/gtkyfjqtco.html

[T50] Perl：逐行读文件
来源：http://hz.zhoulong.xyz/gtrtbohkvt.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.nanxinkj.top/gtafadrkff.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.xuetiantiany.cn/gtndwtfaoe.html

[T51] Scala：Hello World
来源：http://hz.tian-w.cn/gtsglhfonc.html

println("Hello")
来源：http://hz.tian-w.cn/gtofpuuezr.html

[T52] Scala：变量
来源：http://hz.snrcjt.cn/gtpsibcyph.html

val a = 1;  var b = 2
来源：http://hz.sweek.top/gtdjtzpmdx.html

[T53] Scala：字符串插值
来源：http://hz.yvedp.cn/gtwhjahvli.html

s"值: $b"
来源：http://hz.wangdashe.top/gtlrjtyeeo.html

[T54] Scala：集合映射
来源：http://hz.sweek.top/gtoezmlyve.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.316326.xyz/gtrzoysztk.html

[T55] Scala：集合过滤
来源：http://hz.zdqjudy.top/gtzhekpieu.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.zycfv.cn/gtwjicwzyr.html

[T56] Scala：样例类
来源：http://hz.snrcjt.cn/gtokdufkoh.html

case class User(name: String, age: Int)
来源：http://hz.havefunace.top/gtczidgduq.html

[T57] Scala：模式匹配
来源：http://hz.316326.xyz/gtnvfrkere.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.xuanzx.com/gtmartehnw.html

[T58] Scala：函数定义
来源：http://hz.zhiwuduotai.top/gthzffnqho.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yvedp.cn/gtlcqpufpx.html

[T59] Scala：循环
来源：http://hz.smart0.xyz/gtcqbzoifz.html

for (i <- 1 to 10) println(i)
来源：http://hz.kuanghao11.cn/gtmdjzdnsq.html

[T60] Scala：折叠
来源：http://hz.guannengcc.top/gtnrizxczj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.jqgufenzy.top/gtwzyweqzl.html

================================================================================
来源：http://hz.bjfxy.top/gtgehwrfom.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jiagoushi.top/gtyydmbsup.html

================================================================================
来源：http://hz.guannengcc.top/gtzjnrstnb.html

[U01] Py：创建虚拟环境
来源：http://hz.havefunace.top/gtprxwxipw.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.svipenyu.cn/gtllhcedyd.html

[U02] Py：导出 / 安装依赖
来源：http://hz.pycfn.com/gtcaebsryu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.gzhubu.top/gtpyvukybb.html

[U03] Py：加载 .env 配置
来源：http://hz.zdqjudy.top/gtdcomfnwq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jinghuilouyu.cn/gtmxwkiuky.html

[U04] Py：变量调试打印
来源：http://hz.zdqjudy.top/gtccnvqilx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yueranfly.top/gtwsjpeuao.html

[U05] Py：列表去重且保序
来源：http://hz.hysaishi.cn/gtuvnjtvdv.html

list(dict.fromkeys(arr))
来源：http://hz.gzhubu.top/gtszyrosjd.html

[U06] Py：合并两个字典
来源：http://hz.bjfxy.top/gtfxmpbtyt.html

{**a, **b}
来源：http://hz.gogol.net.cn/gtcjwsdqrq.html

[U07] Py：反转字典键值
来源：http://hz.yvedp.cn/gtefbaskdr.html

{v: k for k, v in d.items()}
来源：http://hz.jinqigfzy.top/gtmwvfdbzt.html

[U08] Py：展平二维列表
来源：http://hz.jinqigfzy.top/gtjiqdsbtw.html

[y for x in nested for y in x]
来源：http://hz.ywan-chungtsiang.top/gtrkgxiggd.html

[U09] Py：字典取最大值的键
来源：http://hz.smart0.xyz/gtgitnxnpp.html

max(d, key=d.get)
来源：http://hz.vqdsnc.cn/gtaquweusk.html

[U10] Py：按值排序字典
来源：http://hz.xingfuxueyuan.xyz/gtwlpaporf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.xingfuxueyuan.xyz/gtpspzylor.html

[U11] Py：生成器表达式
来源：http://hz.0kj1m.cn/gtfpiieypl.html

(x * 2 for x in arr)
来源：http://hz.birdmap.top/gtzmxzihui.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.birdmap.top/gtrskkbwwo.html

Counter(arr).most_common(3)
来源：http://hz.xuanzx.com/gtosbzxdnk.html

[U13] Py：固定长度队列
来源：http://hz.zhixingplan.top/gtvmceasoa.html

deque(maxlen=10)
来源：http://hz.jinqigfzy.top/gtroqvohjj.html

[U14] Py：分组收集到列表
来源：http://hz.yanxiufei.cn/gtedabjeok.html

defaultdict(list)
来源：http://hz.aibaodan.cn/gtuafzlhkz.html

[U15] Py：高精度计时
来源：http://hz.zhongyouzk.top/gtbhwifdoo.html

t = time.perf_counter()
来源：http://hz.ybcxt.top/gtbxrusxul.html

[U16] Py：命令行参数解析
来源：http://hz.bjfxy.top/gthftgtuup.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.feifeiyinyue.top/gtejqnwvbz.html

[U17] Py：初始化日志
来源：http://hz.andypj.xyz/gtcgbwkipo.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.xinyue.icu/gtxfwtcbta.html

[U18] Py：预编译正则
来源：http://hz.hywenlv.cn/gtspozxdvu.html

pat = re.compile(r"\d+")
来源：http://hz.ydjk.org.cn/gtvdpscjqk.html

[U19] Py：正则替换带回调
来源：http://hz.nanxuanxn.top/gtclxuusfy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yonumen.top/gtlsezrmfl.html

[U20] Py：缓存函数结果
来源：http://hz.snrcjt.cn/gtodtkhzzr.html

@functools.lru_cache(maxsize=None)
来源：http://hz.shzxlz.cn/gtwgtzyawx.html

[U21] Py：自定义上下文管理器
来源：http://hz.wangdashe.top/gtbkvayury.html

@contextlib.contextmanager
来源：http://hz.sufxvd.cn/gthdjnnrsn.html

[U22] Py：矩阵转置
来源：http://hz.hfpthk.cn/gtrtjaolzn.html

list(zip(*m))
来源：http://hz.fengsongda.top/gteybfaodh.html

[U23] Py：分块读取大文件
来源：http://hz.sysykeji.top/gttinsqaho.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.hysaishi.cn/gtypmxsbcr.html

[U24] Py：路径操作
来源：http://hz.pengpengdd.cyou/gtvydvhasq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.0kj1m.cn/gthekjijcp.html

[U25] Py：CSV 按字典读
来源：http://hz.cheryme.top/gtmscbealy.html

csv.DictReader(f)
来源：http://hz.zdqjudy.top/gtimsqovxj.html

[U26] Py：并发下载
来源：http://hz.sufxvd.cn/gtcaylayqg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.hnxiangtu.top/gtjnovylcw.html

[U27] Py：异步 HTTP
来源：http://hz.gotoacloud.top/gtfxxnvrlz.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.iojbl.cn/gtasaikqju.html

[U28] Py：类型别名
来源：http://hz.cashguo.top/gtzqfhznms.html

UserId = int
来源：http://hz.gzhubu.top/gthsetedoa.html

[U29] Py：属性校验
来源：http://hz.zhiwuduotai.top/gtxwjtysbe.html

@property 与 @x.setter 配合
来源：http://hz.yueranfly.top/gtyunfhgcv.html

[U30] Py：数据类
来源：http://hz.jinyuanbaomall.cn/gtovgpspom.html

@dataclass(slots=True)
来源：http://hz.sweek.top/gtsyzqmcbq.html

[U31] Py：单测
来源：http://hz.ppjwa.cn/gtkpjbpaan.html

python -m pytest -q
来源：http://hz.chenlongwang.top/gtggpfmlbb.html

[U32] Py：代码格式化
来源：http://hz.cqqwz.cn/gtkatpyhih.html

ruff format . && ruff check --fix .
来源：http://hz.yanxiufei.cn/gtqneogdfv.html

[U33] Py：打包发布
来源：http://hz.sxryk.cn/gtaghhopmp.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.hnqzz.top/gtojgrthel.html

[U34] Py：判断编码
来源：http://hz.sysykeji.top/gtfprfmqwc.html

chardet.detect(raw)
来源：http://hz.ppjwa.cn/gtizsjlaqg.html


<!-- 参考信息 -->