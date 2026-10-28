代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://hz.daxiang520.top/gtaqjkelnd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.aibaodan.cn/gtbivyqhxa.html

fclose(f);
来源：http://hz.ehwqpu.com/gtqjjssime.html

[S12] C：写文件
来源：http://hz.yuxming.cn/gthjealebi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xuetiantiany.cn/gtaevzmrcu.html

[S13] C：宏定义
来源：http://hz.nanxinkj.top/gtwdrvmaxn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ehwqpu.com/gttiqlauon.html

[S14] C：枚举
来源：http://hz.gotoacloud.top/gtqzpactzs.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.feifeiyinyue.top/gthgpmanzu.html

[S15] C：类型转换
来源：http://hz.nanxuanxn.top/gtetzrnqud.html

(double) a / b
来源：http://hz.chenzaomai.com/gtnuvjxghz.html

[S16] C：位操作置位
来源：http://hz.hnqzz.top/gtauhlarte.html

x |= (1 << 3);
来源：http://hz.yanxiufei.cn/gtyrlyscfa.html

[S17] C：安全拼接字符串
来源：http://hz.cqqwz.cn/gtvrudbdue.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.nanxinkj.top/gthsqpiyyw.html

[S18] C：命令行参数
来源：http://hz.jinyuanbaomall.cn/gtlhpfdxgc.html

int main(int argc, char **argv)
来源：http://hz.zhengqikj.top/gtdzybyxts.html

[S19] C：快速排序
来源：http://hz.gaohongyu789.top/gtoifmrhqs.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.daxiang520.top/gttxjipobn.html

[S20] C：二分查找
来源：http://hz.hammf.cn/gtbafrycur.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hongshengwenyu.top/gtcaiadnjo.html

[S21] C：字符类别判断
来源：http://hz.xuetiantiany.cn/gtebchpoml.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.tianlin.xyz/gtbnchplqy.html

[S22] C：字符串转数字
来源：http://hz.ybcxt.top/gtfiviuwbd.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.redwolf501.top/gtbyzvmxqy.html

[S23] C：随机数
来源：http://hz.birdmap.top/gticzuqipb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xingfuxueyuan.xyz/gtciyqsewk.html

[S24] C：获取本地时间
来源：http://hz.nanxinkj.top/gtqatlrcow.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jianghu66.top/gtxroknhww.html

[S25] C：内存拷贝
来源：http://hz.hongshengwenyu.top/gtxcaqjgtx.html

memcpy(dst, src, n);
来源：http://hz.cheryme.top/gtcoilrawv.html

[S26] C：内存清零
来源：http://hz.wangdashe.top/gtvexgqudc.html

memset(a, 0, sizeof a);
来源：http://hz.iojbl.cn/gtahjhcjlq.html

[S27] C：定义常量
来源：http://hz.jyoumei.cn/gtfgcrmzvq.html

const double PI = 3.14159;
来源：http://hz.dashuyun.cn/gtgrszjjxn.html

[S28] C：静态变量
来源：http://hz.feifeiyinyue.top/gtqufdkocy.html

static int counter = 0;
来源：http://hz.yanxiufei.cn/gtylzkamgz.html

[S29] C：变参函数
来源：http://hz.gzhubu.top/gtbcderiqg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yueranfly.top/gtizlnvhtf.html

[S30] C：头文件保护
来源：http://hz.jinghuilouyu.cn/gtfaqdskgp.html

#ifndef X_H
来源：http://hz.xziqi.cn/gtbfefnwby.html

#define X_H
来源：http://hz.wangdashe.top/gtrjnzaihf.html

#endif
来源：http://hz.sysykeji.top/gteyxobsms.html

[S31] C++：Hello World
来源：http://hz.jqgfzy.top/gttejziptb.html

#include <iostream>
来源：http://hz.jinqigfzy.top/gtzixqnsle.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zhoulong.xyz/gtakvbwuvd.html

