代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.nwbrower.top/gtxgyrntwi.html

[S08] C：动态内存分配与释放
来源：http://hz.gzhubu.top/gtsifgnlzd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xingfuxueyuan.xyz/gtqszlqosu.html

[S09] C：结构体定义与初始化
来源：http://hz.iojbl.cn/gtpfsyfktp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.pycfn.com/gtrykgiqtx.html

[S10] C：指针与解引用
来源：http://hz.xuetiantiany.cn/gtithkfohq.html

int *p = &a;  *p = 5;
来源：http://hz.pycfn.com/gteaobmnft.html

[S11] C：逐行读文件
来源：http://hz.kuanghao11.cn/gtokpufmug.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.shzxlz.cn/gtqktpxsli.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.sxryk.cn/gtpypxuwnt.html

fclose(f);
来源：http://hz.zhengqikj.top/gtuzrocwrm.html

[S12] C：写文件
来源：http://hz.aizwys.cn/gttoauzxmd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.gotoacloud.top/gtqtsdypfa.html

[S13] C：宏定义
来源：http://hz.jianghu66.top/gtuhbeqabp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.iojbl.cn/gtnwilfsdu.html

[S14] C：枚举
来源：http://hz.yuanzhike.top/gtuankhrmw.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhaomingkeji.xyz/gtiwifosks.html

[S15] C：类型转换
来源：http://hz.xuanzx.com/gthzorjltx.html

(double) a / b
来源：http://hz.zhoulong.xyz/gtpifytqen.html

[S16] C：位操作置位
来源：http://hz.shanyushiyangkeji.top/gtcaqqmvgf.html

x |= (1 << 3);
来源：http://hz.wangshuangyany.cn/gtpatffyhp.html

[S17] C：安全拼接字符串
来源：http://hz.chenlongwang.top/gtsgsjqtkb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ydzc1.top/gtbvvvgoiq.html

[S18] C：命令行参数
来源：http://hz.daria6918.cn/gtbkwlraly.html

int main(int argc, char **argv)
来源：http://hz.quarkkingdee.top/gtjcnrjnwt.html

[S19] C：快速排序
来源：http://hz.zhongyouzk.top/gtorpbwfdj.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.tianlin.xyz/gtraeqswjr.html

[S20] C：二分查找
来源：http://hz.ydjk.org.cn/gtfiikudii.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.xuanzx.com/gtssjluyqv.html

[S21] C：字符类别判断
来源：http://hz.shanyushiyangtech.top/gtejxpfcic.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yueranfly.top/gtvtcggkzm.html

[S22] C：字符串转数字
来源：http://hz.yongpay.top/gtcpjxtzyy.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yvedp.cn/gtxgojllgw.html

[S23] C：随机数
来源：http://hz.0kj1m.cn/gteutlbkll.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.shuidangran.top/gtfesthdho.html

[S24] C：获取本地时间
来源：http://hz.yvedp.cn/gtfuqrhukv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.redwolf501.top/gtjclgalmg.html

[S25] C：内存拷贝
来源：http://hz.bjfxy.top/gtemfownas.html

memcpy(dst, src, n);
来源：http://hz.tanke756.top/gtjefahdyd.html

[S26] C：内存清零
来源：http://hz.ehwqpu.com/gtpksvugxm.html

memset(a, 0, sizeof a);
来源：http://hz.tianlin.xyz/gtgobzdfbm.html

[S27] C：定义常量
来源：http://hz.yj20258.top/gtmgaczvtl.html

const double PI = 3.14159;
来源：http://hz.gogol.net.cn/gtqrncdyhq.html

[S28] C：静态变量
来源：http://hz.ivvv.top/gtmzfmzahb.html

static int counter = 0;
来源：http://hz.cqqwz.cn/gtodjsykdy.html

[S29] C：变参函数
来源：http://hz.aibaodan.cn/gtwgakdmlb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ivvv.top/gtimxjweby.html

[S30] C：头文件保护
来源：http://hz.jlsjyb.cn/gtkodzgmkn.html

#ifndef X_H
来源：http://hz.ywan-chungtsiang.top/gteujetjlm.html

#define X_H
来源：http://hz.sufxvd.cn/gtdskqbyjb.html

#endif
来源：http://hz.sufxvd.cn/gtdodibgpp.html

[S31] C++：Hello World
来源：http://hz.cashguo.top/gtfsgqvvhb.html

#include <iostream>
来源：http://hz.xuanzx.com/gtmonpndvc.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.fzhhl.top/gtsihhlcvt.html

