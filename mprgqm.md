代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://hz.mhx1999.top/gtyghfnnhv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yj20258.top/gtzpmiltyo.html

fclose(f);
来源：http://hz.ybcxt.top/gtglhqejcm.html

[S12] C：写文件
来源：http://hz.zhijiandao.cn/gtxeakhqrg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.guannengcc.top/gtvbhqqzen.html

[S13] C：宏定义
来源：http://hz.tanke756.top/gtkmqwbwgc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.pengpengdd.cyou/gtkjabhxqc.html

[S14] C：枚举
来源：http://hz.zhengqikj.top/gtbbqfwzge.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhongyouzk.top/gtpiioynzx.html

[S15] C：类型转换
来源：http://hz.xuetiantiany.cn/gtmbfszphk.html

(double) a / b
来源：http://hz.haohaochexian.top/gtbjtziffu.html

[S16] C：位操作置位
来源：http://hz.mhx1999.top/gtocdycxrq.html

x |= (1 << 3);
来源：http://hz.jianghu66.top/gtktcjinkk.html

[S17] C：安全拼接字符串
来源：http://hz.vqdsnc.cn/gtusdurhxh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.gaohongyu789.top/gtyvoynhrf.html

[S18] C：命令行参数
来源：http://hz.xuetiantiany.cn/gtxovciiuo.html

int main(int argc, char **argv)
来源：http://hz.zhongyouzk.top/gtlnkqodss.html

[S19] C：快速排序
来源：http://hz.redwolf501.top/gtrzekeilz.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yangfankeji.com/gtekbqtnny.html

[S20] C：二分查找
来源：http://hz.snrcjt.cn/gtheimjnmq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yvedp.cn/gtsbqfpqlb.html

[S21] C：字符类别判断
来源：http://hz.jinyuanbaomall.cn/gtcebvxqii.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.birdmap.top/gtxbwoowrh.html

[S22] C：字符串转数字
来源：http://hz.ppjwa.cn/gtacdzcypt.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xingfuxueyuan.xyz/gtrklcsxxf.html

[S23] C：随机数
来源：http://hz.fzhhl.top/gtmaxrudae.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hammf.cn/gtbbufjkui.html

[S24] C：获取本地时间
来源：http://hz.hysaishi.cn/gtacsahzul.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hongshengwenyu.top/gtpnappyqr.html

[S25] C：内存拷贝
来源：http://hz.pycfn.com/gtyntqtgme.html

memcpy(dst, src, n);
来源：http://hz.birdmap.top/gtepzgaial.html

[S26] C：内存清零
来源：http://hz.zhoulong.xyz/gtyztyqgcl.html

memset(a, 0, sizeof a);
来源：http://hz.hnqzz.top/gtbbiynyxd.html

[S27] C：定义常量
来源：http://hz.52xcode.cn/gttlwldbto.html

const double PI = 3.14159;
来源：http://hz.jqgufenzy.top/gtobkrtmyn.html

[S28] C：静态变量
来源：http://hz.aibaodan.cn/gteqpwlcua.html

static int counter = 0;
来源：http://hz.ydjk.org.cn/gtzulwsuck.html

[S29] C：变参函数
来源：http://hz.ydjk.org.cn/gtnogfkuht.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jqgfzy.top/gtoyfnnrdm.html

[S30] C：头文件保护
来源：http://hz.birdmap.top/gtimotoxnk.html

#ifndef X_H
来源：http://hz.bjfxy.top/gtmamjjgrk.html

#define X_H
来源：http://hz.jinqigufen.top/gtlrttikdc.html

#endif
来源：http://hz.zhongyouzk.top/gttmbsxkje.html

[S31] C++：Hello World
来源：http://hz.xylfe.cn/gtnicjuzdg.html

#include <iostream>
来源：http://hz.svipenyu.cn/gtzdrqyorm.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jqgfzy.top/gtkfguegvc.html

[S32] C++：字符串
来源：http://hz.yangfankeji.com/gtzracsbdv.html

std::string s = "hi";  s += "!";
来源：http://hz.bjfxy.top/gtkdbykbab.html

[S33] C++：vector 增删
来源：http://hz.0kj1m.cn/gtnslrqvgv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yangfankeji.com/gtyamgjmjj.html

[S34] C++：遍历 vector
来源：http://hz.shanyushiyangkeji.top/gtgosrlsxr.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jianghu66.top/gttlnmqaom.html

[S35] C++：map
来源：http://hz.shanyushiyangkeji.top/gttbovcymr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhiwuduotai.top/gtbijtamji.html

