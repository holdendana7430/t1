代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.gotoacloud.top/gtplrvdbse.html

[S10] C：指针与解引用
来源：http://hz.gaohongyu789.top/gteqralrtg.html

int *p = &a;  *p = 5;
来源：http://hz.jqgfzy.top/gtxaxbtldc.html

[S11] C：逐行读文件
来源：http://hz.jlsjyb.cn/gtielfogie.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ydjk.org.cn/gtgcavkcgc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhijiandao.cn/gtdjdxqcex.html

fclose(f);
来源：http://hz.zhixingplan.top/gtvbjxuibh.html

[S12] C：写文件
来源：http://hz.birdmap.top/gtdrzrfots.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.daria6918.cn/gthmdklgoe.html

[S13] C：宏定义
来源：http://hz.sysykeji.top/gtibuwcbce.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.sxryk.cn/gtvncvlyjr.html

[S14] C：枚举
来源：http://hz.shangyingyoupin.top/gtzopfpwdu.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hfpthk.cn/gtfepomejc.html

[S15] C：类型转换
来源：http://hz.vqdsnc.cn/gtqjonuflz.html

(double) a / b
来源：http://hz.iojbl.cn/gtyyzrkdpk.html

[S16] C：位操作置位
来源：http://hz.meibo888.top/gtyqceoefu.html

x |= (1 << 3);
来源：http://hz.sxryk.cn/gtbjjpwcqi.html

[S17] C：安全拼接字符串
来源：http://hz.yonumen.top/gtpkycstfl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yj202588.top/gtmrogxhlx.html

[S18] C：命令行参数
来源：http://hz.hammf.cn/gteimvgwav.html

int main(int argc, char **argv)
来源：http://hz.ybcxt.top/gthyvjqwyo.html

[S19] C：快速排序
来源：http://hz.ehwqpu.com/gtporbszxw.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.kuanghao11.cn/gtytrgfvho.html

[S20] C：二分查找
来源：http://hz.yuanzhike.top/gtjanelpgb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ydzc1.top/gtgmbvdizk.html

[S21] C：字符类别判断
来源：http://hz.cheryme.top/gthvzldgtk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.shuidangran.top/gtoxjwzxwz.html

[S22] C：字符串转数字
来源：http://hz.hammf.cn/gtiehvomgm.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.andypj.xyz/gtfebcifgt.html

[S23] C：随机数
来源：http://hz.ppjwa.cn/gtuibawium.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.sysykeji.top/gtdotmrttz.html

[S24] C：获取本地时间
来源：http://hz.zhaomingkeji.xyz/gtjmuzjthb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.redwolf501.top/gtkylzdzen.html

[S25] C：内存拷贝
来源：http://hz.cashguo.top/gtkhajbvmj.html

memcpy(dst, src, n);
来源：http://hz.havefunace.top/gtrykedplh.html

[S26] C：内存清零
来源：http://hz.birdmap.top/gtqbcmhaip.html

memset(a, 0, sizeof a);
来源：http://hz.hnxiangtu.top/gtpsddfkaz.html

[S27] C：定义常量
来源：http://hz.zhoulong.xyz/gtmdxtzwfu.html

const double PI = 3.14159;
来源：http://hz.bjfxy.top/gtblayjkay.html

[S28] C：静态变量
来源：http://hz.gzhubu.top/gtujdlrtow.html

static int counter = 0;
来源：http://hz.9152youxi.cn/gthepxtocn.html

[S29] C：变参函数
来源：http://hz.cheryme.top/gtikyjiefg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ywan-chungtsiang.top/gtdawlcdzn.html

[S30] C：头文件保护
来源：http://hz.wangshuangyany.cn/gtmmhvfwkk.html

#ifndef X_H
来源：http://hz.gogol.net.cn/gtagndjsiu.html

#define X_H
来源：http://hz.sweek.top/gtjfxgpchz.html

#endif
来源：http://hz.ydzc1.top/gtkdqhpwyg.html

[S31] C++：Hello World
来源：http://hz.sufxvd.cn/gtzlhkufcz.html

#include <iostream>
来源：http://hz.shzxlz.cn/gtxtesqmyg.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hysaishi.cn/gtzqbxrvdn.html

[S32] C++：字符串
来源：http://hz.jqgfzy.top/gtygsgekrk.html

std::string s = "hi";  s += "!";
来源：http://hz.aibaodan.cn/gtjlddkjvt.html

[S33] C++：vector 增删
来源：http://hz.cqqwz.cn/gtfkivclat.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yonumen.top/gtuabnaxsw.html