[S32] C++：字符串
来源：http://hz.jlsjyb.cn/gtdtfprtcn.html

std::string s = "hi";  s += "!";
来源：http://hz.jiagoushi.top/gtisbabfaj.html

[S33] C++：vector 增删
来源：http://hz.zhaomingkeji.xyz/gtmwudxlmg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jqgfzy.top/gtiktnknyv.html

[S34] C++：遍历 vector
来源：http://hz.gaohongyu789.top/gtylhfuyzr.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.aibaodan.cn/gtbbpmtbos.html

[S35] C++：map
来源：http://hz.yj20258888.top/gtpopofrwe.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hnxiangtu.top/gtqrhazxzi.html

[S36] C++：unordered_map
来源：http://hz.svipenyu.cn/gtrsfyfmbt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.svipenyu.cn/gthraghjcj.html

[S37] C++：set
来源：http://hz.shanyushiyangkeji.top/gtlbvuhnua.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ydjk.org.cn/gtfsgjnhhf.html

[S38] C++：排序
来源：http://hz.xylfe.cn/gtqfwknhkz.html

std::sort(v.begin(), v.end());
来源：http://hz.nanxuanxn.top/gtseqtjcjx.html

[S39] C++：自定义比较器排序
来源：http://hz.nwbrower.top/gtrksdwxuh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jinyuanbaomall.cn/gtdvbvqkba.html

[S40] C++：查找元素
来源：http://hz.cdnleiting.top/gtqljxdjzn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jiagoushi.top/gtgjmmwuak.html

[S41] C++：类与构造函数
来源：http://hz.hysaishi.cn/gtigvcdijm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.chenjidiqi.icu/gtgwpadqdi.html

[S42] C++：继承与虚函数
来源：http://hz.yongpay.top/gtkozunhzn.html

class B : public Base { public: void f() override {} };
来源：http://hz.guannengcc.top/gtaktmqrug.html

[S43] C++：智能指针
来源：http://hz.chenzaomai.com/gtrlhbrxeg.html

auto p = std::make_unique<int>(5);
来源：http://hz.gaohongyu789.top/gthmdxrvue.html

[S44] C++：引用传参
来源：http://hz.52xcode.cn/gtviywjwrb.html

void inc(int &x) { ++x; }
来源：http://hz.yangfankeji.com/gtklsehowu.html

[S45] C++：lambda
来源：http://hz.sysykeji.top/gtwuflphvz.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhijiandao.cn/gtacmfccyy.html

[S46] C++：函数模板
来源：http://hz.chenjidiqi.icu/gtieuutjzu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.chenzaomai.com/gttfxuwvzu.html

[S47] C++：结构化绑定遍历
来源：http://hz.pengpengdd.cyou/gtnfhckjwn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ivvv.top/gtuvknvbrn.html

[S48] C++：逐行读文件
来源：http://hz.52xcode.cn/gtptqpodws.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.316326.xyz/gtacayzvtc.html

while (std::getline(in, line)) { }
来源：http://hz.gotoacloud.top/gthvozrjpy.html

[S49] C++：写文件
来源：http://hz.fzhhl.top/gtexfajiyd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.c1oappe.top/gtqhinaoha.html

[S50] C++：格式化数字
来源：http://hz.yanxiufei.cn/gtdjkucuoi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jinqigufen.top/gtljzxsfsa.html

[S51] C++：显式类型转换
来源：http://hz.dashuyun.cn/gtxldexjgy.html

static_cast<double>(a) / b
来源：http://hz.aibaodan.cn/gtfzgtuetg.html

[S52] C++：const 与 noexcept
来源：http://hz.xziqi.cn/gtcnfkstll.html

int size() const noexcept { return n_; }
来源：http://hz.yongpay.top/gtqkyxytfc.html

[S53] C++：移动语义
来源：http://hz.fengsongda.top/gtzgghpwwr.html

std::vector<int> w = std::move(v);
来源：http://hz.wangshuangyany.cn/gtvozsvsgy.html

[S54] C++：异常处理
来源：http://hz.chenzaomai.com/gtvrdsenlt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.svipenyu.cn/gthvoebiml.html

[S55] C++：结构化绑定
来源：http://hz.ydjk.org.cn/gtgcvhdycl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.cdnleiting.top/gtzouvdnoo.html

[S56] C++：optional
来源：http://hz.hysaishi.cn/gtvjfcmibw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.ydzc1.top/gtzooktkoj.html

