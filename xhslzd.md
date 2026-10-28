代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yvedp.cn/gtzakbzhov.html

[S08] C：动态内存分配与释放
来源：http://hz.wangdashe.top/gtdkvxecor.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.tian-w.cn/gtgbllytrq.html

[S09] C：结构体定义与初始化
来源：http://hz.nanxuanxn.top/gtvgqvnmxh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yangfankeji.com/gtjrzoqger.html

[S10] C：指针与解引用
来源：http://hz.zhijiandao.cn/gtugnjtlld.html

int *p = &a;  *p = 5;
来源：http://hz.xinyue.icu/gtxtlrbytj.html

[S11] C：逐行读文件
来源：http://hz.xziqi.cn/gtvdhkxleq.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.wangshuangyany.cn/gtsfgwctta.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.shangyingyoupin.top/gtaeobnuef.html

fclose(f);
来源：http://hz.cucudq.cn/gtlqgoskla.html

[S12] C：写文件
来源：http://hz.cashguo.top/gtylxczsvi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jinqigufen.top/gtimvypsol.html

[S13] C：宏定义
来源：http://hz.mhx1999.top/gtriofxvth.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.nwbrower.top/gtlwjmdklf.html

[S14] C：枚举
来源：http://hz.wangshuangyany.cn/gtntjhmmbc.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.sysykeji.top/gtbkivrdhb.html

[S15] C：类型转换
来源：http://hz.hfpthk.cn/gtexywukrh.html

(double) a / b
来源：http://hz.hongshengwenyu.top/gtmrahoech.html

[S16] C：位操作置位
来源：http://hz.zhiwuduotai.top/gtgcdpsxhf.html

x |= (1 << 3);
来源：http://hz.ybcxt.top/gthnubhcuf.html

[S17] C：安全拼接字符串
来源：http://hz.bjfxy.top/gtfbuvofed.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.bjfxy.top/gtsdnlipiq.html

[S18] C：命令行参数
来源：http://hz.xylfe.cn/gtoxertixk.html

int main(int argc, char **argv)
来源：http://hz.feifeiyinyue.top/gtinkhtvbj.html

[S19] C：快速排序
来源：http://hz.ehwqpu.com/gtqptjpaqh.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shangyingyoupin.top/gtttkhoucl.html

[S20] C：二分查找
来源：http://hz.xinyue.icu/gtzogyqgih.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhijiandao.cn/gthwtyowxc.html

[S21] C：字符类别判断
来源：http://hz.xinyue.icu/gtwzbkubyt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jinyuanbaomall.cn/gthyimlzys.html

[S22] C：字符串转数字
来源：http://hz.chenzaomai.com/gtxfkwsuln.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yuanzhike.top/gtjhgbeadz.html

[S23] C：随机数
来源：http://hz.xinyue.icu/gtzlxxiwdl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.52xcode.cn/gtyidjcmjg.html

[S24] C：获取本地时间
来源：http://hz.meibo888.top/gtibzwmako.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hywenlv.cn/gttiecmvno.html

[S25] C：内存拷贝
来源：http://hz.xziqi.cn/gtcrbfpvzr.html

memcpy(dst, src, n);
来源：http://hz.ydzc1.top/gtqwdqvbmq.html

[S26] C：内存清零
来源：http://hz.jqgfzy.top/gtomvfslwj.html

memset(a, 0, sizeof a);
来源：http://hz.ivvv.top/gtcfomswrv.html

[S27] C：定义常量
来源：http://hz.jyoumei.cn/gthfwxgvpc.html

const double PI = 3.14159;
来源：http://hz.pycfn.com/gtxaxxkdwr.html

[S28] C：静态变量
来源：http://hz.meibo888.top/gtjbotyzym.html

static int counter = 0;
来源：http://hz.jlsjyb.cn/gtcvonsduy.html

[S29] C：变参函数
来源：http://hz.0kj1m.cn/gtnczmcnlv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.shanyushiyangkeji.top/gtcgksxptp.html

[S30] C：头文件保护
来源：http://hz.xuetiantiany.cn/gtzjcdjufu.html

#ifndef X_H
来源：http://hz.guannengcc.top/gthggcprfn.html

#define X_H
来源：http://hz.zhoulong.xyz/gtrcjljyqc.html

#endif
来源：http://hz.cdnleiting.top/gtkccborfp.html

[S31] C++：Hello World
来源：http://hz.pycfn.com/gtllimvfpw.html