[S34] C++：遍历 vector
来源：http://hz.0kj1m.cn/gthjtwvaiz.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cucudq.cn/gtkqxkgcqh.html

[S35] C++：map
来源：http://hz.tian-w.cn/gtgqkmzxul.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hfpthk.cn/gtmkwrcbyr.html

[S36] C++：unordered_map
来源：http://hz.yj20258888.top/gttvqphebs.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sxryk.cn/gtxocdapvg.html

[S37] C++：set
来源：http://hz.sufxvd.cn/gtcslcaibp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xuanzx.com/gteykujkix.html

[S38] C++：排序
来源：http://hz.feifeiyinyue.top/gtszkgqrkr.html

std::sort(v.begin(), v.end());
来源：http://hz.zdqjudy.top/gttuujegoz.html

[S39] C++：自定义比较器排序
来源：http://hz.hnxiangtu.top/gtfbrjkavo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.wangdashe.top/gtgvoogkov.html

[S40] C++：查找元素
来源：http://hz.yj20258.top/gtbufkbliu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jyoumei.cn/gttilnyhya.html

[S41] C++：类与构造函数
来源：http://hz.aibaodan.cn/gtnzyhuobw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhaomingkeji.xyz/gtweotzmex.html

[S42] C++：继承与虚函数
来源：http://hz.hfpthk.cn/gtzyziyucp.html

class B : public Base { public: void f() override {} };
来源：http://hz.feifeiyinyue.top/gtfzfeyxac.html

[S43] C++：智能指针
来源：http://hz.hammf.cn/gtmgsfbryh.html

auto p = std::make_unique<int>(5);
来源：http://hz.yangfankeji.com/gtpoznvdla.html

[S44] C++：引用传参
来源：http://hz.xinyue.icu/gtfmztvfrs.html

void inc(int &x) { ++x; }
来源：http://hz.jlsjyb.cn/gtsovthhro.html

[S45] C++：lambda
来源：http://hz.gaohongyu789.top/gtdbtzhjxy.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yanxiufei.cn/gtyprhhkrz.html

[S46] C++：函数模板
来源：http://hz.wangdashe.top/gthkjmzzrq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.gotoacloud.top/gtjztjfehz.html

[S47] C++：结构化绑定遍历
来源：http://hz.nanxinkj.top/gtlisqrcfw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhijiandao.cn/gtbcfiaxaq.html

[S48] C++：逐行读文件
来源：http://hz.zhixingplan.top/gtbzschynq.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.hnxiangtu.top/gthptxwujv.html

while (std::getline(in, line)) { }
来源：http://hz.xuetiantiany.cn/gthiirqqaw.html

[S49] C++：写文件
来源：http://hz.sysykeji.top/gtfqtpykuq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.smart0.xyz/gthdfwwjmi.html

[S50] C++：格式化数字
来源：http://hz.bjfxy.top/gtvpuamkzr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.gogol.net.cn/gtlhbtzdeh.html

[S51] C++：显式类型转换
来源：http://hz.nwbrower.top/gtxdefrwxu.html

static_cast<double>(a) / b
来源：http://hz.zhongyouzk.top/gtkwoulyty.html

[S52] C++：const 与 noexcept
来源：http://hz.yonumen.top/gtdoftjwue.html

int size() const noexcept { return n_; }
来源：http://hz.yj202588.top/gtyrstswja.html

[S53] C++：移动语义
来源：http://hz.ywan-chungtsiang.top/gtfefwbpga.html

std::vector<int> w = std::move(v);
来源：http://hz.hnxiangtu.top/gttmmryohl.html

[S54] C++：异常处理
来源：http://hz.guowangkeji.top/gtgrgjbpgh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.andypj.xyz/gtijlklmyn.html

[S55] C++：结构化绑定
来源：http://hz.c1oappe.top/gtjhutfmxj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.shzxlz.cn/gtlcfqdfvu.html

[S56] C++：optional
来源：http://hz.jianghu66.top/gtzahzfvkt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yongpay.top/gtxpctlgcc.html

[S57] C++：编译期常量
来源：http://hz.iojbl.cn/gtgrfembda.html

constexpr int N = 10;
来源：http://hz.zhongyouzk.top/gtuxrplgtu.html

[S58] C++：命名空间
来源：http://hz.nwbrower.top/gtfhvwkaha.html

namespace ns { int f() { return 1; } }
来源：http://hz.0kj1m.cn/gtlmqndtgx.html