[S32] C++：字符串
来源：http://hz.yonumen.top/gtlehebyzt.html

std::string s = "hi";  s += "!";
来源：http://hz.ppjwa.cn/gtcnohwgsa.html

[S33] C++：vector 增删
来源：http://hz.bjfxy.top/gtwvyrnevh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.nanxinkj.top/gtsipeqvnd.html

[S34] C++：遍历 vector
来源：http://hz.zhengqikj.top/gtatgkpnom.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yj20258888.top/gtgylpnmmo.html

[S35] C++：map
来源：http://hz.wangdashe.top/gtydhaeaky.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ydzc1.top/gtuusohhmo.html

[S36] C++：unordered_map
来源：http://hz.haohaochexian.top/gtmvvdegsm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hfpthk.cn/gtfrthydes.html

[S37] C++：set
来源：http://hz.vqdsnc.cn/gtjzbzbhit.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.meibo888.top/gtzlbcjcat.html

[S38] C++：排序
来源：http://hz.andypj.xyz/gtadnzvavi.html

std::sort(v.begin(), v.end());
来源：http://hz.zhongyouzk.top/gtjdknplnv.html

[S39] C++：自定义比较器排序
来源：http://hz.quarkkingdee.top/gthsfjjtsz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.birdmap.top/gttdzsucfg.html

[S40] C++：查找元素
来源：http://hz.chenlongwang.top/gtanekzjxj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.ehwqpu.com/gtskukobrs.html

[S41] C++：类与构造函数
来源：http://hz.tianlin.xyz/gtghpkhniu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xziqi.cn/gtzyidpdsi.html

[S42] C++：继承与虚函数
来源：http://hz.hongshengwenyu.top/gtifumprkg.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhengqikj.top/gtncpaukpk.html

[S43] C++：智能指针
来源：http://hz.quarkkingdee.top/gtaitadcvy.html

auto p = std::make_unique<int>(5);
来源：http://hz.xziqi.cn/gtgkiklaxp.html

[S44] C++：引用传参
来源：http://hz.jlsjyb.cn/gtofkzblko.html

void inc(int &x) { ++x; }
来源：http://hz.yj202588.top/gtggwsbaud.html

[S45] C++：lambda
来源：http://hz.hywenlv.cn/gtwygtiwzb.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hfpthk.cn/gtzkfykcgo.html

[S46] C++：函数模板
来源：http://hz.daria6918.cn/gtndybmswm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.smart0.xyz/gtetoelumh.html

[S47] C++：结构化绑定遍历
来源：http://hz.jinyuanbaomall.cn/gtvmoyylec.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.nanxinkj.top/gtctxshsfk.html

[S48] C++：逐行读文件
来源：http://hz.nwbrower.top/gtjqawxslj.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yueranfly.top/gtlkkearib.html

while (std::getline(in, line)) { }
来源：http://hz.zhaomingkeji.xyz/gtldojftbt.html

[S49] C++：写文件
来源：http://hz.0kj1m.cn/gtwfrurtvp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhaomingkeji.xyz/gtwcsmcyct.html

[S50] C++：格式化数字
来源：http://hz.svipenyu.cn/gtqwhvffhl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.fzhhl.top/gtesromcia.html

[S51] C++：显式类型转换
来源：http://hz.shanyushiyangtech.top/gtlaxporhf.html

static_cast<double>(a) / b
来源：http://hz.52xcode.cn/gtmcisqhux.html

[S52] C++：const 与 noexcept
来源：http://hz.shanyushiyangtech.top/gtupriqdwy.html

int size() const noexcept { return n_; }
来源：http://hz.sxryk.cn/gthjtliulo.html

[S53] C++：移动语义
来源：http://hz.sufxvd.cn/gtpfsnehfl.html

std::vector<int> w = std::move(v);
来源：http://hz.hysaishi.cn/gtkgjscsbn.html

