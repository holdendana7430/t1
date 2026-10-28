代发 wailian999

strlen(s)
来源：http://hz.nanxuanxn.top/gtxcwvapqo.html

[S06] C：字符串比较
来源：http://hz.iojbl.cn/gtzensqule.html

strcmp(a, b) == 0
来源：http://hz.tian-w.cn/gtcbvwpmtl.html

[S07] C：数组遍历求和
来源：http://hz.dianchejie.cn/gtxtpyqaxf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.chenlongwang.top/gtvmhrnivk.html

[S08] C：动态内存分配与释放
来源：http://hz.bjfxy.top/gtrweoeufs.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.nwbrower.top/gtrlpctmdb.html

[S09] C：结构体定义与初始化
来源：http://hz.jinghuilouyu.cn/gtccmtoxjd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jqgufenzy.top/gtxmwbzqzx.html

[S10] C：指针与解引用
来源：http://hz.hammf.cn/gtuavzhqky.html

int *p = &a;  *p = 5;
来源：http://hz.fzhhl.top/gtanmimlzt.html

[S11] C：逐行读文件
来源：http://hz.cashguo.top/gtzcxbcblt.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.quarkkingdee.top/gtxlycnpuz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ehwqpu.com/gtjwadvwrd.html

fclose(f);
来源：http://hz.smart0.xyz/gtznarroje.html

[S12] C：写文件
来源：http://hz.zhoulong.xyz/gtabsjijvc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.gogol.net.cn/gtzplqagis.html

[S13] C：宏定义
来源：http://hz.gaohongyu789.top/gtvokqtvne.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.redwolf501.top/gttuzpyxne.html

[S14] C：枚举
来源：http://hz.52xcode.cn/gtvquldyge.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhengqikj.top/gtimesxanj.html

[S15] C：类型转换
来源：http://hz.redwolf501.top/gtztrzbcso.html

(double) a / b
来源：http://hz.jqgfzy.top/gtumpsmxpf.html

[S16] C：位操作置位
来源：http://hz.jqgufenzy.top/gtehyvvcsl.html

x |= (1 << 3);
来源：http://hz.cashguo.top/gtbtzbsbdc.html

[S17] C：安全拼接字符串
来源：http://hz.nanxuanxn.top/gtizrzcfnv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yueranfly.top/gthchcpkcn.html

[S18] C：命令行参数
来源：http://hz.fzhhl.top/gtjvmfyunl.html

int main(int argc, char **argv)
来源：http://hz.zhaomingkeji.xyz/gtjcwxizhd.html

[S19] C：快速排序
来源：http://hz.hammf.cn/gtpsixshla.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zycfv.cn/gtzqcxsgze.html

[S20] C：二分查找
来源：http://hz.guowangkeji.top/gtiwmhgmgp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.0kj1m.cn/gtxqngyicr.html

[S21] C：字符类别判断
来源：http://hz.quarkkingdee.top/gtroyokins.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.haohaochexian.top/gttiowddpe.html

[S22] C：字符串转数字
来源：http://hz.yj20258888.top/gtekigndfr.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.meibo888.top/gtasysgxvu.html

[S23] C：随机数
来源：http://hz.zhijiandao.cn/gtkbtpmfzg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.guowangkeji.top/gtuhiqgtby.html

[S24] C：获取本地时间
来源：http://hz.yj20258888.top/gtscrncnup.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.dashuyun.cn/gtwsowejos.html

[S25] C：内存拷贝
来源：http://hz.jinyuanbaomall.cn/gtvbiwlhjd.html

memcpy(dst, src, n);
来源：http://hz.gogol.net.cn/gtqqvryogi.html

[S26] C：内存清零
来源：http://hz.iojbl.cn/gtcrqndkkl.html

memset(a, 0, sizeof a);
来源：http://hz.shanyushiyangtech.top/gtrfdbnswb.html

[S27] C：定义常量
来源：http://hz.yuxming.cn/gtovpfsaxb.html

const double PI = 3.14159;
来源：http://hz.zhengqikj.top/gtkpanhnyc.html

[S28] C：静态变量
来源：http://hz.xinyue.icu/gtpiayfeye.html

static int counter = 0;
来源：http://hz.pycfn.com/gtnddjntiz.html

[S29] C：变参函数
来源：http://hz.52xcode.cn/gtkqluzqns.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jqgfzy.top/gtdkokyilg.html

[S30] C：头文件保护
来源：http://hz.yuanzhike.top/gtlwtlkwxn.html