[S57] C++：编译期常量
来源：http://hz.cdnleiting.top/gtkdadxlih.html

constexpr int N = 10;
来源：http://hz.tian-w.cn/gtaxwnthmk.html

[S58] C++：命名空间
来源：http://hz.sufxvd.cn/gtwntflyud.html

namespace ns { int f() { return 1; } }
来源：http://hz.52xcode.cn/gtpgsimgpz.html

[S59] C++：静态断言
来源：http://hz.zhijiandao.cn/gtjzowbbct.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ydzc1.top/gtkldjodis.html

[S60] C++：遍历并删除元素
来源：http://hz.ydzc1.top/gtjckbvrtw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.vqdsnc.cn/gteoqgwmsc.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtwbxhbflc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.wangdashe.top/gtkmizypmg.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtxwgpyfvb.html

[T01] Kotlin：Hello World
来源：http://hz.andypj.xyz/gtcippzzcf.html

println("Hello")
来源：http://hz.cashguo.top/gtrftdjewb.html

[T02] Kotlin：变量
来源：http://hz.yj20258888.top/gtxrkmpmkg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jinyuanbaomall.cn/gtgeuaaaeo.html

[T03] Kotlin：字符串模板
来源：http://hz.jinghuilouyu.cn/gtopxiqkrx.html

"值: $b"
来源：http://hz.daria6918.cn/gturueebed.html

[T04] Kotlin：空安全
来源：http://hz.dashuyun.cn/gthuoyvyxm.html

val n: String? = null;  n?.length
来源：http://hz.vqdsnc.cn/gthbevdjgl.html

[T05] Kotlin：when 表达式
来源：http://hz.cashguo.top/gtdqbmldkd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ybcxt.top/gtgbvkcmsx.html

[T06] Kotlin：集合映射
来源：http://hz.smart0.xyz/gtwusmqrse.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.havefunace.top/gtofomiydz.html

[T07] Kotlin：集合过滤
来源：http://hz.yj202588.top/gtesnglrfc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.guannengcc.top/gtcnjmbygw.html

[T08] Kotlin：数据类
来源：http://hz.pycfn.com/gtmhpzfdmo.html

data class User(val name: String, val age: Int)
来源：http://hz.yanxiufei.cn/gthdcksdgv.html

[T09] Kotlin：扩展函数
来源：http://hz.xinyue.icu/gtpjtdxbwe.html

fun String.exclaim() = this + "!"
来源：http://hz.cheryme.top/gtzdisnutv.html

[T10] Kotlin：默认参数
来源：http://hz.gogol.net.cn/gtrhbsstaa.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zycfv.cn/gtefkbndol.html

[T11] Kotlin：协程
来源：http://hz.sufxvd.cn/gtyoyluxhm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.hysaishi.cn/gttljepokb.html

[T12] Kotlin：解构声明
来源：http://hz.aibaodan.cn/gtfhnlafyi.html

val (a, b) = Pair(1, 2)
来源：http://hz.redwolf501.top/gtnqelxmbo.html

[T13] Kotlin：只读 Map
来源：http://hz.sysykeji.top/gtlsvryabw.html

val m = mapOf("a" to 1)
来源：http://hz.jlsjyb.cn/gtucwwnpxy.html

[T14] Kotlin：循环
来源：http://hz.shzxlz.cn/gtxqmtwfkq.html

for (i in 1..10) println(i)
来源：http://hz.gaohongyu789.top/gtsrdxcqbr.html

[T15] Kotlin：接口
来源：http://hz.jlsjyb.cn/gtypalbyvz.html

interface Shape { fun area(): Double }
来源：http://hz.yonumen.top/gtxtqnktbq.html

[T16] Swift：Hello World
来源：http://hz.xuanzx.com/gtrddbjnlz.html

print("Hello")
来源：http://hz.nanxuanxn.top/gtevryzhwg.html

[T17] Swift：变量与常量
来源：http://hz.yuxming.cn/gtecawwsbh.html

var a = 1;  let b = 2
来源：http://hz.tanke756.top/gtklaxhsfr.html

[T18] Swift：字符串插值
来源：http://hz.yj20258.top/gtcjwmwfld.html

"值: \(b)"
来源：http://hz.jlsjyb.cn/gtwlzcqtux.html

[T19] Swift：可选绑定
来源：http://hz.hysaishi.cn/gtwhqxlidk.html

if let n = opt { print(n) }
来源：http://hz.andypj.xyz/gtuxvbwgyl.html