[S54] C++：异常处理
来源：http://hz.hysaishi.cn/gtwxmeivdb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yvedp.cn/gtbncfbelm.html

[S55] C++：结构化绑定
来源：http://hz.hnqzz.top/gtnhhumukp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.kuanghao11.cn/gtqztzdnkh.html

[S56] C++：optional
来源：http://hz.cdnleiting.top/gtvpxsdyki.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.bjfxy.top/gtxclvqlkr.html

[S57] C++：编译期常量
来源：http://hz.zdqjudy.top/gtgkufduho.html

constexpr int N = 10;
来源：http://hz.guowangkeji.top/gtoprgxpqn.html

[S58] C++：命名空间
来源：http://hz.nanxuanxn.top/gthxecwlnx.html

namespace ns { int f() { return 1; } }
来源：http://hz.shangyingyoupin.top/gtfeunpvnt.html

[S59] C++：静态断言
来源：http://hz.zhijiandao.cn/gththpzooz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.aibaodan.cn/gtdmisntcg.html

[S60] C++：遍历并删除元素
来源：http://hz.yj20258.top/gtfxosuygb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jqgufenzy.top/gtdfguwzwi.html

================================================================================
来源：http://hz.aizwys.cn/gtdpuxmlkr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.andypj.xyz/gtsqwwzpwc.html

================================================================================
来源：http://hz.zhixingplan.top/gtwnrwnuhj.html

[T01] Kotlin：Hello World
来源：http://hz.cheryme.top/gtizajrtor.html

println("Hello")
来源：http://hz.cucudq.cn/gtoddihuoi.html

[T02] Kotlin：变量
来源：http://hz.shangyingyoupin.top/gtdfqzjswt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hnxiangtu.top/gtuhnrjfnf.html

[T03] Kotlin：字符串模板
来源：http://hz.yanxiufei.cn/gtgcgxzjmy.html

"值: $b"
来源：http://hz.zdqjudy.top/gtzrwunxmu.html

[T04] Kotlin：空安全
来源：http://hz.daxiang520.top/gtiwbkcjsj.html

val n: String? = null;  n?.length
来源：http://hz.hnxiangtu.top/gtxickyvip.html

[T05] Kotlin：when 表达式
来源：http://hz.ehwqpu.com/gtbmdaousl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.havefunace.top/gtkmxsrfns.html

[T06] Kotlin：集合映射
来源：http://hz.svipenyu.cn/gthlrzkycs.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yuxming.cn/gtematcvjm.html

[T07] Kotlin：集合过滤
来源：http://hz.hywenlv.cn/gtyqiyrztc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.gaohongyu789.top/gtwuuqmmcc.html

[T08] Kotlin：数据类
来源：http://hz.cheryme.top/gtsrfcwlyu.html

data class User(val name: String, val age: Int)
来源：http://hz.pengpengdd.cyou/gtmafykqqs.html

[T09] Kotlin：扩展函数
来源：http://hz.316326.xyz/gtrzkbbxwy.html

fun String.exclaim() = this + "!"
来源：http://hz.birdmap.top/gtokgejxag.html

[T10] Kotlin：默认参数
来源：http://hz.yj20258888.top/gtfzwycvhq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.cheryme.top/gtgsacbuqw.html

[T11] Kotlin：协程
来源：http://hz.yj20258888.top/gtmlsdddbo.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yanxiufei.cn/gtwcfkimfd.html

[T12] Kotlin：解构声明
来源：http://hz.sysykeji.top/gteffvauok.html

val (a, b) = Pair(1, 2)
来源：http://hz.jqgufenzy.top/gtthuhwbom.html

[T13] Kotlin：只读 Map
来源：http://hz.jinqigufen.top/gtaxqoglzm.html

val m = mapOf("a" to 1)
来源：http://hz.birdmap.top/gtcmpouxfv.html