#ifndef X_H
来源：http://hz.zhijiandao.cn/gtkaiyrlfy.html

#define X_H
来源：http://hz.yj20258.top/gtujrpqbpy.html

#endif
来源：http://hz.cqqwz.cn/gtwgfpuycy.html

[S31] C++：Hello World
来源：http://hz.shangyingyoupin.top/gtscyfofdx.html

#include <iostream>
来源：http://hz.jlsjyb.cn/gttvcvvpoo.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.redwolf501.top/gtbcdgjqzi.html

[S32] C++：字符串
来源：http://hz.snrcjt.cn/gtxskjhtrp.html

std::string s = "hi";  s += "!";
来源：http://hz.pengpengdd.cyou/gtnyvmsoox.html

[S33] C++：vector 增删
来源：http://hz.vqdsnc.cn/gtqejcjwzy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.nwbrower.top/gtipdqqszf.html

[S34] C++：遍历 vector
来源：http://hz.yvedp.cn/gtyntsbgwn.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cqqwz.cn/gtzkgkrgjf.html

[S35] C++：map
来源：http://hz.yuanzhike.top/gtcrndgguc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.c1oappe.top/gtfrlgdqop.html

[S36] C++：unordered_map
来源：http://hz.xuanzx.com/gtfvdfpbup.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ehwqpu.com/gthmxstxia.html

[S37] C++：set
来源：http://hz.ywan-chungtsiang.top/gtbzlegdlt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yongpay.top/gtorwrfhog.html

[S38] C++：排序
来源：http://hz.tianlin.xyz/gtudxckjnw.html

std::sort(v.begin(), v.end());
来源：http://hz.vqdsnc.cn/gttltwxdgv.html

[S39] C++：自定义比较器排序
来源：http://hz.ywan-chungtsiang.top/gtfniirjcz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.xylfe.cn/gtxkntdjsz.html

[S40] C++：查找元素
来源：http://hz.xuanzx.com/gtbgpzdjyl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhaomingkeji.xyz/gtsdynfacx.html

[S41] C++：类与构造函数
来源：http://hz.ywan-chungtsiang.top/gtgqmkdvyt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.daxiang520.top/gtikttqecz.html

[S42] C++：继承与虚函数
来源：http://hz.yj20258888.top/gtkyzgrayd.html

class B : public Base { public: void f() override {} };
来源：http://hz.fzhhl.top/gtwpirjwqh.html

[S43] C++：智能指针
来源：http://hz.gaohongyu789.top/gtwrzrsxmp.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhiwuduotai.top/gteqtolixo.html

[S44] C++：引用传参
来源：http://hz.chenjidiqi.icu/gtmznnjfxd.html

void inc(int &x) { ++x; }
来源：http://hz.zhengqikj.top/gtjhzqkzkj.html

[S45] C++：lambda
来源：http://hz.andypj.xyz/gtkdddaewc.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.guannengcc.top/gtxdvabgrk.html

[S46] C++：函数模板
来源：http://hz.sweek.top/gtqapacnwc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.xziqi.cn/gtoilbftpf.html

[S47] C++：结构化绑定遍历
来源：http://hz.hnxiangtu.top/gtpddnxcwc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.shangyingyoupin.top/gtvejvsioy.html

[S48] C++：逐行读文件
来源：http://hz.yj20258888.top/gtajpbbwuy.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.ivvv.top/gtwrzdxbkk.html

while (std::getline(in, line)) { }
来源：http://hz.cucudq.cn/gteqkpucxu.html

[S49] C++：写文件
来源：http://hz.dashuyun.cn/gtyieyqsol.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.c1oappe.top/gticdtsaee.html

[S50] C++：格式化数字
来源：http://hz.nwbrower.top/gtmhvyvipl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.havefunace.top/gtwbjkqdfy.html

[S51] C++：显式类型转换
来源：http://hz.yuanzhike.top/gtsvhyjino.html

static_cast<double>(a) / b
来源：http://hz.xinyue.icu/gtarzxohwn.html

[S52] C++：const 与 noexcept
来源：http://hz.hnxiangtu.top/gtwszbauyz.html

int size() const noexcept { return n_; }
来源：http://hz.jinghuilouyu.cn/gtzrtugrsn.html

[S53] C++：移动语义
来源：http://hz.hammf.cn/gtwmhsrtip.html

std::vector<int> w = std::move(v);
来源：http://hz.nwbrower.top/gtkpmulouy.html