[T20] Swift：数组操作
来源：http://hz.svipenyu.cn/gtawiqqzai.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.hnxiangtu.top/gtnkgguwpf.html

[T21] Swift：遍历
来源：http://hz.xuetiantiany.cn/gtahxpffng.html

for x in a { print(x) }
来源：http://hz.daxiang520.top/gttqnvwwbu.html

[T22] Swift：字典
来源：http://hz.dianchejie.cn/gtkbljcyhy.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.fengsongda.top/gtwumscjdj.html

[T23] Swift：函数
来源：http://hz.jianghu66.top/gtasvmjsaa.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.andypj.xyz/gtrcefjnro.html

[T24] Swift：闭包
来源：http://hz.nanxinkj.top/gtpintozod.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.iojbl.cn/gtffkvdeqj.html

[T25] Swift：结构体
来源：http://hz.0kj1m.cn/gtlvnmbysu.html

struct P { var x: Int }
来源：http://hz.pengpengdd.cyou/gtnmerqahs.html

[T26] Swift：类与重写
来源：http://hz.guannengcc.top/gtpzfmygtu.html

class A: Base { override func f() {} }
来源：http://hz.aizwys.cn/gtdvtsczfm.html

[T27] Swift：错误处理
来源：http://hz.birdmap.top/gtzpwitxln.html

do { try f() } catch { print(error) }
来源：http://hz.mhx1999.top/gtarotardu.html

[T28] Swift：枚举
来源：http://hz.bjfxy.top/gtldtwfxku.html

enum Color { case red, green }
来源：http://hz.xingfuxueyuan.xyz/gtahnwzorn.html

[T29] Swift：guard 提前返回
来源：http://hz.cucudq.cn/gtgnfniwbj.html

guard let x = opt else { return }
来源：http://hz.aizwys.cn/gtzxaczwmk.html

[T30] Swift：协议
来源：http://hz.hnxiangtu.top/gtwxhcyksw.html

protocol Shape { func area() -> Double }
来源：http://hz.jinqigufen.top/gtpxvketxg.html

[T31] Lua：Hello World
来源：http://hz.xuetiantiany.cn/gtdbqbeqlu.html

print("Hello")
来源：http://hz.yuanzhike.top/gttrnqphsk.html

[T32] Lua：局部变量
来源：http://hz.yuanzhike.top/gtrqcodqan.html

local a = 1
来源：http://hz.jqgfzy.top/gtsnkftfxn.html

[T33] Lua：表（数组）
来源：http://hz.jinqigfzy.top/gtfbfmwzwt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zhongyouzk.top/gtnvpqggzy.html

[T34] Lua：遍历表
来源：http://hz.guannengcc.top/gtoqbrejbu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yj202588.top/gtudenwcyu.html

[T35] Lua：字典表
来源：http://hz.andypj.xyz/gtozllqokx.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jqgufenzy.top/gtaptezlez.html

[T36] Lua：函数
来源：http://hz.jyoumei.cn/gtdrfudbhp.html

function add(a, b) return a + b end
来源：http://hz.ivvv.top/gttwdtjzjp.html

[T37] Lua：字符串拼接
来源：http://hz.cheryme.top/gtoykakaux.html

"a" .. "b"
来源：http://hz.shanyushiyangkeji.top/gtoajhupql.html

[T38] Lua：条件
来源：http://hz.xingfuxueyuan.xyz/gtckrrgsdg.html

if x > 0 then print("正") end
来源：http://hz.shzxlz.cn/gtctwdiuiu.html

[T39] Lua：模式匹配
来源：http://hz.tianlin.xyz/gtcpplnily.html

string.find(s, "%d+")
来源：http://hz.havefunace.top/gtaiybmgjb.html

[T40] Lua：元表
来源：http://hz.jqgufenzy.top/gttadcmjny.html

setmetatable({}, { __index = base })
来源：http://hz.yonumen.top/gtwfbmvoet.html

[T41] Perl：Hello World
来源：http://hz.tanke756.top/gtrdxjjzbi.html

print "Hello\n";
来源：http://hz.havefunace.top/gtpnfpqtcc.html

[T42] Perl：变量类型
来源：http://hz.gzhubu.top/gtlxtyuegg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.chenlongwang.top/gtwjjxrlcs.html

[T43] Perl：字符串插值
来源：http://hz.guannengcc.top/gttxlcfwmy.html

"值: $a"
来源：http://hz.0kj1m.cn/gtdzyeckup.html