[T14] Kotlin：循环
来源：http://hz.ydzc1.top/gtjjfcnmjn.html

for (i in 1..10) println(i)
来源：http://hz.shanyushiyangtech.top/gtafyzbasr.html

[T15] Kotlin：接口
来源：http://hz.ppjwa.cn/gtpoqkszcr.html

interface Shape { fun area(): Double }
来源：http://hz.vqdsnc.cn/gtqzphanoz.html

[T16] Swift：Hello World
来源：http://hz.hywenlv.cn/gttafqywya.html

print("Hello")
来源：http://hz.hfpthk.cn/gtxejwomci.html

[T17] Swift：变量与常量
来源：http://hz.sysykeji.top/gtihludljc.html

var a = 1;  let b = 2
来源：http://hz.yangfankeji.com/gtzqkhugra.html

[T18] Swift：字符串插值
来源：http://hz.ywan-chungtsiang.top/gtxhqezwan.html

"值: \(b)"
来源：http://hz.cucudq.cn/gtbuphrvjm.html

[T19] Swift：可选绑定
来源：http://hz.aizwys.cn/gtpfyznthu.html

if let n = opt { print(n) }
来源：http://hz.gaohongyu789.top/gtmhjjsbhp.html

[T20] Swift：数组操作
来源：http://hz.nanxinkj.top/gtnciygjgv.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.sysykeji.top/gtzwdrdbvr.html

[T21] Swift：遍历
来源：http://hz.ydzc1.top/gtnrntfzks.html

for x in a { print(x) }
来源：http://hz.ywan-chungtsiang.top/gtnkzyfigj.html

[T22] Swift：字典
来源：http://hz.ywan-chungtsiang.top/gtlcizbtgu.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yuanzhike.top/gtdlgtwhwj.html

[T23] Swift：函数
来源：http://hz.nwbrower.top/gtsfzcffcl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.sweek.top/gtuxbbvgnv.html

[T24] Swift：闭包
来源：http://hz.sufxvd.cn/gtsncpyhdk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.cucudq.cn/gtzdjwcgqe.html

[T25] Swift：结构体
来源：http://hz.mhx1999.top/gtozqzcpzj.html

struct P { var x: Int }
来源：http://hz.9152youxi.cn/gtwhrihtes.html

[T26] Swift：类与重写
来源：http://hz.fzhhl.top/gtoknthlfw.html

class A: Base { override func f() {} }
来源：http://hz.zhijiandao.cn/gtzwlzrxpm.html

[T27] Swift：错误处理
来源：http://hz.shzxlz.cn/gtziylmiyj.html

do { try f() } catch { print(error) }
来源：http://hz.hnqzz.top/gtfgdqxabd.html

[T28] Swift：枚举
来源：http://hz.hnxiangtu.top/gtyetxhzxy.html

enum Color { case red, green }
来源：http://hz.svipenyu.cn/gtsyygamds.html

[T29] Swift：guard 提前返回
来源：http://hz.tianlin.xyz/gtuufsltbm.html

guard let x = opt else { return }
来源：http://hz.shzxlz.cn/gtssuxdwfa.html

[T30] Swift：协议
来源：http://hz.snrcjt.cn/gtyzeumjlw.html

protocol Shape { func area() -> Double }
来源：http://hz.yvedp.cn/gtnhlcxnxi.html

[T31] Lua：Hello World
来源：http://hz.52xcode.cn/gtuacqafnb.html

print("Hello")
来源：http://hz.ppjwa.cn/gtttviusbn.html

[T32] Lua：局部变量
来源：http://hz.yongpay.top/gtmghjacyd.html

local a = 1
来源：http://hz.daxiang520.top/gtopndjwrm.html

[T33] Lua：表（数组）
来源：http://hz.zhaomingkeji.xyz/gtsowfztwr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jinqigufen.top/gthprxfvoh.html