[S59] C++：静态断言
来源：http://hz.zhengqikj.top/gtjwmrktis.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.tianlin.xyz/gtcwuyjcjq.html

[S60] C++：遍历并删除元素
来源：http://hz.yuxming.cn/gtopvmxkzb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jianghu66.top/gtaqdrvhxr.html

================================================================================
来源：http://hz.yj20258888.top/gtatystdrq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.gotoacloud.top/gtxxzwunfl.html

================================================================================
来源：http://hz.yj202588.top/gtdatufxcz.html

[T01] Kotlin：Hello World
来源：http://hz.jyoumei.cn/gtgedtfxze.html

println("Hello")
来源：http://hz.shzxlz.cn/gttexlbxme.html

[T02] Kotlin：变量
来源：http://hz.ybcxt.top/gtriyxzpgm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.fengsongda.top/gtlijvqscu.html

[T03] Kotlin：字符串模板
来源：http://hz.zdqjudy.top/gtkhlkirfu.html

"值: $b"
来源：http://hz.xingfuxueyuan.xyz/gtddmtzouw.html

[T04] Kotlin：空安全
来源：http://hz.ppjwa.cn/gtuxtjvieh.html

val n: String? = null;  n?.length
来源：http://hz.sysykeji.top/gtlkuvrrms.html

[T05] Kotlin：when 表达式
来源：http://hz.cqqwz.cn/gtzpuslqcg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yuxming.cn/gtgcxqzqjz.html

[T06] Kotlin：集合映射
来源：http://hz.xingfuxueyuan.xyz/gtqnqmcanv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.cdnleiting.top/gtnsuecbgk.html

[T07] Kotlin：集合过滤
来源：http://hz.andypj.xyz/gttsyqbynz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.chenlongwang.top/gthxlnoonf.html

[T08] Kotlin：数据类
来源：http://hz.yuxming.cn/gttlwxjvvh.html

data class User(val name: String, val age: Int)
来源：http://hz.tianlin.xyz/gtcjmjjsjm.html

[T09] Kotlin：扩展函数
来源：http://hz.kuanghao11.cn/gtzlccalag.html

fun String.exclaim() = this + "!"
来源：http://hz.zhoulong.xyz/gtmxnxojzs.html

[T10] Kotlin：默认参数
来源：http://hz.redwolf501.top/gtliclskws.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yvedp.cn/gtgqlivhkz.html

[T11] Kotlin：协程
来源：http://hz.shuidangran.top/gtfthddrlk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.guowangkeji.top/gticgvhcva.html

[T12] Kotlin：解构声明
来源：http://hz.daria6918.cn/gtywqlemaz.html

val (a, b) = Pair(1, 2)
来源：http://hz.vqdsnc.cn/gtypidepay.html

[T13] Kotlin：只读 Map
来源：http://hz.zhongyouzk.top/gtmihekexe.html

val m = mapOf("a" to 1)
来源：http://hz.hysaishi.cn/gtkvbjagqg.html

[T14] Kotlin：循环
来源：http://hz.yj20258888.top/gtbfleqdkc.html

for (i in 1..10) println(i)
来源：http://hz.shangyingyoupin.top/gtpjbuqfwu.html

[T15] Kotlin：接口
来源：http://hz.zhongyouzk.top/gtcrxkozwn.html

interface Shape { fun area(): Double }
来源：http://hz.dianchejie.cn/gthnunqwxh.html

[T16] Swift：Hello World
来源：http://hz.pycfn.com/gtgailzzdi.html

print("Hello")
来源：http://hz.tianlin.xyz/gtbcncwsbp.html

[T17] Swift：变量与常量
来源：http://hz.nanxinkj.top/gtverklwqf.html

var a = 1;  let b = 2
来源：http://hz.dashuyun.cn/gtwyuxtqtu.html

[T18] Swift：字符串插值
来源：http://hz.hywenlv.cn/gtzvxzlpgx.html

"值: \(b)"
来源：http://hz.bjfxy.top/gtdibkwjor.html

[T19] Swift：可选绑定
来源：http://hz.nanxuanxn.top/gtwlrvlqwv.html

if let n = opt { print(n) }
来源：http://hz.tian-w.cn/gtwiowjstj.html

[T20] Swift：数组操作
来源：http://hz.cheryme.top/gtjebouirb.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zhixingplan.top/gtkheuynci.html

[T21] Swift：遍历
来源：http://hz.jqgufenzy.top/gthqqgwpjj.html