#include <iostream>
来源：http://hz.hongshengwenyu.top/gtxlxmfkwa.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.nanxuanxn.top/gtnvwvyxdi.html

[S32] C++：字符串
来源：http://hz.zhongyouzk.top/gtqlirikzj.html

std::string s = "hi";  s += "!";
来源：http://hz.mhx1999.top/gtzcdekgba.html

[S33] C++：vector 增删
来源：http://hz.yueranfly.top/gtwisgfwvr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.havefunace.top/gtumcovrkp.html

[S34] C++：遍历 vector
来源：http://hz.daxiang520.top/gterbdiqzm.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.smart0.xyz/gthzwgctrg.html

[S35] C++：map
来源：http://hz.hysaishi.cn/gtgiaazofx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hammf.cn/gtcdrfmawp.html

[S36] C++：unordered_map
来源：http://hz.shzxlz.cn/gtglgkadoi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ppjwa.cn/gtjiuddmvn.html

[S37] C++：set
来源：http://hz.ybcxt.top/gttxxnrxem.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.iojbl.cn/gtsmmdzdvs.html

[S38] C++：排序
来源：http://hz.shzxlz.cn/gtloywcuri.html

std::sort(v.begin(), v.end());
来源：http://hz.xingfuxueyuan.xyz/gtcqwffugn.html

[S39] C++：自定义比较器排序
来源：http://hz.jqgfzy.top/gtgbkpdihn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hnxiangtu.top/gtfgwdgpwf.html

[S40] C++：查找元素
来源：http://hz.52xcode.cn/gtiruurozv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.cheryme.top/gtffvpthag.html

[S41] C++：类与构造函数
来源：http://hz.0kj1m.cn/gttuibtaqb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ydjk.org.cn/gtwakblnkq.html

[S42] C++：继承与虚函数
来源：http://hz.xziqi.cn/gtxqvrmccz.html

class B : public Base { public: void f() override {} };
来源：http://hz.hongshengwenyu.top/gtzmzbgedg.html

[S43] C++：智能指针
来源：http://hz.xuetiantiany.cn/gtwloipeyv.html

auto p = std::make_unique<int>(5);
来源：http://hz.hnqzz.top/gtoyfgepol.html

[S44] C++：引用传参
来源：http://hz.jianghu66.top/gtorakbahr.html

void inc(int &x) { ++x; }
来源：http://hz.ivvv.top/gtmpuuoasj.html

[S45] C++：lambda
来源：http://hz.mhx1999.top/gtnhloxlgo.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.guowangkeji.top/gtslehtzmw.html

[S46] C++：函数模板
来源：http://hz.meibo888.top/gtlcozhexy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yanxiufei.cn/gtavfthiin.html

[S47] C++：结构化绑定遍历
来源：http://hz.yj20258.top/gtbeqgsgjj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhoulong.xyz/gtxeeawgmq.html

[S48] C++：逐行读文件
来源：http://hz.chenjidiqi.icu/gtfcfasejj.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhijiandao.cn/gtmnqcugcr.html

while (std::getline(in, line)) { }
来源：http://hz.yj202588.top/gtxfgmubuf.html

[S49] C++：写文件
来源：http://hz.pengpengdd.cyou/gtgrlkrxlk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ppjwa.cn/gtclevjffm.html

[S50] C++：格式化数字
来源：http://hz.nanxuanxn.top/gtdyscwegj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jinqigufen.top/gtxxqwdcxp.html

[S51] C++：显式类型转换
来源：http://hz.nanxinkj.top/gtrprtxkgo.html

static_cast<double>(a) / b
来源：http://hz.pycfn.com/gtzxaimpna.html

[S52] C++：const 与 noexcept
来源：http://hz.jqgufenzy.top/gtujpdhgrr.html

int size() const noexcept { return n_; }
来源：http://hz.ppjwa.cn/gtfoftowon.html

[S53] C++：移动语义
来源：http://hz.nanxuanxn.top/gtvkffzcrs.html

std::vector<int> w = std::move(v);
来源：http://hz.gotoacloud.top/gtuhwakdbn.html

[S54] C++：异常处理
来源：http://hz.chenlongwang.top/gtqqbakylv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhoulong.xyz/gtaoyionje.html

[S55] C++：结构化绑定
来源：http://hz.aizwys.cn/gttbfrmodd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.9152youxi.cn/gtvjswqhbv.html

[S56] C++：optional
来源：http://hz.vqdsnc.cn/gtpdkmomch.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.0kj1m.cn/gtcigupoga.html