[T34] Lua：遍历表
来源：http://hz.ywan-chungtsiang.top/gtkvjsxdsp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.nanxinkj.top/gtodeunjzx.html

[T35] Lua：字典表
来源：http://hz.0kj1m.cn/gtkirwoltt.html

local d = { a = 1 };  d.b = 2
来源：http://hz.xuetiantiany.cn/gtvxzwcltd.html

[T36] Lua：函数
来源：http://hz.c1oappe.top/gtzviglehv.html

function add(a, b) return a + b end
来源：http://hz.dashuyun.cn/gtdsarwzsi.html

[T37] Lua：字符串拼接
来源：http://hz.hnxiangtu.top/gtgwktkakq.html

"a" .. "b"
来源：http://hz.sxryk.cn/gtahkkwrfz.html

[T38] Lua：条件
来源：http://hz.nanxinkj.top/gtncfkifos.html

if x > 0 then print("正") end
来源：http://hz.dashuyun.cn/gtxdgqfoem.html

[T39] Lua：模式匹配
来源：http://hz.0kj1m.cn/gtxbihqsqy.html

string.find(s, "%d+")
来源：http://hz.aibaodan.cn/gtzxubtnay.html

[T40] Lua：元表
来源：http://hz.jlsjyb.cn/gtvpwxgido.html

setmetatable({}, { __index = base })
来源：http://hz.ydzc1.top/gtqnmbsnbx.html

[T41] Perl：Hello World
来源：http://hz.nanxinkj.top/gtcaiyscbc.html

print "Hello\n";
来源：http://hz.xingfuxueyuan.xyz/gtokeajtyn.html

[T42] Perl：变量类型
来源：http://hz.andypj.xyz/gtzdozdimu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.guannengcc.top/gtzaqwrmyi.html

[T43] Perl：字符串插值
来源：http://hz.tianlin.xyz/gtttolfmvn.html

"值: $a"
来源：http://hz.gaohongyu789.top/gteufucglt.html

[T44] Perl：条件
来源：http://hz.jyoumei.cn/gtqydeteoa.html

if ($a > 0) { print "正"; }
来源：http://hz.jqgfzy.top/gtxypffhro.html

[T45] Perl：数组遍历
来源：http://hz.nwbrower.top/gtsgqvwplh.html

for my $x (@arr) { print $x; }
来源：http://hz.jqgfzy.top/gtapkyzfdh.html

[T46] Perl：哈希操作
来源：http://hz.andypj.xyz/gtsyualiqs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yanxiufei.cn/gtdaqbhbgi.html

[T47] Perl：正则捕获
来源：http://hz.hfpthk.cn/gtnbkadohw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.316326.xyz/gtqztodknv.html

[T48] Perl：正则替换
来源：http://hz.sweek.top/gtvruyocjx.html

$s =~ s/old/new/g;
来源：http://hz.zhaomingkeji.xyz/gtbkdlifgz.html

[T49] Perl：函数
来源：http://hz.mhx1999.top/gtrdqjovfv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.shanyushiyangtech.top/gtfmeevkmw.html

[T50] Perl：逐行读文件
来源：http://hz.fzhhl.top/gtniedfoll.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yj202588.top/gtbjzxuxey.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.nanxuanxn.top/gtdbmneghr.html

[T51] Scala：Hello World
来源：http://hz.chenzaomai.com/gtapzlsopp.html

println("Hello")
来源：http://hz.yj202588.top/gtbfpwdqon.html

[T52] Scala：变量
来源：http://hz.cdnleiting.top/gtxivahbzt.html

val a = 1;  var b = 2
来源：http://hz.aibaodan.cn/gttybmgcyb.html

[T53] Scala：字符串插值
来源：http://hz.nanxinkj.top/gtlzbegyrx.html

s"值: $b"
来源：http://hz.hysaishi.cn/gtxtidwtsb.html