for x in a { print(x) }
来源：http://hz.hongshengwenyu.top/gtfsihqdnv.html

[T22] Swift：字典
来源：http://hz.cashguo.top/gtkifvutoj.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.cdnleiting.top/gtpvhvocpt.html

[T23] Swift：函数
来源：http://hz.ehwqpu.com/gtfnldqdxr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.guannengcc.top/gtwnsqsdai.html

[T24] Swift：闭包
来源：http://hz.sxryk.cn/gtxuijkjfb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.meibo888.top/gtcuiyafgg.html

[T25] Swift：结构体
来源：http://hz.0kj1m.cn/gtvenynjia.html

struct P { var x: Int }
来源：http://hz.chenlongwang.top/gtlyrpobgz.html

[T26] Swift：类与重写
来源：http://hz.snrcjt.cn/gtudwkfnst.html

class A: Base { override func f() {} }
来源：http://hz.tianlin.xyz/gttffoptka.html

[T27] Swift：错误处理
来源：http://hz.pycfn.com/gtbavznqag.html

do { try f() } catch { print(error) }
来源：http://hz.xziqi.cn/gtkpaszrjh.html

[T28] Swift：枚举
来源：http://hz.bjfxy.top/gtfswywhvc.html

enum Color { case red, green }
来源：http://hz.yj20258.top/gtwhnwjnzg.html

[T29] Swift：guard 提前返回
来源：http://hz.gzhubu.top/gtmjnjjqbd.html

guard let x = opt else { return }
来源：http://hz.guowangkeji.top/gtxcifxaox.html

[T30] Swift：协议
来源：http://hz.chenlongwang.top/gtgoplipwa.html

protocol Shape { func area() -> Double }
来源：http://hz.daxiang520.top/gtoocrbcmz.html

[T31] Lua：Hello World
来源：http://hz.wangshuangyany.cn/gtafsptqju.html

print("Hello")
来源：http://hz.yueranfly.top/gtatwbajzi.html

[T32] Lua：局部变量
来源：http://hz.hnxiangtu.top/gttqeiicjg.html

local a = 1
来源：http://hz.9152youxi.cn/gtvsqmjguy.html

[T33] Lua：表（数组）
来源：http://hz.316326.xyz/gtfgdrgjau.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.daxiang520.top/gtnbzmrioh.html

[T34] Lua：遍历表
来源：http://hz.yueranfly.top/gtblenqsol.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jinqigufen.top/gtdbcaxkao.html

[T35] Lua：字典表
来源：http://hz.yuanzhike.top/gtbdezrzhy.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yongpay.top/gtboqpzcbo.html

[T36] Lua：函数
来源：http://hz.hysaishi.cn/gtjhaligjy.html

function add(a, b) return a + b end
来源：http://hz.xziqi.cn/gtgqeefdlt.html

[T37] Lua：字符串拼接
来源：http://hz.gzhubu.top/gtozovidhp.html

"a" .. "b"
来源：http://hz.quarkkingdee.top/gttutjjdgn.html

[T38] Lua：条件
来源：http://hz.fengsongda.top/gtvygszfyz.html

if x > 0 then print("正") end
来源：http://hz.shanyushiyangtech.top/gtuiwvgnag.html

[T39] Lua：模式匹配
来源：http://hz.nanxuanxn.top/gtvtdnxtwq.html

string.find(s, "%d+")
来源：http://hz.zycfv.cn/gtrszqzviw.html

[T40] Lua：元表
来源：http://hz.birdmap.top/gtzizqcbas.html

setmetatable({}, { __index = base })
来源：http://hz.gogol.net.cn/gtrmravxjn.html

[T41] Perl：Hello World
来源：http://hz.52xcode.cn/gtysztfvgl.html

print "Hello\n";
来源：http://hz.ywan-chungtsiang.top/gtzyvuexek.html

[T42] Perl：变量类型
来源：http://hz.yueranfly.top/gtsmsixkcf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.haohaochexian.top/gtvylgqrvb.html

[T43] Perl：字符串插值
来源：http://hz.shangyingyoupin.top/gtmjylfllm.html

"值: $a"
来源：http://hz.shanyushiyangkeji.top/gtavjyukyx.html

[T44] Perl：条件
来源：http://hz.yonumen.top/gtuxzkoqoj.html

if ($a > 0) { print "正"; }
来源：http://hz.ydjk.org.cn/gtlcdozsvc.html

[T45] Perl：数组遍历
来源：http://hz.hnxiangtu.top/gthzimuxww.html