[S36] C++：unordered_map
来源：http://hz.0kj1m.cn/gtvddtfuby.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jqgufenzy.top/gtfhvxmlwo.html

[S37] C++：set
来源：http://hz.shangyingyoupin.top/gtypgckiae.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhiwuduotai.top/gtfswvfldn.html

[S38] C++：排序
来源：http://hz.jianghu66.top/gtbjdajomm.html

std::sort(v.begin(), v.end());
来源：http://hz.xziqi.cn/gtraxpsnfl.html

[S39] C++：自定义比较器排序
来源：http://hz.ydzc1.top/gtkqdugpgp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zycfv.cn/gtgcgjwayj.html

[S40] C++：查找元素
来源：http://hz.hfpthk.cn/gtbgpmbjfu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.9152youxi.cn/gtwfatdimf.html

[S41] C++：类与构造函数
来源：http://hz.dianchejie.cn/gtuuxohgdi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.pengpengdd.cyou/gtokciwhpt.html

[S42] C++：继承与虚函数
来源：http://hz.tanke756.top/gtyzywnzie.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhoulong.xyz/gtirawrwyu.html

[S43] C++：智能指针
来源：http://hz.sxryk.cn/gtgeirueug.html

auto p = std::make_unique<int>(5);
来源：http://hz.52xcode.cn/gtmzfmodtu.html

[S44] C++：引用传参
来源：http://hz.ybcxt.top/gtiwagfvan.html

void inc(int &x) { ++x; }
来源：http://hz.ywan-chungtsiang.top/gtgdqthyub.html

[S45] C++：lambda
来源：http://hz.gogol.net.cn/gtzqjvyokm.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hnqzz.top/gttjridlxw.html

[S46] C++：函数模板
来源：http://hz.redwolf501.top/gtvcscdpzg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yonumen.top/gthncinabq.html

[S47] C++：结构化绑定遍历
来源：http://hz.ybcxt.top/gtqkilwnev.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.sysykeji.top/gtkqihajej.html

[S48] C++：逐行读文件
来源：http://hz.xuanzx.com/gtfsxgkgao.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yonumen.top/gtpfapqejy.html

while (std::getline(in, line)) { }
来源：http://hz.zhiwuduotai.top/gtvgzgktnj.html

[S49] C++：写文件
来源：http://hz.hnqzz.top/gtinycyuos.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yj202588.top/gtidihpxgz.html

[S50] C++：格式化数字
来源：http://hz.nanxuanxn.top/gtbzzntypm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.tanke756.top/gtyrrlrgzv.html

[S51] C++：显式类型转换
来源：http://hz.yj20258888.top/gtkyevcblk.html

static_cast<double>(a) / b
来源：http://hz.yuxming.cn/gtsdvvedzl.html

[S52] C++：const 与 noexcept
来源：http://hz.yueranfly.top/gtdncsfcdg.html

int size() const noexcept { return n_; }
来源：http://hz.0kj1m.cn/gtirqjjvuw.html

[S53] C++：移动语义
来源：http://hz.jinyuanbaomall.cn/gtuwhewbcb.html

std::vector<int> w = std::move(v);
来源：http://hz.jinqigufen.top/gtcchbjqhi.html

[S54] C++：异常处理
来源：http://hz.tian-w.cn/gtayrmryws.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.xziqi.cn/gtrrwbzord.html

[S55] C++：结构化绑定
来源：http://hz.chenzaomai.com/gtjtlntifl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yj202588.top/gtuedupwxj.html

[S56] C++：optional
来源：http://hz.yj20258888.top/gtdqlftnws.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.wangshuangyany.cn/gtcgpnoswk.html

[S57] C++：编译期常量
来源：http://hz.ywan-chungtsiang.top/gtkgzzvxxl.html

constexpr int N = 10;
来源：http://hz.andypj.xyz/gtnxposvzt.html

[S58] C++：命名空间
来源：http://hz.hfpthk.cn/gtsihgaftg.html

namespace ns { int f() { return 1; } }
来源：http://hz.aizwys.cn/gtekfihqld.html

[S59] C++：静态断言
来源：http://hz.ydzc1.top/gtjpgunmvf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.guannengcc.top/gtjcksuclr.html

[S60] C++：遍历并删除元素
来源：http://hz.yj20258.top/gtdqgfyiow.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.shanyushiyangtech.top/gtjytnquni.html