[T44] Perl：条件
来源：http://hz.yueranfly.top/gtsuqrgbmy.html

if ($a > 0) { print "正"; }
来源：http://hz.xingfuxueyuan.xyz/gtakolgicy.html

[T45] Perl：数组遍历
来源：http://hz.zhiwuduotai.top/gtpvfgvrzg.html

for my $x (@arr) { print $x; }
来源：http://hz.bjfxy.top/gtlpbtfqum.html

[T46] Perl：哈希操作
来源：http://hz.yuanzhike.top/gtqlgxslpb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.hywenlv.cn/gtrgbigwfs.html

[T47] Perl：正则捕获
来源：http://hz.ywan-chungtsiang.top/gtxoryjhoz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.feifeiyinyue.top/gttfsilvfz.html

[T48] Perl：正则替换
来源：http://hz.cheryme.top/gtocuswxug.html

$s =~ s/old/new/g;
来源：http://hz.zhengqikj.top/gtlwlukyjn.html

[T49] Perl：函数
来源：http://hz.yj20258.top/gtlnxdjphm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.shanyushiyangkeji.top/gtxgcwvoet.html

[T50] Perl：逐行读文件
来源：http://hz.wangdashe.top/gtjyiwebzy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.ybcxt.top/gtwwfuqdnk.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.hammf.cn/gtzdygtntn.html

[T51] Scala：Hello World
来源：http://hz.fengsongda.top/gtwmoqnxrm.html

println("Hello")
来源：http://hz.daria6918.cn/gtgeqhkyzk.html

[T52] Scala：变量
来源：http://hz.smart0.xyz/gtcuwhggtf.html

val a = 1;  var b = 2
来源：http://hz.andypj.xyz/gtoyofcfbk.html

[T53] Scala：字符串插值
来源：http://hz.meibo888.top/gtlinsfvgr.html

s"值: $b"
来源：http://hz.yj20258.top/gtyxhaafyl.html

[T54] Scala：集合映射
来源：http://hz.wangdashe.top/gtwiovjniy.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yuanzhike.top/gtzxahilmu.html

[T55] Scala：集合过滤
来源：http://hz.fzhhl.top/gtaxzeyvez.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.aizwys.cn/gtthtrzehr.html

[T56] Scala：样例类
来源：http://hz.daxiang520.top/gtcmjprjqo.html

case class User(name: String, age: Int)
来源：http://hz.jlsjyb.cn/gtarfcqgzk.html

[T57] Scala：模式匹配
来源：http://hz.gaohongyu789.top/gttepdyskg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.jiagoushi.top/gtwnpnzcfc.html

[T58] Scala：函数定义
来源：http://hz.xziqi.cn/gtcntdyhty.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yangfankeji.com/gtzoxaudmk.html

[T59] Scala：循环
来源：http://hz.ydjk.org.cn/gtfbsufwzc.html

for (i <- 1 to 10) println(i)
来源：http://hz.chenjidiqi.icu/gtsqulagse.html

[T60] Scala：折叠
来源：http://hz.yangfankeji.com/gtynnzxsfy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.tanke756.top/gtqxvebiya.html

================================================================================
来源：http://hz.meibo888.top/gtvjihwyhw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.hnxiangtu.top/gtlohibbhf.html

================================================================================
来源：http://hz.kuanghao11.cn/gtroicwefd.html

[U01] Py：创建虚拟环境
来源：http://hz.zhaomingkeji.xyz/gtwntvfzxu.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.gogol.net.cn/gtbsgrjszc.html

[U02] Py：导出 / 安装依赖
来源：http://hz.nanxuanxn.top/gtuojljzyz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.fengsongda.top/gtfuzxkiti.html

[U03] Py：加载 .env 配置
来源：http://hz.shanyushiyangtech.top/gtosfyiusc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zhixingplan.top/gtmwdcxvjb.html

[U04] Py：变量调试打印
来源：http://hz.ivvv.top/gtibhwcomw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yj202588.top/gtbywzdsoi.html

[U05] Py：列表去重且保序
来源：http://hz.wangdashe.top/gtwdvyjopo.html

list(dict.fromkeys(arr))
来源：http://hz.jqgfzy.top/gtdlfzwvcf.html

[U06] Py：合并两个字典
来源：http://hz.jlsjyb.cn/gthzgopjls.html

{**a, **b}
来源：http://hz.jinyuanbaomall.cn/gtyquokulk.html