for my $x (@arr) { print $x; }
来源：http://hz.kuanghao11.cn/gtzukttiqs.html

[T46] Perl：哈希操作
来源：http://hz.fengsongda.top/gtxnxgbykh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.meibo888.top/gtnpptimfh.html

[T47] Perl：正则捕获
来源：http://hz.shuidangran.top/gtjaxneeci.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.aizwys.cn/gtnvmmftql.html

[T48] Perl：正则替换
来源：http://hz.jianghu66.top/gtrlzykyxj.html

$s =~ s/old/new/g;
来源：http://hz.redwolf501.top/gtsfqkfate.html

[T49] Perl：函数
来源：http://hz.birdmap.top/gttehqhdra.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.wangshuangyany.cn/gtaaxqyyuf.html

[T50] Perl：逐行读文件
来源：http://hz.tian-w.cn/gtvuleagfy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.snrcjt.cn/gtbxtgpscg.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.sxryk.cn/gtgjjrcjir.html

[T51] Scala：Hello World
来源：http://hz.yongpay.top/gtgbzwbnly.html

println("Hello")
来源：http://hz.ybcxt.top/gtkykllxwh.html

[T52] Scala：变量
来源：http://hz.sysykeji.top/gtodyfwhyd.html

val a = 1;  var b = 2
来源：http://hz.zycfv.cn/gtpcdonphu.html

[T53] Scala：字符串插值
来源：http://hz.xuanzx.com/gtokqvsjma.html

s"值: $b"
来源：http://hz.wangshuangyany.cn/gtiouqagle.html

[T54] Scala：集合映射
来源：http://hz.tanke756.top/gtysowylvm.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yuanzhike.top/gtcijudrtn.html

[T55] Scala：集合过滤
来源：http://hz.tianlin.xyz/gtkorqphgj.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.zhijiandao.cn/gtdntjublf.html

[T56] Scala：样例类
来源：http://hz.chenzaomai.com/gtkvvmggek.html

case class User(name: String, age: Int)
来源：http://hz.yonumen.top/gtebborybk.html

[T57] Scala：模式匹配
来源：http://hz.guowangkeji.top/gtzzfcqcmb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.daxiang520.top/gtzxmcigjv.html

[T58] Scala：函数定义
来源：http://hz.bjfxy.top/gtcqytsxfv.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.xingfuxueyuan.xyz/gtnlhogaqw.html

[T59] Scala：循环
来源：http://hz.yonumen.top/gtsvohizqk.html

for (i <- 1 to 10) println(i)
来源：http://hz.gaohongyu789.top/gttqqfrolg.html

[T60] Scala：折叠
来源：http://hz.iojbl.cn/gtappmnbok.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hfpthk.cn/gtvfvefkqs.html

================================================================================
来源：http://hz.aizwys.cn/gtdbuhcpki.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.9152youxi.cn/gtgomsfxhj.html

================================================================================
来源：http://hz.zhongyouzk.top/gtwusdjvzt.html

[U01] Py：创建虚拟环境
来源：http://hz.tianlin.xyz/gtlpsoiwcg.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.hammf.cn/gtkelsvdfd.html

[U02] Py：导出 / 安装依赖
来源：http://hz.sxryk.cn/gtzcdcotkv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jinghuilouyu.cn/gtlwfnutxv.html

[U03] Py：加载 .env 配置
来源：http://hz.dashuyun.cn/gtpkysdzse.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.xinyue.icu/gtxvebulkl.html

[U04] Py：变量调试打印
来源：http://hz.yj202588.top/gthcepkkek.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yueranfly.top/gtzntqyyfp.html

[U05] Py：列表去重且保序
来源：http://hz.tanke756.top/gtpxenisnf.html

list(dict.fromkeys(arr))
来源：http://hz.shzxlz.cn/gthcjeojbz.html

[U06] Py：合并两个字典
来源：http://hz.iojbl.cn/gtoxdidwyd.html

{**a, **b}
来源：http://hz.hongshengwenyu.top/gtuzjfshud.html

[U07] Py：反转字典键值
来源：http://hz.sxryk.cn/gttvppxwis.html

{v: k for k, v in d.items()}
来源：http://hz.zhiwuduotai.top/gtfgucfayh.html

[U08] Py：展平二维列表
来源：http://hz.smart0.xyz/gtrjqquzqy.html

[y for x in nested for y in x]
来源：http://hz.zhijiandao.cn/gtgafadbgs.html