[T54] Scala：集合映射
来源：http://hz.aibaodan.cn/gtumprmspt.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.havefunace.top/gtdivdnjrp.html

[T55] Scala：集合过滤
来源：http://hz.xinyue.icu/gtfgcachmp.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.yj20258.top/gtqfbhkgst.html

[T56] Scala：样例类
来源：http://hz.xingfuxueyuan.xyz/gtofdffkjt.html

case class User(name: String, age: Int)
来源：http://hz.pengpengdd.cyou/gtxrarerzw.html

[T57] Scala：模式匹配
来源：http://hz.pengpengdd.cyou/gtcnabvltx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.yj20258.top/gtmwxwdoji.html

[T58] Scala：函数定义
来源：http://hz.hammf.cn/gtegsyoave.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.hongshengwenyu.top/gtdvicbvkz.html

[T59] Scala：循环
来源：http://hz.shanyushiyangtech.top/gtwntkhliu.html

for (i <- 1 to 10) println(i)
来源：http://hz.zhiwuduotai.top/gtqxwnwiki.html

[T60] Scala：折叠
来源：http://hz.316326.xyz/gtyknfhaed.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yanxiufei.cn/gtpdsugjqb.html

================================================================================
来源：http://hz.hywenlv.cn/gtuyeubvva.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yanxiufei.cn/gtkxtzwbpk.html

================================================================================
来源：http://hz.jiagoushi.top/gtpesoqiha.html

[U01] Py：创建虚拟环境
来源：http://hz.tanke756.top/gtwxzhsuxc.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.hongshengwenyu.top/gtnvmffhhr.html

[U02] Py：导出 / 安装依赖
来源：http://hz.shanyushiyangkeji.top/gtaifhzcth.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.gzhubu.top/gtrggqbwdb.html

[U03] Py：加载 .env 配置
来源：http://hz.jianghu66.top/gtlkekomgk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zhijiandao.cn/gtgroglngc.html

[U04] Py：变量调试打印
来源：http://hz.sufxvd.cn/gtfjudsnqj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yuanzhike.top/gtcmcdwvoi.html

[U05] Py：列表去重且保序
来源：http://hz.hnxiangtu.top/gtuhptxamn.html

list(dict.fromkeys(arr))
来源：http://hz.feifeiyinyue.top/gttxukamyt.html

[U06] Py：合并两个字典
来源：http://hz.cucudq.cn/gttgmvfexu.html

{**a, **b}
来源：http://hz.cqqwz.cn/gturvnpcwh.html

[U07] Py：反转字典键值
来源：http://hz.yvedp.cn/gtilcarusd.html

{v: k for k, v in d.items()}
来源：http://hz.hammf.cn/gtwqpsdxgi.html

[U08] Py：展平二维列表
来源：http://hz.gzhubu.top/gtxgegjmty.html

[y for x in nested for y in x]
来源：http://hz.yuanzhike.top/gtdxvebjvd.html

[U09] Py：字典取最大值的键
来源：http://hz.zycfv.cn/gtejqshxem.html

max(d, key=d.get)
来源：http://hz.fzhhl.top/gterepswmi.html

[U10] Py：按值排序字典
来源：http://hz.hfpthk.cn/gtytnfryom.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.jiagoushi.top/gtlfqlikkt.html

[U11] Py：生成器表达式
来源：http://hz.redwolf501.top/gtigggqvrb.html

(x * 2 for x in arr)
来源：http://hz.zhongyouzk.top/gtmjwdgkyn.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.shuidangran.top/gtalhlrlxe.html

Counter(arr).most_common(3)
来源：http://hz.havefunace.top/gtrtjjpjtj.html

[U13] Py：固定长度队列
来源：http://hz.zhaomingkeji.xyz/gtlmxrbyqs.html

deque(maxlen=10)
来源：http://hz.jqgufenzy.top/gtlkysqlmn.html

[U14] Py：分组收集到列表
来源：http://hz.pengpengdd.cyou/gtiifmwfky.html