[S57] C++：编译期常量
来源：http://hz.shzxlz.cn/gtummyrfml.html

constexpr int N = 10;
来源：http://hz.wangdashe.top/gtkiiuqyvv.html

[S58] C++：命名空间
来源：http://hz.hammf.cn/gtathftoln.html

namespace ns { int f() { return 1; } }
来源：http://hz.ivvv.top/gtrxytmpzf.html

[S59] C++：静态断言
来源：http://hz.yueranfly.top/gtjiywslfo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.fengsongda.top/gtetshvxcf.html

[S60] C++：遍历并删除元素
来源：http://hz.xuanzx.com/gtccsomyze.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.mhx1999.top/gtwyjqfqsz.html

================================================================================
来源：http://hz.ybcxt.top/gtdiyadnmr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.nanxuanxn.top/gtbtlxfbbr.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtwaszofmf.html

[T01] Kotlin：Hello World
来源：http://hz.sufxvd.cn/gtmfpeppzw.html

println("Hello")
来源：http://hz.tian-w.cn/gtorluueeo.html

[T02] Kotlin：变量
来源：http://hz.pycfn.com/gtkunnzrag.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.9152youxi.cn/gttrxkvumm.html

[T03] Kotlin：字符串模板
来源：http://hz.zycfv.cn/gtcawbjtsu.html

"值: $b"
来源：http://hz.guannengcc.top/gtcjvdukzk.html

[T04] Kotlin：空安全
来源：http://hz.hammf.cn/gtjsxlkhle.html

val n: String? = null;  n?.length
来源：http://hz.ydjk.org.cn/gtapsruqbt.html

[T05] Kotlin：when 表达式
来源：http://hz.zhaomingkeji.xyz/gtmtosudks.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.svipenyu.cn/gtvhknvrse.html

[T06] Kotlin：集合映射
来源：http://hz.daria6918.cn/gtjjttcchj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.wangdashe.top/gtbqatnebo.html

[T07] Kotlin：集合过滤
来源：http://hz.daria6918.cn/gtojffqsga.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.chenzaomai.com/gtgclmyarc.html

[T08] Kotlin：数据类
来源：http://hz.hysaishi.cn/gthlwcuyuo.html

data class User(val name: String, val age: Int)
来源：http://hz.cheryme.top/gtwhugwhou.html

[T09] Kotlin：扩展函数
来源：http://hz.nwbrower.top/gtbfwkquao.html

fun String.exclaim() = this + "!"
来源：http://hz.hywenlv.cn/gtchsesfbo.html

[T10] Kotlin：默认参数
来源：http://hz.jiagoushi.top/gtzylvfdjs.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.wangdashe.top/gtkgqulnxz.html

[T11] Kotlin：协程
来源：http://hz.ydzc1.top/gtnhovikyf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.nanxuanxn.top/gtwlksjuhv.html

[T12] Kotlin：解构声明
来源：http://hz.zhongyouzk.top/gtmzzpeugl.html

val (a, b) = Pair(1, 2)
来源：http://hz.yonumen.top/gtdaemfcen.html

[T13] Kotlin：只读 Map
来源：http://hz.hnxiangtu.top/gtqphhpmmh.html

val m = mapOf("a" to 1)
来源：http://hz.316326.xyz/gtcvtkskls.html

[T14] Kotlin：循环
来源：http://hz.wangshuangyany.cn/gtaiszdjdc.html

for (i in 1..10) println(i)
来源：http://hz.0kj1m.cn/gtxdreymqd.html

[T15] Kotlin：接口
来源：http://hz.yj20258.top/gtevlewnfv.html

interface Shape { fun area(): Double }
来源：http://hz.xinyue.icu/gtlufyrwfw.html

[T16] Swift：Hello World
来源：http://hz.wangdashe.top/gtcszoxyyr.html

print("Hello")
来源：http://hz.shanyushiyangtech.top/gtvmdiqhgt.html

[T17] Swift：变量与常量
来源：http://hz.daxiang520.top/gtftfoiueb.html

var a = 1;  let b = 2
来源：http://hz.hnxiangtu.top/gtvsuacxom.html

[T18] Swift：字符串插值
来源：http://hz.jinghuilouyu.cn/gtxfubrkig.html

"值: \(b)"
来源：http://hz.zhaomingkeji.xyz/gtbwxeknty.html

[T19] Swift：可选绑定
来源：http://hz.aizwys.cn/gtynwpyavf.html

if let n = opt { print(n) }
来源：http://hz.aibaodan.cn/gtkgvtpudi.html