[S54] C++：异常处理
来源：http://hz.meibo888.top/gtnwugvptc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.vqdsnc.cn/gtzdjwmcmo.html

[S55] C++：结构化绑定
来源：http://hz.zhixingplan.top/gtncbmcxwu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhixingplan.top/gtnwaxrfth.html

[S56] C++：optional
来源：http://hz.zhijiandao.cn/gtokvsoybq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.wangdashe.top/gtzohaifba.html

[S57] C++：编译期常量
来源：http://hz.iojbl.cn/gtpcbcpgbi.html

constexpr int N = 10;
来源：http://hz.tian-w.cn/gtcoenilhx.html

[S58] C++：命名空间
来源：http://hz.9152youxi.cn/gtaprcglhd.html

namespace ns { int f() { return 1; } }
来源：http://hz.guannengcc.top/gtvnwjlkuc.html

[S59] C++：静态断言
来源：http://hz.nanxuanxn.top/gtiwvjwwud.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jinqigufen.top/gtuzajhwvk.html

[S60] C++：遍历并删除元素
来源：http://hz.vqdsnc.cn/gtfawdbodz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.iojbl.cn/gtgqjvvuhu.html

================================================================================
来源：http://hz.meibo888.top/gtaeunvfxy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cqqwz.cn/gtautzrqjt.html

================================================================================
来源：http://hz.hnqzz.top/gtdaoqurno.html

[T01] Kotlin：Hello World
来源：http://hz.snrcjt.cn/gtojxwvpwj.html

println("Hello")
来源：http://hz.gaohongyu789.top/gtzfekgmju.html

[T02] Kotlin：变量
来源：http://hz.jlsjyb.cn/gtnjnqleae.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hfpthk.cn/gtigrimhzv.html

[T03] Kotlin：字符串模板
来源：http://hz.fengsongda.top/gtckctmsmn.html

"值: $b"
来源：http://hz.bjfxy.top/gtswaqlwzu.html

[T04] Kotlin：空安全
来源：http://hz.xinyue.icu/gtxjifukek.html

val n: String? = null;  n?.length
来源：http://hz.chenzaomai.com/gtcksmfbzc.html

[T05] Kotlin：when 表达式
来源：http://hz.jqgufenzy.top/gtxbjpuhya.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.0kj1m.cn/gtvilnpsvt.html

[T06] Kotlin：集合映射
来源：http://hz.zhixingplan.top/gtzechquij.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hnxiangtu.top/gtvbhhtvdd.html

[T07] Kotlin：集合过滤
来源：http://hz.ydzc1.top/gtwyhmqmng.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhengqikj.top/gthqwjwogh.html

[T08] Kotlin：数据类
来源：http://hz.gaohongyu789.top/gtflknikvi.html

data class User(val name: String, val age: Int)
来源：http://hz.yangfankeji.com/gtaxqtcdma.html

[T09] Kotlin：扩展函数
来源：http://hz.zhengqikj.top/gtyuyoojgt.html

fun String.exclaim() = this + "!"
来源：http://hz.zycfv.cn/gtmmifzxer.html

[T10] Kotlin：默认参数
来源：http://hz.sxryk.cn/gtrelcmcqb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.gogol.net.cn/gtlegikevp.html

[T11] Kotlin：协程
来源：http://hz.zhixingplan.top/gtmnuyrpix.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.aibaodan.cn/gtqzudcyaz.html

[T12] Kotlin：解构声明
来源：http://hz.gaohongyu789.top/gtlluqmjen.html

val (a, b) = Pair(1, 2)
来源：http://hz.iojbl.cn/gtgszsqhip.html

[T13] Kotlin：只读 Map
来源：http://hz.fzhhl.top/gtkjlnvpfs.html

val m = mapOf("a" to 1)
来源：http://hz.feifeiyinyue.top/gtwngpabab.html

[T14] Kotlin：循环
来源：http://hz.haohaochexian.top/gtqrrnqocm.html

for (i in 1..10) println(i)
来源：http://hz.jqgufenzy.top/gtpjebsxtb.html

[T15] Kotlin：接口
来源：http://hz.jianghu66.top/gtupfbwpmy.html

interface Shape { fun area(): Double }
来源：http://hz.hysaishi.cn/gtvypukzge.html

[T16] Swift：Hello World
来源：http://hz.jinghuilouyu.cn/gtwhtlzjtz.html

print("Hello")
来源：http://hz.birdmap.top/gtmgcvfgdi.html

[T17] Swift：变量与常量
来源：http://hz.cqqwz.cn/gtambqvpgr.html