defaultdict(list)
来源：http://hz.jlsjyb.cn/gtytgyorec.html

[U15] Py：高精度计时
来源：http://hz.yanxiufei.cn/gtgdcjwlyd.html

t = time.perf_counter()
来源：http://hz.birdmap.top/gtideqjctu.html

[U16] Py：命令行参数解析
来源：http://hz.redwolf501.top/gtplhkhcad.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.nanxuanxn.top/gtunkzmman.html

[U17] Py：初始化日志
来源：http://hz.mhx1999.top/gtjcjodojy.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.xuetiantiany.cn/gtrjhhgcfr.html

[U18] Py：预编译正则
来源：http://hz.nwbrower.top/gtqscmynre.html

pat = re.compile(r"\d+")
来源：http://hz.zhengqikj.top/gtrwunvnuj.html

[U19] Py：正则替换带回调
来源：http://hz.guowangkeji.top/gtanszejef.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.pycfn.com/gtshvwimyr.html

[U20] Py：缓存函数结果
来源：http://hz.ehwqpu.com/gtlxoeypxj.html

@functools.lru_cache(maxsize=None)
来源：http://hz.sysykeji.top/gtfuhtoblr.html

[U21] Py：自定义上下文管理器
来源：http://hz.pycfn.com/gtedywhirg.html

@contextlib.contextmanager
来源：http://hz.pengpengdd.cyou/gtblxmtpix.html

[U22] Py：矩阵转置
来源：http://hz.ehwqpu.com/gtwtaanogr.html

list(zip(*m))
来源：http://hz.dianchejie.cn/gtaljfkpot.html

[U23] Py：分块读取大文件
来源：http://hz.hongshengwenyu.top/gtzaysnadq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.pycfn.com/gtyfvvlvzr.html

[U24] Py：路径操作
来源：http://hz.cheryme.top/gtcskdwyyy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.zhijiandao.cn/gtfhltqews.html

[U25] Py：CSV 按字典读
来源：http://hz.fengsongda.top/gtuebxrdym.html

csv.DictReader(f)
来源：http://hz.zhiwuduotai.top/gtcmyatqfo.html

[U26] Py：并发下载
来源：http://hz.zhiwuduotai.top/gtgyjkjkce.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.ywan-chungtsiang.top/gtnxifwdho.html

[U27] Py：异步 HTTP
来源：http://hz.c1oappe.top/gtaloeqxzf.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.yongpay.top/gtlkptpybw.html

[U28] Py：类型别名
来源：http://hz.daxiang520.top/gtfzfjtrgq.html

UserId = int
来源：http://hz.jiagoushi.top/gtgqdpmfwr.html

[U29] Py：属性校验
来源：http://hz.cashguo.top/gtkvbpnwsm.html

@property 与 @x.setter 配合
来源：http://hz.guowangkeji.top/gtzndzfjxs.html

[U30] Py：数据类
来源：http://hz.yongpay.top/gteefiamvy.html

@dataclass(slots=True)
来源：http://hz.haohaochexian.top/gtqyckmofx.html

[U31] Py：单测
来源：http://hz.dashuyun.cn/gtdgbuaysx.html

python -m pytest -q
来源：http://hz.hammf.cn/gtllxcdape.html

[U32] Py：代码格式化
来源：http://hz.jinghuilouyu.cn/gtrjflgmzx.html

ruff format . && ruff check --fix .
来源：http://hz.tanke756.top/gtcxqqwpvs.html

[U33] Py：打包发布
来源：http://hz.guannengcc.top/gthotnbaxq.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.sxryk.cn/gtcmbaymfv.html

[U34] Py：判断编码
来源：http://hz.sufxvd.cn/gteglglsfm.html

chardet.detect(raw)
来源：http://hz.kuanghao11.cn/gtpzkcruyx.html


<!-- 参考信息 -->