[U09] Py：字典取最大值的键
来源：http://hz.yj202588.top/gtrtsknspg.html

max(d, key=d.get)
来源：http://hz.yongpay.top/gtnfvdyrnc.html

[U10] Py：按值排序字典
来源：http://hz.xingfuxueyuan.xyz/gtwlqgdgph.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.guowangkeji.top/gtgeqssyiy.html

[U11] Py：生成器表达式
来源：http://hz.cqqwz.cn/gtphdvqbzv.html

(x * 2 for x in arr)
来源：http://hz.wangdashe.top/gtspwnurid.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.aizwys.cn/gtaeqdzwqf.html

Counter(arr).most_common(3)
来源：http://hz.316326.xyz/gtlsbcxdcz.html

[U13] Py：固定长度队列
来源：http://hz.yj202588.top/gtecuzuxvl.html

deque(maxlen=10)
来源：http://hz.ybcxt.top/gtktxuttfl.html

[U14] Py：分组收集到列表
来源：http://hz.xingfuxueyuan.xyz/gttwfqvpxb.html

defaultdict(list)
来源：http://hz.ivvv.top/gtdktwrlkd.html

[U15] Py：高精度计时
来源：http://hz.xingfuxueyuan.xyz/gtaziwgmpx.html

t = time.perf_counter()
来源：http://hz.fzhhl.top/gtrlltgzrs.html

[U16] Py：命令行参数解析
来源：http://hz.fengsongda.top/gtsijmxmec.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.ehwqpu.com/gtmaxkeevx.html

[U17] Py：初始化日志
来源：http://hz.dianchejie.cn/gtpiskzvwk.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.316326.xyz/gtpmmobgjj.html

[U18] Py：预编译正则
来源：http://hz.fengsongda.top/gtfugxcilw.html

pat = re.compile(r"\d+")
来源：http://hz.meibo888.top/gtblabiacb.html

[U19] Py：正则替换带回调
来源：http://hz.sufxvd.cn/gtqodwhtpa.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.hnqzz.top/gtpewntsxm.html

[U20] Py：缓存函数结果
来源：http://hz.9152youxi.cn/gtyljbwums.html

@functools.lru_cache(maxsize=None)
来源：http://hz.shuidangran.top/gtfeyqdogc.html

[U21] Py：自定义上下文管理器
来源：http://hz.xuetiantiany.cn/gthsvlbbfh.html

@contextlib.contextmanager
来源：http://hz.yvedp.cn/gtksosornt.html

[U22] Py：矩阵转置
来源：http://hz.cdnleiting.top/gtxkivcfzt.html

list(zip(*m))
来源：http://hz.daria6918.cn/gtplorlbfm.html

[U23] Py：分块读取大文件
来源：http://hz.c1oappe.top/gtfxlldiia.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yuanzhike.top/gtlbjoppnx.html

[U24] Py：路径操作
来源：http://hz.tian-w.cn/gtuabzbmbz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.tanke756.top/gtvxzhnqaw.html

[U25] Py：CSV 按字典读
来源：http://hz.pycfn.com/gttgyjiyme.html

csv.DictReader(f)
来源：http://hz.yj202588.top/gtvxdfvxeq.html

[U26] Py：并发下载
来源：http://hz.xinyue.icu/gtgilnevzi.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.yueranfly.top/gtwjweoiit.html

[U27] Py：异步 HTTP
来源：http://hz.daria6918.cn/gtjjsgnjwh.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.yj20258888.top/gtjknpqsfr.html

[U28] Py：类型别名
来源：http://hz.jianghu66.top/gtmzchrpxa.html

UserId = int
来源：http://hz.jlsjyb.cn/gtlxelvkhx.html

[U29] Py：属性校验
来源：http://hz.pycfn.com/gtxtglhpnr.html

@property 与 @x.setter 配合
来源：http://hz.zhiwuduotai.top/gtkrezkdol.html

[U30] Py：数据类
来源：http://hz.jlsjyb.cn/gthbxhrwem.html

@dataclass(slots=True)
来源：http://hz.zdqjudy.top/gtshngqhze.html

[U31] Py：单测
来源：http://hz.haohaochexian.top/gtejhpuzul.html

python -m pytest -q
来源：http://hz.yj20258.top/gtjkflztge.html

[U32] Py：代码格式化
来源：http://hz.cucudq.cn/gtkwnsvwai.html

ruff format . && ruff check --fix .
来源：http://hz.chenjidiqi.icu/gtwrnmuixj.html


<!-- 参考信息 -->