var a = 1;  let b = 2
来源：http://hz.iojbl.cn/gtpiuxtgip.html

[T18] Swift：字符串插值
来源：http://hz.hongshengwenyu.top/gtypinjtez.html

"值: \(b)"
来源：http://hz.guowangkeji.top/gtxtshjuba.html

[T19] Swift：可选绑定
来源：http://hz.gogol.net.cn/gtvglkncmf.html

if let n = opt { print(n) }
来源：http://hz.ybcxt.top/gtwzfrnkxh.html

[T20] Swift：数组操作
来源：http://hz.hammf.cn/gtrhpkjydt.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.fzhhl.top/gtznchvfsl.html

[T21] Swift：遍历
来源：http://hz.jqgfzy.top/gtgtniyulz.html

for x in a { print(x) }
来源：http://hz.aibaodan.cn/gtttdpkitz.html

[T22] Swift：字典
来源：http://hz.zhengqikj.top/gtvsefxlba.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.shzxlz.cn/gtoohgalcn.html

[T23] Swift：函数
来源：http://hz.xziqi.cn/gtgdbliztq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.guannengcc.top/gttynzkcml.html

[T24] Swift：闭包
来源：http://hz.meibo888.top/gtoiiqbbmt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.xuetiantiany.cn/gtrgotnyll.html

[T25] Swift：结构体
来源：http://hz.xziqi.cn/gtxfmbrcnr.html

struct P { var x: Int }
来源：http://hz.daxiang520.top/gtajrqohfh.html

[T26] Swift：类与重写
来源：http://hz.wangdashe.top/gtpppjminf.html

class A: Base { override func f() {} }
来源：http://hz.guowangkeji.top/gtafyhzjdp.html

[T27] Swift：错误处理
来源：http://hz.gzhubu.top/gtezmrmdzo.html

do { try f() } catch { print(error) }
来源：http://hz.jqgfzy.top/gtvlemepzh.html

[T28] Swift：枚举
来源：http://hz.jinqigfzy.top/gtvweojauc.html

enum Color { case red, green }
来源：http://hz.ywan-chungtsiang.top/gtgjmbhopw.html

[T29] Swift：guard 提前返回
来源：http://hz.ehwqpu.com/gtpvsbrprv.html

guard let x = opt else { return }
来源：http://hz.dashuyun.cn/gtrnnyduyz.html

[T30] Swift：协议
来源：http://hz.yj20258888.top/gtxrthkikq.html

protocol Shape { func area() -> Double }
来源：http://hz.316326.xyz/gtvthcbvrh.html

[T31] Lua：Hello World
来源：http://hz.guannengcc.top/gturwghhzc.html

print("Hello")
来源：http://hz.ydzc1.top/gtxnvfwlaj.html

[T32] Lua：局部变量
来源：http://hz.xingfuxueyuan.xyz/gtiriwccqa.html

local a = 1
来源：http://hz.chenlongwang.top/gtnvkyizni.html

[T33] Lua：表（数组）
来源：http://hz.dianchejie.cn/gtztudoznj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.snrcjt.cn/gtciwjvusr.html

[T34] Lua：遍历表
来源：http://hz.pengpengdd.cyou/gtfcibjunk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yj202588.top/gtqosdnlpd.html

[T35] Lua：字典表
来源：http://hz.redwolf501.top/gtlithsiwp.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yongpay.top/gtsmcnbecx.html

[T36] Lua：函数
来源：http://hz.shanyushiyangkeji.top/gttsthzpof.html

function add(a, b) return a + b end
来源：http://hz.yanxiufei.cn/gtkymndpwu.html

[T37] Lua：字符串拼接
来源：http://hz.zdqjudy.top/gtjvnzmlia.html

"a" .. "b"
来源：http://hz.svipenyu.cn/gtqnmevmqi.html

[T38] Lua：条件
来源：http://hz.nanxinkj.top/gtbjeoniax.html

if x > 0 then print("正") end
来源：http://hz.9152youxi.cn/gtgktpiywq.html

[T39] Lua：模式匹配
来源：http://hz.yj20258.top/gtglaymodx.html

string.find(s, "%d+")
来源：http://hz.chenjidiqi.icu/gtsdujwzrq.html

[T40] Lua：元表
来源：http://hz.pengpengdd.cyou/gtedykgeoh.html

setmetatable({}, { __index = base })
来源：http://hz.ppjwa.cn/gtnjtlhiim.html

[T41] Perl：Hello World
来源：http://hz.redwolf501.top/gteqktijfg.html