================================================================================
来源：http://hz.ppjwa.cn/gtnsmqyevl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ydjk.org.cn/gtarwtqzrp.html

================================================================================
来源：http://hz.quarkkingdee.top/gtlueybzix.html

[T01] Kotlin：Hello World
来源：http://hz.shzxlz.cn/gtrrdrrjsn.html

println("Hello")
来源：http://hz.jqgufenzy.top/gtzpretfyx.html

[T02] Kotlin：变量
来源：http://hz.yj202588.top/gtkuscuszk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jiagoushi.top/gtqckuuacz.html

[T03] Kotlin：字符串模板
来源：http://hz.yj20258888.top/gttfllrwks.html

"值: $b"
来源：http://hz.fengsongda.top/gtwbxgdyty.html

[T04] Kotlin：空安全
来源：http://hz.dianchejie.cn/gtybcrtexd.html

val n: String? = null;  n?.length
来源：http://hz.sxryk.cn/gtabgdxgzc.html

[T05] Kotlin：when 表达式
来源：http://hz.sxryk.cn/gtucuuhvfg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.gaohongyu789.top/gtlxjisgmd.html

[T06] Kotlin：集合映射
来源：http://hz.hywenlv.cn/gtobpcdggk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.9152youxi.cn/gtvkeenffw.html

[T07] Kotlin：集合过滤
来源：http://hz.hammf.cn/gtwnzlkqzh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.pycfn.com/gtxqpieovy.html

[T08] Kotlin：数据类
来源：http://hz.xuanzx.com/gtadlqwkoc.html

data class User(val name: String, val age: Int)
来源：http://hz.hywenlv.cn/gtubsrkzws.html

[T09] Kotlin：扩展函数
来源：http://hz.sufxvd.cn/gtrubzqiiy.html

fun String.exclaim() = this + "!"
来源：http://hz.nanxuanxn.top/gtmsohtdxc.html

[T10] Kotlin：默认参数
来源：http://hz.bjfxy.top/gtpalkuhzz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.chenjidiqi.icu/gtqdutnjbr.html

[T11] Kotlin：协程
来源：http://hz.dianchejie.cn/gtwfgqsyeg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.guannengcc.top/gttvrhpscp.html

[T12] Kotlin：解构声明
来源：http://hz.snrcjt.cn/gtzqxazflw.html

val (a, b) = Pair(1, 2)
来源：http://hz.jyoumei.cn/gtjsgfhduz.html

[T13] Kotlin：只读 Map
来源：http://hz.chenzaomai.com/gtuqggieih.html

val m = mapOf("a" to 1)
来源：http://hz.hnqzz.top/gtxzrzofxn.html

[T14] Kotlin：循环
来源：http://hz.iojbl.cn/gttvuxdskh.html

for (i in 1..10) println(i)
来源：http://hz.zhiwuduotai.top/gtyfdqcthp.html

[T15] Kotlin：接口
来源：http://hz.316326.xyz/gtuvwgprkg.html

interface Shape { fun area(): Double }
来源：http://hz.xuetiantiany.cn/gtxsdedvls.html

[T16] Swift：Hello World
来源：http://hz.shuidangran.top/gtvowrwxbu.html

print("Hello")
来源：http://hz.yueranfly.top/gtcankqihi.html

[T17] Swift：变量与常量
来源：http://hz.ydjk.org.cn/gthnnmeajn.html

var a = 1;  let b = 2
来源：http://hz.iojbl.cn/gtwbuqatxu.html

[T18] Swift：字符串插值
来源：http://hz.zhengqikj.top/gtnnbkdjru.html

"值: \(b)"
来源：http://hz.sysykeji.top/gthdjpirka.html

[T19] Swift：可选绑定
来源：http://hz.dianchejie.cn/gtaubwocpg.html

if let n = opt { print(n) }
来源：http://hz.havefunace.top/gtejttjmun.html

[T20] Swift：数组操作
来源：http://hz.jqgfzy.top/gteirgakze.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.hywenlv.cn/gtziehxxli.html

[T21] Swift：遍历
来源：http://hz.hongshengwenyu.top/gtjouqmute.html

for x in a { print(x) }
来源：http://hz.nanxuanxn.top/gtwhqtibzx.html

[T22] Swift：字典
来源：http://hz.jinqigufen.top/gtnsihlxjh.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.pycfn.com/gtlesnoesg.html

[T23] Swift：函数
来源：http://hz.pycfn.com/gtsgsukwah.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.shangyingyoupin.top/gtpzixhise.html