[T20] Swift：数组操作
来源：http://hz.pycfn.com/gtjaauessd.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zhengqikj.top/gteiyxaisg.html

[T21] Swift：遍历
来源：http://hz.wangdashe.top/gtutfidizn.html

for x in a { print(x) }
来源：http://hz.aizwys.cn/gtifurbwbq.html

[T22] Swift：字典
来源：http://hz.hnqzz.top/gtbotfglvx.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.iojbl.cn/gtppkbqaiv.html

[T23] Swift：函数
来源：http://hz.fzhhl.top/gthetgenqo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.shzxlz.cn/gtkqpmbfia.html

[T24] Swift：闭包
来源：http://hz.yj20258.top/gtxzsxzsgo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.xylfe.cn/gtotchjqai.html

[T25] Swift：结构体
来源：http://hz.xziqi.cn/gtexnmlioj.html

struct P { var x: Int }
来源：http://hz.ywan-chungtsiang.top/gttuxwvsnv.html

[T26] Swift：类与重写
来源：http://hz.feifeiyinyue.top/gtpjlkgdcu.html

class A: Base { override func f() {} }
来源：http://hz.gzhubu.top/gtdrbfcuii.html

[T27] Swift：错误处理
来源：http://hz.jiagoushi.top/gtlfukjvyo.html

do { try f() } catch { print(error) }
来源：http://hz.ehwqpu.com/gtwitnypoa.html

[T28] Swift：枚举
来源：http://hz.cheryme.top/gtcgddeffy.html

enum Color { case red, green }
来源：http://hz.hammf.cn/gtkjfcxkkh.html

[T29] Swift：guard 提前返回
来源：http://hz.shuidangran.top/gtaexabyji.html

guard let x = opt else { return }
来源：http://hz.aizwys.cn/gtpcuhcmpv.html

[T30] Swift：协议
来源：http://hz.vqdsnc.cn/gtbtmtcrol.html

protocol Shape { func area() -> Double }
来源：http://hz.yj202588.top/gtovplxnao.html

[T31] Lua：Hello World
来源：http://hz.zhixingplan.top/gtfrknklns.html

print("Hello")
来源：http://hz.sysykeji.top/gtobrhaidv.html

[T32] Lua：局部变量
来源：http://hz.fzhhl.top/gtjftxwrvk.html

local a = 1
来源：http://hz.jiagoushi.top/gtuwozucpy.html

[T33] Lua：表（数组）
来源：http://hz.hnqzz.top/gtfnwnslrl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.daria6918.cn/gtyxsuqwmg.html

[T34] Lua：遍历表
来源：http://hz.yuanzhike.top/gtnrjvudkj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.nanxuanxn.top/gtbewmibao.html

[T35] Lua：字典表
来源：http://hz.zhaomingkeji.xyz/gtemimvevz.html

local d = { a = 1 };  d.b = 2
来源：http://hz.hywenlv.cn/gtgfpcecde.html

[T36] Lua：函数
来源：http://hz.cdnleiting.top/gtopizhwos.html

function add(a, b) return a + b end
来源：http://hz.zhongyouzk.top/gtezjtvnid.html

[T37] Lua：字符串拼接
来源：http://hz.jqgfzy.top/gtqztlvqzg.html

"a" .. "b"
来源：http://hz.ywan-chungtsiang.top/gtpflbqjwn.html

[T38] Lua：条件
来源：http://hz.cucudq.cn/gtnytjdmik.html

if x > 0 then print("正") end
来源：http://hz.ppjwa.cn/gtslvptcav.html

[T39] Lua：模式匹配
来源：http://hz.wangdashe.top/gtazhhbyey.html

string.find(s, "%d+")
来源：http://hz.pycfn.com/gtjhaijfoy.html

[T40] Lua：元表
来源：http://hz.dashuyun.cn/gtfrtwwgrt.html

setmetatable({}, { __index = base })
来源：http://hz.zhaomingkeji.xyz/gtrgbufwav.html

[T41] Perl：Hello World
来源：http://hz.zhengqikj.top/gtguewyolk.html

print "Hello\n";
来源：http://hz.haohaochexian.top/gtihwpdynb.html

[T42] Perl：变量类型
来源：http://hz.ehwqpu.com/gtmyszbvin.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.hysaishi.cn/gtfmwnhszr.html

[T43] Perl：字符串插值
来源：http://hz.xuetiantiany.cn/gtllhxayty.html

"值: $a"
来源：http://hz.tanke756.top/gtkycdwwkf.html