[U07] Py：反转字典键值
来源：http://hz.hnqzz.top/gtkkonalbr.html

{v: k for k, v in d.items()}
来源：http://hz.vqdsnc.cn/gtbyhwigeq.html

[U08] Py：展平二维列表
来源：http://hz.svipenyu.cn/gtskdrisxu.html

[y for x in nested for y in x]
来源：http://hz.zdqjudy.top/gtdgufqvri.html

[U09] Py：字典取最大值的键
来源：http://hz.cashguo.top/gtltcfxvjh.html

max(d, key=d.get)
来源：http://hz.birdmap.top/gtrpwweqhq.html

[U10] Py：按值排序字典
来源：http://hz.xingfuxueyuan.xyz/gtkhxgztov.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.feifeiyinyue.top/gtdlgfwsan.html

[U11] Py：生成器表达式
来源：http://hz.gzhubu.top/gtugnomclc.html

(x * 2 for x in arr)
来源：http://hz.hnqzz.top/gthlzcozjg.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.dashuyun.cn/gtorymlgza.html

Counter(arr).most_common(3)
来源：http://hz.wangdashe.top/gtdjhghmfa.html

[U13] Py：固定长度队列
来源：http://hz.hnxiangtu.top/gtuunmuapz.html

deque(maxlen=10)
来源：http://hz.shzxlz.cn/gthnvofzoy.html

[U14] Py：分组收集到列表
来源：http://hz.316326.xyz/gtalngtrph.html

defaultdict(list)
来源：http://hz.redwolf501.top/gtxcijolbm.html

[U15] Py：高精度计时
来源：http://hz.chenzaomai.com/gtfmnacgsb.html

t = time.perf_counter()
来源：http://hz.hywenlv.cn/gtijkzeyon.html

[U16] Py：命令行参数解析
来源：http://hz.nanxuanxn.top/gtghaffeyd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.sweek.top/gtqxxxwimi.html

[U17] Py：初始化日志
来源：http://hz.smart0.xyz/gtdvfbniax.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.hysaishi.cn/gtkevpabls.html

[U18] Py：预编译正则
来源：http://hz.zhiwuduotai.top/gtjatmncco.html

pat = re.compile(r"\d+")
来源：http://hz.gzhubu.top/gthepejwhb.html

[U19] Py：正则替换带回调
来源：http://hz.wangshuangyany.cn/gtoikemfqp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.xingfuxueyuan.xyz/gtltyarjzo.html

[U20] Py：缓存函数结果
来源：http://hz.cheryme.top/gtvzpxugsg.html

@functools.lru_cache(maxsize=None)
来源：http://hz.haohaochexian.top/gtilbfyaen.html

[U21] Py：自定义上下文管理器
来源：http://hz.zhongyouzk.top/gtmstwdxlk.html

@contextlib.contextmanager
来源：http://hz.yj20258888.top/gtihrprbzu.html

[U22] Py：矩阵转置
来源：http://hz.andypj.xyz/gtgrcoxzjq.html

list(zip(*m))
来源：http://hz.yvedp.cn/gtnhcjgods.html

[U23] Py：分块读取大文件
来源：http://hz.nwbrower.top/gtmdxagtdh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.daria6918.cn/gttnxajozq.html

[U24] Py：路径操作
来源：http://hz.zhoulong.xyz/gtpojielcw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.jlsjyb.cn/gttfbxakqv.html

[U25] Py：CSV 按字典读
来源：http://hz.xylfe.cn/gtkdodlqta.html

csv.DictReader(f)
来源：http://hz.gogol.net.cn/gtbuhwrfql.html

[U26] Py：并发下载
来源：http://hz.jinqigufen.top/gtoplsrubp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.aizwys.cn/gtkgrzlkdr.html

[U27] Py：异步 HTTP
来源：http://hz.shzxlz.cn/gttmkxifmo.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.jianghu66.top/gtgcqauczb.html

[U28] Py：类型别名
来源：http://hz.cucudq.cn/gtmtnawdww.html

UserId = int
来源：http://hz.pycfn.com/gtmkqjesnx.html

[U29] Py：属性校验
来源：http://hz.ydjk.org.cn/gtazighxgy.html

@property 与 @x.setter 配合
来源：http://hz.svipenyu.cn/gtzdyluhzm.html

[U30] Py：数据类
来源：http://hz.fengsongda.top/gtwlyaxpgd.html

@dataclass(slots=True)
来源：http://hz.daria6918.cn/gtiqiexicf.html


<!-- 参考信息 -->