[T24] Swift：闭包
来源：http://hz.shzxlz.cn/gtjidzzbpy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.shangyingyoupin.top/gtolztltpv.html

[T25] Swift：结构体
来源：http://hz.ybcxt.top/gtjjeujuxx.html

struct P { var x: Int }
来源：http://hz.yongpay.top/gtxvlblrnc.html

[T26] Swift：类与重写
来源：http://hz.jianghu66.top/gtokylkhdt.html

class A: Base { override func f() {} }
来源：http://hz.cucudq.cn/gtpnymnynx.html

[T27] Swift：错误处理
来源：http://hz.yj20258.top/gtiytrxzdb.html

do { try f() } catch { print(error) }
来源：http://hz.cashguo.top/gtioillevi.html

[T28] Swift：枚举
来源：http://hz.chenzaomai.com/gtovaketqy.html

enum Color { case red, green }
来源：http://hz.shangyingyoupin.top/gtfsbbepzw.html

[T29] Swift：guard 提前返回
来源：http://hz.yj202588.top/gtyjrflbol.html

guard let x = opt else { return }
来源：http://hz.xziqi.cn/gtubapgzto.html

[T30] Swift：协议
来源：http://hz.sweek.top/gtakjlsosf.html

protocol Shape { func area() -> Double }
来源：http://hz.zhaomingkeji.xyz/gtfobyfxwo.html

[T31] Lua：Hello World
来源：http://hz.zhaomingkeji.xyz/gtxajiasjl.html

print("Hello")
来源：http://hz.iojbl.cn/gttdmgyxjd.html

[T32] Lua：局部变量
来源：http://hz.ywan-chungtsiang.top/gtbmpbqnbr.html

local a = 1
来源：http://hz.nanxuanxn.top/gtxdusrzls.html

[T33] Lua：表（数组）
来源：http://hz.iojbl.cn/gtejbjfijl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.52xcode.cn/gtyejhohvh.html

[T34] Lua：遍历表
来源：http://hz.fzhhl.top/gtrqzewgmb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.shanyushiyangtech.top/gtjzkemheb.html

[T35] Lua：字典表
来源：http://hz.cqqwz.cn/gtjzadggxv.html

local d = { a = 1 };  d.b = 2
来源：http://hz.birdmap.top/gtdhszoqnm.html

[T36] Lua：函数
来源：http://hz.yongpay.top/gtxlrbglrt.html

function add(a, b) return a + b end
来源：http://hz.shangyingyoupin.top/gtppdemfya.html

[T37] Lua：字符串拼接
来源：http://hz.jlsjyb.cn/gtiyvbxcjr.html

"a" .. "b"
来源：http://hz.mhx1999.top/gtruqxovaa.html

[T38] Lua：条件
来源：http://hz.0kj1m.cn/gtrafwqauq.html

if x > 0 then print("正") end
来源：http://hz.9152youxi.cn/gtxraroogp.html

[T39] Lua：模式匹配
来源：http://hz.bjfxy.top/gtqcssqxxt.html

string.find(s, "%d+")
来源：http://hz.yj202588.top/gtvgahakwi.html

[T40] Lua：元表
来源：http://hz.yvedp.cn/gtorymirwd.html

setmetatable({}, { __index = base })
来源：http://hz.wangshuangyany.cn/gtriaumeim.html

[T41] Perl：Hello World
来源：http://hz.dianchejie.cn/gtbdvzgjeu.html

print "Hello\n";
来源：http://hz.zdqjudy.top/gtncsxbvcg.html

[T42] Perl：变量类型
来源：http://hz.jqgfzy.top/gtytfpkqew.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.ybcxt.top/gtyhwbmmcb.html

[T43] Perl：字符串插值
来源：http://hz.gogol.net.cn/gtyvajrxri.html

"值: $a"
来源：http://hz.guowangkeji.top/gtcdkxaepn.html

[T44] Perl：条件
来源：http://hz.ybcxt.top/gtvxdaggfc.html

if ($a > 0) { print "正"; }
来源：http://hz.xinyue.icu/gtiirkache.html

[T45] Perl：数组遍历
来源：http://hz.gogol.net.cn/gtnvnkysdg.html

for my $x (@arr) { print $x; }
来源：http://hz.gzhubu.top/gtmwaxfpeu.html

[T46] Perl：哈希操作
来源：http://hz.andypj.xyz/gthwfeccjl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.shangyingyoupin.top/gtkomlssvx.html

[T47] Perl：正则捕获
来源：http://hz.birdmap.top/gttzsexrew.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jqgufenzy.top/gtqdhrpsal.html