[T44] Perl：条件
来源：http://hz.guannengcc.top/gtpfbmixec.html

if ($a > 0) { print "正"; }
来源：http://hz.jinqigfzy.top/gtulfozcnf.html

[T45] Perl：数组遍历
来源：http://hz.redwolf501.top/gtasxflewh.html

for my $x (@arr) { print $x; }
来源：http://hz.hywenlv.cn/gtoglvcfhm.html

[T46] Perl：哈希操作
来源：http://hz.zhoulong.xyz/gtqoqcqoko.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.shanyushiyangkeji.top/gtgthrkkhf.html

[T47] Perl：正则捕获
来源：http://hz.nanxinkj.top/gtwhwmskhj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.sweek.top/gtnvpgaqyy.html

[T48] Perl：正则替换
来源：http://hz.smart0.xyz/gtnmzmlbqv.html

$s =~ s/old/new/g;
来源：http://hz.meibo888.top/gtmmjwkwaa.html

[T49] Perl：函数
来源：http://hz.hysaishi.cn/gtlhbfdnbw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.nanxinkj.top/gtkisuwxin.html

[T50] Perl：逐行读文件
来源：http://hz.meibo888.top/gtnzqcswfg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.316326.xyz/gtepzzpyul.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jinqigufen.top/gtbgaehdrk.html

[T51] Scala：Hello World
来源：http://hz.ppjwa.cn/gttdogbfyv.html

println("Hello")
来源：http://hz.guannengcc.top/gtoshjvtop.html

[T52] Scala：变量
来源：http://hz.fengsongda.top/gtpugtyyka.html

val a = 1;  var b = 2
来源：http://hz.cucudq.cn/gtrzhtcsmp.html

[T53] Scala：字符串插值
来源：http://hz.tianlin.xyz/gtulgvmuce.html

s"值: $b"
来源：http://hz.cheryme.top/gtfilyqwrx.html

[T54] Scala：集合映射
来源：http://hz.shanyushiyangkeji.top/gtvotcrwye.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.iojbl.cn/gtuhligvav.html

[T55] Scala：集合过滤
来源：http://hz.52xcode.cn/gtwijjdlad.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.316326.xyz/gtbofoodlg.html

[T56] Scala：样例类
来源：http://hz.jinqigfzy.top/gtlcudrjyg.html

case class User(name: String, age: Int)
来源：http://hz.hammf.cn/gtzkmqzujp.html

[T57] Scala：模式匹配
来源：http://hz.zhiwuduotai.top/gtdsuefxvd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.gotoacloud.top/gtjxsoeieu.html

[T58] Scala：函数定义
来源：http://hz.redwolf501.top/gtuoxqonbo.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jlsjyb.cn/gtvinzvpoi.html

[T59] Scala：循环
来源：http://hz.yonumen.top/gtwcqvyyip.html

for (i <- 1 to 10) println(i)
来源：http://hz.ybcxt.top/gtmfspdrdq.html

[T60] Scala：折叠
来源：http://hz.iojbl.cn/gtlxfyjnzi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.zhongyouzk.top/gtoaeetqmu.html

================================================================================
来源：http://hz.yj20258888.top/gtxpwqvixa.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhoulong.xyz/gtcfbuisnz.html

================================================================================
来源：http://hz.hnqzz.top/gthvxywfza.html

[U01] Py：创建虚拟环境
来源：http://hz.shanyushiyangtech.top/gtdixqouxo.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.pycfn.com/gtdhitgorx.html

[U02] Py：导出 / 安装依赖
来源：http://hz.xuetiantiany.cn/gtoesfxyky.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.nanxinkj.top/gtbjmurgyl.html

[U03] Py：加载 .env 配置
来源：http://hz.gaohongyu789.top/gtmjuukkye.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.gzhubu.top/gtsstzsnef.html

[U04] Py：变量调试打印
来源：http://hz.smart0.xyz/gtlgsfxssc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.sysykeji.top/gteznffojf.html

[U05] Py：列表去重且保序
来源：http://hz.fengsongda.top/gtnpkhpxqc.html

list(dict.fromkeys(arr))
来源：http://hz.gzhubu.top/gtnmlgntyz.html

[U06] Py：合并两个字典
来源：http://hz.mhx1999.top/gtmbtotrts.html

{**a, **b}
来源：http://hz.hongshengwenyu.top/gtlfacetat.html

[U07] Py：反转字典键值
来源：http://hz.zhongyouzk.top/gtwzaqmdbl.html