print "Hello\n";
来源：http://hz.snrcjt.cn/gtqbnodguy.html

[T42] Perl：变量类型
来源：http://hz.ywan-chungtsiang.top/gtorjokxdy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yongpay.top/gtzuzladda.html

[T43] Perl：字符串插值
来源：http://hz.xuetiantiany.cn/gtfcgrrvqk.html

"值: $a"
来源：http://hz.ivvv.top/gtcnlnkrhl.html

[T44] Perl：条件
来源：http://hz.yj202588.top/gtknwewkyo.html

if ($a > 0) { print "正"; }
来源：http://hz.redwolf501.top/gtxuyyicrp.html

[T45] Perl：数组遍历
来源：http://hz.hnxiangtu.top/gtkgiomrsz.html

for my $x (@arr) { print $x; }
来源：http://hz.jiagoushi.top/gtgsllssyq.html

[T46] Perl：哈希操作
来源：http://hz.9152youxi.cn/gtxchksrsh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.nwbrower.top/gtqlcmhjvn.html

[T47] Perl：正则捕获
来源：http://hz.yangfankeji.com/gtihuqeeer.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.shuidangran.top/gtpwiuxcdf.html

[T48] Perl：正则替换
来源：http://hz.daxiang520.top/gthmxsbajw.html

$s =~ s/old/new/g;
来源：http://hz.guowangkeji.top/gtnlvqlpyk.html

[T49] Perl：函数
来源：http://hz.xingfuxueyuan.xyz/gtxpizdfuw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.quarkkingdee.top/gtrjsgrssd.html

[T50] Perl：逐行读文件
来源：http://hz.pengpengdd.cyou/gtlsgqeefm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yangfankeji.com/gtyyknjsvi.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yj202588.top/gtjrovvqdv.html

[T51] Scala：Hello World
来源：http://hz.wangdashe.top/gtaeaafpqx.html

println("Hello")
来源：http://hz.dashuyun.cn/gtppacjdtx.html

[T52] Scala：变量
来源：http://hz.jinqigufen.top/gtyarolwvo.html

val a = 1;  var b = 2
来源：http://hz.vqdsnc.cn/gtgbwmdkxt.html

[T53] Scala：字符串插值
来源：http://hz.gogol.net.cn/gttifujfrd.html

s"值: $b"
来源：http://hz.bjfxy.top/gtqskudlss.html

[T54] Scala：集合映射
来源：http://hz.9152youxi.cn/gtyffmgqjx.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.snrcjt.cn/gtjtemshzu.html

[T55] Scala：集合过滤
来源：http://hz.fengsongda.top/gtaddhqfuy.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jqgufenzy.top/gtfiucuqib.html

[T56] Scala：样例类
来源：http://hz.tanke756.top/gtqisiwiwr.html

case class User(name: String, age: Int)
来源：http://hz.hammf.cn/gthebgqkvb.html

[T57] Scala：模式匹配
来源：http://hz.jinqigufen.top/gthbwoiaui.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hfpthk.cn/gtjtstrqdc.html

[T58] Scala：函数定义
来源：http://hz.guannengcc.top/gtykfcrkkf.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yj20258.top/gtzqymsdmv.html

[T59] Scala：循环
来源：http://hz.jiagoushi.top/gtylrsfape.html

for (i <- 1 to 10) println(i)
来源：http://hz.gaohongyu789.top/gtfqqgatja.html

[T60] Scala：折叠
来源：http://hz.ydzc1.top/gtzagccydi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.xuetiantiany.cn/gtdhizuzht.html

================================================================================
来源：http://hz.hnxiangtu.top/gtuyhyzjke.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.xinyue.icu/gtquxwshsc.html

================================================================================
来源：http://hz.zhijiandao.cn/gtgoscmdfq.html

[U01] Py：创建虚拟环境
来源：http://hz.smart0.xyz/gtbpltkqwt.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.9152youxi.cn/gtjqxflnzy.html

[U02] Py：导出 / 安装依赖
来源：http://hz.wangshuangyany.cn/gtqbxvdsdo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.iojbl.cn/gtnpbjmgqt.html

[U03] Py：加载 .env 配置
来源：http://hz.havefunace.top/gtqszygcvc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.xziqi.cn/gtwxpvdffv.html

[U04] Py：变量调试打印
来源：http://hz.hnqzz.top/gtmaqiydig.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.wangdashe.top/gtlxmjyrlj.html