[T48] Perl：正则替换
来源：http://hz.xingfuxueyuan.xyz/gtffbytlzk.html

$s =~ s/old/new/g;
来源：http://hz.hongshengwenyu.top/gtnctkvykb.html

[T49] Perl：函数
来源：http://hz.zycfv.cn/gtpuqbeftf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.sufxvd.cn/gtvhfxfeht.html

[T50] Perl：逐行读文件
来源：http://hz.chenjidiqi.icu/gtjvnxevyn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.iojbl.cn/gtisotdlqg.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.feifeiyinyue.top/gtsuexotup.html

[T51] Scala：Hello World
来源：http://hz.cqqwz.cn/gthpybmkja.html

println("Hello")
来源：http://hz.jlsjyb.cn/gtxnknrftq.html

[T52] Scala：变量
来源：http://hz.xuanzx.com/gtuiwjdugm.html

val a = 1;  var b = 2
来源：http://hz.c1oappe.top/gtbqukcjjq.html

[T53] Scala：字符串插值
来源：http://hz.xziqi.cn/gtnxoqautn.html

s"值: $b"
来源：http://hz.gotoacloud.top/gttmtfjaef.html

[T54] Scala：集合映射
来源：http://hz.tianlin.xyz/gtevzjzyxx.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.redwolf501.top/gtsnzmwvur.html

[T55] Scala：集合过滤
来源：http://hz.wangshuangyany.cn/gtpreoyzfq.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.sweek.top/gtsonbmvew.html

[T56] Scala：样例类
来源：http://hz.vqdsnc.cn/gttkxgfcev.html

case class User(name: String, age: Int)
来源：http://hz.cucudq.cn/gtiiipclve.html

[T57] Scala：模式匹配
来源：http://hz.jianghu66.top/gtoefktlqh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.xuanzx.com/gtpiltlyvz.html

[T58] Scala：函数定义
来源：http://hz.gogol.net.cn/gtkhlabrfe.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jqgfzy.top/gtdfjsvycs.html

[T59] Scala：循环
来源：http://hz.hongshengwenyu.top/gtipigdrdn.html

for (i <- 1 to 10) println(i)
来源：http://hz.meibo888.top/gtsyhshwgb.html

[T60] Scala：折叠
来源：http://hz.fengsongda.top/gtlfeioqqi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.gaohongyu789.top/gtatkfmegk.html

================================================================================
来源：http://hz.aibaodan.cn/gtnrzioxaz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.nanxuanxn.top/gtuoreopdr.html

================================================================================
来源：http://hz.zhoulong.xyz/gtinromgok.html

[U01] Py：创建虚拟环境
来源：http://hz.zhaomingkeji.xyz/gtrikibmsa.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.feifeiyinyue.top/gttfhehnqy.html

[U02] Py：导出 / 安装依赖
来源：http://hz.pengpengdd.cyou/gtsdqinvoo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.guowangkeji.top/gtifnewkpi.html

[U03] Py：加载 .env 配置
来源：http://hz.hnxiangtu.top/gtviycxdec.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.shanyushiyangtech.top/gtakmiesch.html

[U04] Py：变量调试打印
来源：http://hz.zhaomingkeji.xyz/gtlihafhhf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yj20258.top/gtspgbmhac.html

[U05] Py：列表去重且保序
来源：http://hz.pengpengdd.cyou/gtzhmcdfai.html

list(dict.fromkeys(arr))
来源：http://hz.chenzaomai.com/gtgtwcwhpy.html

[U06] Py：合并两个字典
来源：http://hz.cqqwz.cn/gtzwsyyupx.html

{**a, **b}
来源：http://hz.daxiang520.top/gtezqymnoe.html

[U07] Py：反转字典键值
来源：http://hz.meibo888.top/gtcnrlalhm.html

{v: k for k, v in d.items()}
来源：http://hz.zdqjudy.top/gtceqnejby.html

[U08] Py：展平二维列表
来源：http://hz.dashuyun.cn/gtobtloeki.html

[y for x in nested for y in x]
来源：http://hz.yuxming.cn/gthgemywkj.html

[U09] Py：字典取最大值的键
来源：http://hz.zhiwuduotai.top/gtyovmwatx.html

max(d, key=d.get)
来源：http://hz.hongshengwenyu.top/gtfampdsdn.html

[U10] Py：按值排序字典
来源：http://hz.iojbl.cn/gtymglkrht.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.cheryme.top/gtalwcygtg.html