{v: k for k, v in d.items()}
来源：http://hz.smart0.xyz/gtvnvjcbgn.html

[U08] Py：展平二维列表
来源：http://hz.yueranfly.top/gtpjqqtcsr.html

[y for x in nested for y in x]
来源：http://hz.xziqi.cn/gtreveowqp.html

[U09] Py：字典取最大值的键
来源：http://hz.hywenlv.cn/gtwxrjcibj.html

max(d, key=d.get)
来源：http://hz.chenlongwang.top/gtpvdjxinv.html

[U10] Py：按值排序字典
来源：http://hz.sysykeji.top/gtndszjcsl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yj20258888.top/gttkiywtwy.html

[U11] Py：生成器表达式
来源：http://hz.zhaomingkeji.xyz/gtudpyznxc.html

(x * 2 for x in arr)
来源：http://hz.hammf.cn/gtrrgnfdrr.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.chenzaomai.com/gtjhlarkdn.html

Counter(arr).most_common(3)
来源：http://hz.guannengcc.top/gtsacoxttt.html

[U13] Py：固定长度队列
来源：http://hz.snrcjt.cn/gtfffbtwxr.html

deque(maxlen=10)
来源：http://hz.zhengqikj.top/gtyjfqdmrp.html

[U14] Py：分组收集到列表
来源：http://hz.zhengqikj.top/gtooqsgtvm.html

defaultdict(list)
来源：http://hz.zhiwuduotai.top/gtndberkqd.html

[U15] Py：高精度计时
来源：http://hz.yonumen.top/gtakapzyam.html

t = time.perf_counter()
来源：http://hz.jinqigufen.top/gtlhpylkpz.html

[U16] Py：命令行参数解析
来源：http://hz.chenlongwang.top/gtwmhcuomv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.birdmap.top/gtwasgtbkd.html

[U17] Py：初始化日志
来源：http://hz.cashguo.top/gtxbqkftjk.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.jinghuilouyu.cn/gtuphauwdk.html

[U18] Py：预编译正则
来源：http://hz.bjfxy.top/gthzjmpqry.html

pat = re.compile(r"\d+")
来源：http://hz.hywenlv.cn/gtebeezlck.html

[U19] Py：正则替换带回调
来源：http://hz.zhaomingkeji.xyz/gtrfoqheyq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.daxiang520.top/gtmavspihn.html

[U20] Py：缓存函数结果
来源：http://hz.yuxming.cn/gteyvfvsmo.html

@functools.lru_cache(maxsize=None)
来源：http://hz.daria6918.cn/gtyksjjtpx.html

[U21] Py：自定义上下文管理器
来源：http://hz.sweek.top/gtckuulgnk.html

@contextlib.contextmanager
来源：http://hz.gaohongyu789.top/gtkezoimqd.html

[U22] Py：矩阵转置
来源：http://hz.0kj1m.cn/gtrbmrioqd.html

list(zip(*m))
来源：http://hz.feifeiyinyue.top/gtitqqxhrr.html

[U23] Py：分块读取大文件
来源：http://hz.bjfxy.top/gtkczvmwdz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.gotoacloud.top/gtbgtfchpt.html

[U24] Py：路径操作
来源：http://hz.zhiwuduotai.top/gtbmvvmymz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.sysykeji.top/gtxunkktxg.html

[U25] Py：CSV 按字典读
来源：http://hz.zhijiandao.cn/gtyuygijif.html

csv.DictReader(f)
来源：http://hz.jinyuanbaomall.cn/gtvutfyfsk.html

[U26] Py：并发下载
来源：http://hz.tianlin.xyz/gtkmghxnzg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.ydjk.org.cn/gtjmxfgctv.html

[U27] Py：异步 HTTP
来源：http://hz.jinyuanbaomall.cn/gtchmsgmdu.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.feifeiyinyue.top/gtcznpfrps.html

[U28] Py：类型别名
来源：http://hz.nanxinkj.top/gtywtbfnws.html

UserId = int
来源：http://hz.iojbl.cn/gtabgagmon.html

[U29] Py：属性校验
来源：http://hz.chenlongwang.top/gtowxlsson.html

@property 与 @x.setter 配合
来源：http://hz.dianchejie.cn/gtlogmsvnd.html

[U30] Py：数据类
来源：http://hz.zhiwuduotai.top/gtkistqwdu.html

@dataclass(slots=True)
来源：http://hz.iojbl.cn/gtckyjffvn.html


<!-- 参考信息 -->