[U05] Py：列表去重且保序
来源：http://hz.chenjidiqi.icu/gtvyksubxx.html

list(dict.fromkeys(arr))
来源：http://hz.aibaodan.cn/gtaonyxodp.html

[U06] Py：合并两个字典
来源：http://hz.jinyuanbaomall.cn/gtyhdoqllb.html

{**a, **b}
来源：http://hz.smart0.xyz/gtxpyyhvwr.html

[U07] Py：反转字典键值
来源：http://hz.guowangkeji.top/gtixxmpmxt.html

{v: k for k, v in d.items()}
来源：http://hz.gzhubu.top/gtdpyygolq.html

[U08] Py：展平二维列表
来源：http://hz.feifeiyinyue.top/gtmmmxcncm.html

[y for x in nested for y in x]
来源：http://hz.hnxiangtu.top/gtofplptrb.html

[U09] Py：字典取最大值的键
来源：http://hz.yvedp.cn/gtvawxqhsg.html

max(d, key=d.get)
来源：http://hz.hfpthk.cn/gtxnhbrqph.html

[U10] Py：按值排序字典
来源：http://hz.yongpay.top/gtryzjhuyi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.iojbl.cn/gtoctacnbg.html

[U11] Py：生成器表达式
来源：http://hz.xingfuxueyuan.xyz/gtutxluqiu.html

(x * 2 for x in arr)
来源：http://hz.ydzc1.top/gtyxccxkiz.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.tianlin.xyz/gtgbfjlqww.html

Counter(arr).most_common(3)
来源：http://hz.xylfe.cn/gtpraaygsu.html

[U13] Py：固定长度队列
来源：http://hz.dashuyun.cn/gtgzcssxgr.html

deque(maxlen=10)
来源：http://hz.yj20258.top/gtwgtjyaix.html

[U14] Py：分组收集到列表
来源：http://hz.nanxinkj.top/gtiytaoqod.html

defaultdict(list)
来源：http://hz.iojbl.cn/gtbyrkahhr.html

[U15] Py：高精度计时
来源：http://hz.gotoacloud.top/gtwjyslzld.html

t = time.perf_counter()
来源：http://hz.meibo888.top/gtmrnqudul.html

[U16] Py：命令行参数解析
来源：http://hz.jianghu66.top/gtpkdeiehy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yuanzhike.top/gtaxtetjtz.html

[U17] Py：初始化日志
来源：http://hz.chenjidiqi.icu/gtttxotxwm.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.zhengqikj.top/gtrbcjgjoi.html

[U18] Py：预编译正则
来源：http://hz.chenjidiqi.icu/gtqnkfowwn.html

pat = re.compile(r"\d+")
来源：http://hz.gaohongyu789.top/gtrjzzzacz.html

[U19] Py：正则替换带回调
来源：http://hz.hongshengwenyu.top/gtjjgmpzuw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.gzhubu.top/gtbklqouzm.html

[U20] Py：缓存函数结果
来源：http://hz.sufxvd.cn/gtgfaxwacl.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jqgufenzy.top/gtuuofngfu.html

[U21] Py：自定义上下文管理器
来源：http://hz.shanyushiyangkeji.top/gtkqfjdeng.html

@contextlib.contextmanager
来源：http://hz.guowangkeji.top/gtoqnincji.html

[U22] Py：矩阵转置
来源：http://hz.cqqwz.cn/gtnocwuowr.html

list(zip(*m))
来源：http://hz.yangfankeji.com/gtfblvijey.html

[U23] Py：分块读取大文件
来源：http://hz.shzxlz.cn/gtphezyajq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.shuidangran.top/gtdwdeyjgc.html

[U24] Py：路径操作
来源：http://hz.bjfxy.top/gtgcbfcsiw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.ybcxt.top/gtwwavzkzd.html

[U25] Py：CSV 按字典读
来源：http://hz.snrcjt.cn/gtxoucholz.html

csv.DictReader(f)
来源：http://hz.shzxlz.cn/gtrlewzjcz.html

[U26] Py：并发下载
来源：http://hz.jqgufenzy.top/gtcacdacxg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.chenjidiqi.icu/gtjibyqzaa.html

[U27] Py：异步 HTTP
来源：http://hz.yj20258888.top/gtqtjwccgy.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.smart0.xyz/gtongtbcrr.html

[U28] Py：类型别名
来源：http://hz.yongpay.top/gtgxkspqqd.html

UserId = int
来源：http://hz.zhoulong.xyz/gtxssbppmg.html


<!-- 参考信息 -->