[U11] Py：生成器表达式
来源：http://hz.shanyushiyangtech.top/gtxzqbmmmb.html

(x * 2 for x in arr)
来源：http://hz.xingfuxueyuan.xyz/gtjuronsaa.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.quarkkingdee.top/gtkyfzxhxm.html

Counter(arr).most_common(3)
来源：http://hz.cdnleiting.top/gtpmcsgbvt.html

[U13] Py：固定长度队列
来源：http://hz.c1oappe.top/gtmzbypcxi.html

deque(maxlen=10)
来源：http://hz.xinyue.icu/gtpsssnmto.html

[U14] Py：分组收集到列表
来源：http://hz.c1oappe.top/gtebpivbsz.html

defaultdict(list)
来源：http://hz.fengsongda.top/gtwngpqqky.html

[U15] Py：高精度计时
来源：http://hz.gotoacloud.top/gthxdfilec.html

t = time.perf_counter()
来源：http://hz.yanxiufei.cn/gtsloojpdu.html

[U16] Py：命令行参数解析
来源：http://hz.guannengcc.top/gtxcjfbkjb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yj202588.top/gtdejnhqpb.html

[U17] Py：初始化日志
来源：http://hz.wangshuangyany.cn/gtnvbwzoek.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.gaohongyu789.top/gtwjydbeie.html

[U18] Py：预编译正则
来源：http://hz.xuetiantiany.cn/gtxvbcmufa.html

pat = re.compile(r"\d+")
来源：http://hz.dashuyun.cn/gtpcimtblu.html

[U19] Py：正则替换带回调
来源：http://hz.52xcode.cn/gthnbwfuqd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.nanxuanxn.top/gtfvfhymxl.html

[U20] Py：缓存函数结果
来源：http://hz.haohaochexian.top/gtsccanifl.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zhoulong.xyz/gtdxmyrrmf.html

[U21] Py：自定义上下文管理器
来源：http://hz.cashguo.top/gtsjwesojd.html

@contextlib.contextmanager
来源：http://hz.nwbrower.top/gtgjevgmfv.html

[U22] Py：矩阵转置
来源：http://hz.c1oappe.top/gtycxaedfm.html

list(zip(*m))
来源：http://hz.smart0.xyz/gtocuxcohl.html

[U23] Py：分块读取大文件
来源：http://hz.aizwys.cn/gtokjztqhl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.aibaodan.cn/gttzavipbl.html

[U24] Py：路径操作
来源：http://hz.vqdsnc.cn/gtpbrldijj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.hnqzz.top/gtslfxzxtg.html

[U25] Py：CSV 按字典读
来源：http://hz.sxryk.cn/gtvjwqvchx.html

csv.DictReader(f)
来源：http://hz.snrcjt.cn/gtktxckngo.html

[U26] Py：并发下载
来源：http://hz.yanxiufei.cn/gtwircjdyt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.xziqi.cn/gtcxqwjcqt.html

[U27] Py：异步 HTTP
来源：http://hz.iojbl.cn/gtfapzscpj.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.ydzc1.top/gtxunlhpmc.html

[U28] Py：类型别名
来源：http://hz.guowangkeji.top/gtdcszylms.html

UserId = int
来源：http://hz.ywan-chungtsiang.top/gtcodxiotr.html

[U29] Py：属性校验
来源：http://hz.yanxiufei.cn/gtbahvgvrx.html

@property 与 @x.setter 配合
来源：http://hz.vqdsnc.cn/gtyxkgieuo.html

[U30] Py：数据类
来源：http://hz.yanxiufei.cn/gtifopqlbr.html

@dataclass(slots=True)
来源：http://hz.nanxinkj.top/gtqtualddy.html

[U31] Py：单测
来源：http://hz.yuanzhike.top/gtzekqddhs.html

python -m pytest -q
来源：http://hz.iojbl.cn/gttnmepjdq.html

[U32] Py：代码格式化
来源：http://hz.yangfankeji.com/gtrbdwguwm.html

ruff format . && ruff check --fix .
来源：http://hz.zhixingplan.top/gtzrakbqps.html

[U33] Py：打包发布
来源：http://hz.0kj1m.cn/gtatyxcwyo.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.gotoacloud.top/gtkpjcsamv.html

[U34] Py：判断编码
来源：http://hz.nanxinkj.top/gtzdowlyjt.html

chardet.detect(raw)
来源：http://hz.chenlongwang.top/gtabdekjjl.html


<!-- 参考信息 -->