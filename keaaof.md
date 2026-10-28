代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jianghu66.top/gtcifjuhty.html

[S08] C：动态内存分配与释放
来源：http://hz.gogol.net.cn/gtijbvvpke.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.gzhubu.top/gtgszcodyc.html

[S09] C：结构体定义与初始化
来源：http://hz.zdqjudy.top/gtqdkiauty.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jinqigfzy.top/gtvvhfagpv.html

[S10] C：指针与解引用
来源：http://hz.iojbl.cn/gtkijjaspp.html

int *p = &a;  *p = 5;
来源：http://hz.cqqwz.cn/gthacpwwoi.html

[S11] C：逐行读文件
来源：http://hz.smart0.xyz/gtanfqnoyp.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yvedp.cn/gtbznfrtst.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ydjk.org.cn/gtxwnhxsdv.html

fclose(f);
来源：http://hz.ydzc1.top/gtphvrcvky.html

[S12] C：写文件
来源：http://hz.pengpengdd.cyou/gteeqwcqnq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.cashguo.top/gtzxdaetpt.html

[S13] C：宏定义
来源：http://hz.bjfxy.top/gtbdikbiyb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.chenzaomai.com/gtpewvkuoi.html

[S14] C：枚举
来源：http://hz.shzxlz.cn/gtoiivkxro.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xingfuxueyuan.xyz/gtkpnnvgug.html

[S15] C：类型转换
来源：http://hz.guannengcc.top/gtwuwavand.html

(double) a / b
来源：http://hz.ivvv.top/gtmnmyhywu.html

[S16] C：位操作置位
来源：http://hz.hfpthk.cn/gteqrvwslk.html

x |= (1 << 3);
来源：http://hz.meibo888.top/gtrvmprkca.html

[S17] C：安全拼接字符串
来源：http://hz.zhijiandao.cn/gtmptnalzl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.svipenyu.cn/gtvaeldtav.html

[S18] C：命令行参数
来源：http://hz.yanxiufei.cn/gtidzvfpxo.html

int main(int argc, char **argv)
来源：http://hz.xuetiantiany.cn/gtyiruomwj.html

[S19] C：快速排序
来源：http://hz.cqqwz.cn/gtvmfsnbrr.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zycfv.cn/gttwcxisbt.html

[S20] C：二分查找
来源：http://hz.pengpengdd.cyou/gtvvhpyyos.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.quarkkingdee.top/gtvrbpmsnn.html

[S21] C：字符类别判断
来源：http://hz.ehwqpu.com/gtyxrizcdj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.cqqwz.cn/gtdfmcoufg.html

[S22] C：字符串转数字
来源：http://hz.cdnleiting.top/gtwikqjczn.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.shanyushiyangkeji.top/gticbmyyzy.html

[S23] C：随机数
来源：http://hz.kuanghao11.cn/gttqkjhrvv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yonumen.top/gtdybcdknb.html

[S24] C：获取本地时间
来源：http://hz.svipenyu.cn/gtavvozhet.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.daxiang520.top/gtxnyyeruk.html

[S25] C：内存拷贝
来源：http://hz.tianlin.xyz/gtaktxudhu.html

memcpy(dst, src, n);
来源：http://hz.0kj1m.cn/gtnbgwidvs.html

[S26] C：内存清零
来源：http://hz.xingfuxueyuan.xyz/gtbbruqjnn.html

memset(a, 0, sizeof a);
来源：http://hz.jqgufenzy.top/gtzxplhnkw.html

[S27] C：定义常量
来源：http://hz.sysykeji.top/gtftpavzsm.html

const double PI = 3.14159;
来源：http://hz.redwolf501.top/gtdbqsjpoo.html

[S28] C：静态变量
来源：http://hz.shanyushiyangkeji.top/gtmklotogz.html

static int counter = 0;
来源：http://hz.xuanzx.com/gtucimnjiz.html

[S29] C：变参函数
来源：http://hz.chenjidiqi.icu/gthudyyfyz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhaomingkeji.xyz/gtgbsjcguu.html

[S30] C：头文件保护
来源：http://hz.xziqi.cn/gtqzswopwh.html

#ifndef X_H
来源：http://hz.zdqjudy.top/gtmooofcwv.html

#define X_H
来源：http://hz.ybcxt.top/gtppwvrmej.html

#endif
来源：http://hz.ivvv.top/gthhcdmmhv.html

[S31] C++：Hello World
来源：http://hz.shzxlz.cn/gtjalmrlbi.html

#include <iostream>
来源：http://hz.yangfankeji.com/gtzzgqpyls.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hammf.cn/gtiunqxtnr.html

[S32] C++：字符串
来源：http://hz.wangdashe.top/gtqkzilkaf.html

std::string s = "hi";  s += "!";
来源：http://hz.shanyushiyangtech.top/gthhuddqoe.html

[S33] C++：vector 增删
来源：http://hz.smart0.xyz/gtnajgkkep.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.c1oappe.top/gtbmlqnlou.html

[S34] C++：遍历 vector
来源：http://hz.mhx1999.top/gtwjfggiim.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.svipenyu.cn/gtxvmucqdk.html

[S35] C++：map
来源：http://hz.9152youxi.cn/gtqsxfyxhk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xuanzx.com/gtjszzhxvp.html

[S36] C++：unordered_map
来源：http://hz.shangyingyoupin.top/gthcvyckrk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhixingplan.top/gtkrhtljtc.html

[S37] C++：set
来源：http://hz.gogol.net.cn/gtqsfzxuey.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.chenlongwang.top/gtxwotqjnh.html

[S38] C++：排序
来源：http://hz.wangshuangyany.cn/gtrzpggmbb.html

std::sort(v.begin(), v.end());
来源：http://hz.shanyushiyangtech.top/gtdriybcdy.html

[S39] C++：自定义比较器排序
来源：http://hz.pengpengdd.cyou/gtxbyjzmof.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.cqqwz.cn/gtijinlhrq.html

[S40] C++：查找元素
来源：http://hz.haohaochexian.top/gtauwgvtyi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yuanzhike.top/gtaivevwyb.html

[S41] C++：类与构造函数
来源：http://hz.redwolf501.top/gtgxrwaaka.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ivvv.top/gtyggxdgxk.html

[S42] C++：继承与虚函数
来源：http://hz.hysaishi.cn/gtojxgmsmi.html

class B : public Base { public: void f() override {} };
来源：http://hz.nanxuanxn.top/gtvfcgjuqr.html

[S43] C++：智能指针
来源：http://hz.shangyingyoupin.top/gtzoyxdeoj.html

auto p = std::make_unique<int>(5);
来源：http://hz.mhx1999.top/gtqnhvgrdm.html

[S44] C++：引用传参
来源：http://hz.jiagoushi.top/gtulgoigeg.html

void inc(int &x) { ++x; }
来源：http://hz.hywenlv.cn/gtmzlwkudi.html

[S45] C++：lambda
来源：http://hz.daxiang520.top/gtatfjuszy.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhiwuduotai.top/gtctljugle.html

[S46] C++：函数模板
来源：http://hz.9152youxi.cn/gtrsneqcyj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.haohaochexian.top/gtimpgsahe.html

[S47] C++：结构化绑定遍历
来源：http://hz.ehwqpu.com/gtonlkswfx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.havefunace.top/gtjnubxgjq.html

[S48] C++：逐行读文件
来源：http://hz.9152youxi.cn/gtsdhexgpl.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yueranfly.top/gthlwuepzd.html

while (std::getline(in, line)) { }
来源：http://hz.zhaomingkeji.xyz/gtluanamdz.html

[S49] C++：写文件
来源：http://hz.xylfe.cn/gtwtlorpqy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.xinyue.icu/gtyepayyov.html

[S50] C++：格式化数字
来源：http://hz.hammf.cn/gtjgvbtxme.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.316326.xyz/gtanzhmhyv.html

[S51] C++：显式类型转换
来源：http://hz.aizwys.cn/gtbutdwqac.html

static_cast<double>(a) / b
来源：http://hz.tanke756.top/gtckpjtclk.html

[S52] C++：const 与 noexcept
来源：http://hz.sysykeji.top/gtpcpqiwym.html

int size() const noexcept { return n_; }
来源：http://hz.tanke756.top/gtqzkyqlvp.html

[S53] C++：移动语义
来源：http://hz.ppjwa.cn/gthuszcfaw.html

std::vector<int> w = std::move(v);
来源：http://hz.haohaochexian.top/gtpaapqowj.html

[S54] C++：异常处理
来源：http://hz.vqdsnc.cn/gtkkqstwia.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.pengpengdd.cyou/gtgrwpnyuc.html

[S55] C++：结构化绑定
来源：http://hz.cucudq.cn/gtpccenonv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhongyouzk.top/gtdazurgkr.html

[S56] C++：optional
来源：http://hz.havefunace.top/gtqiluqqyd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yj20258888.top/gtjygqwsox.html

[S57] C++：编译期常量
来源：http://hz.0kj1m.cn/gtthjitxnt.html

constexpr int N = 10;
来源：http://hz.9152youxi.cn/gtbkumstpl.html

[S58] C++：命名空间
来源：http://hz.pengpengdd.cyou/gtmtxvdizd.html

namespace ns { int f() { return 1; } }
来源：http://hz.haohaochexian.top/gtwzbqzrop.html

[S59] C++：静态断言
来源：http://hz.sxryk.cn/gtgocogyuc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.tianlin.xyz/gtovrnnyra.html

[S60] C++：遍历并删除元素
来源：http://hz.yvedp.cn/gtamvegcxw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhixingplan.top/gtbygokkdg.html

================================================================================
来源：http://hz.shzxlz.cn/gtmpnsockv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.316326.xyz/gtutyxjiqc.html

================================================================================
来源：http://hz.daxiang520.top/gtoglphsal.html

[T01] Kotlin：Hello World
来源：http://hz.ehwqpu.com/gtyreqjjdl.html

println("Hello")
来源：http://hz.nanxinkj.top/gtrpyhhgom.html

[T02] Kotlin：变量
来源：http://hz.jqgufenzy.top/gtesmbmqxc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xuetiantiany.cn/gtgleelwuk.html

[T03] Kotlin：字符串模板
来源：http://hz.shangyingyoupin.top/gtzymnffze.html

"值: $b"
来源：http://hz.guowangkeji.top/gtmgmpsnid.html

[T04] Kotlin：空安全
来源：http://hz.sufxvd.cn/gtedkczufj.html

val n: String? = null;  n?.length
来源：http://hz.zycfv.cn/gtsftbcoro.html

[T05] Kotlin：when 表达式
来源：http://hz.yuxming.cn/gtjtuncdjj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jinghuilouyu.cn/gtpjsjsqws.html

[T06] Kotlin：集合映射
来源：http://hz.yonumen.top/gtuopnmyya.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.ydjk.org.cn/gtskjwqgfn.html

[T07] Kotlin：集合过滤
来源：http://hz.nwbrower.top/gthumvghpz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.chenjidiqi.icu/gtwfivpqno.html

[T08] Kotlin：数据类
来源：http://hz.hfpthk.cn/gtprrxbklc.html

data class User(val name: String, val age: Int)
来源：http://hz.yj20258888.top/gtsehyrgjk.html

[T09] Kotlin：扩展函数
来源：http://hz.havefunace.top/gtquarupoa.html

fun String.exclaim() = this + "!"
来源：http://hz.dianchejie.cn/gtcvztsteq.html

[T10] Kotlin：默认参数
来源：http://hz.9152youxi.cn/gtbjngsrsx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.birdmap.top/gtiearngif.html

[T11] Kotlin：协程
来源：http://hz.cdnleiting.top/gtlgqibkqm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zycfv.cn/gtxvyubbqb.html

[T12] Kotlin：解构声明
来源：http://hz.ivvv.top/gtaxtikgjc.html

val (a, b) = Pair(1, 2)
来源：http://hz.xingfuxueyuan.xyz/gtgbdrzurl.html

[T13] Kotlin：只读 Map
来源：http://hz.cqqwz.cn/gtlurpxvjm.html

val m = mapOf("a" to 1)
来源：http://hz.tian-w.cn/gtdtwccocf.html

[T14] Kotlin：循环
来源：http://hz.pycfn.com/gtppwgavjm.html

for (i in 1..10) println(i)
来源：http://hz.iojbl.cn/gtgqbzrfku.html

[T15] Kotlin：接口
来源：http://hz.jinyuanbaomall.cn/gtpmnebfmj.html

interface Shape { fun area(): Double }
来源：http://hz.chenzaomai.com/gtstuwvgaj.html

[T16] Swift：Hello World
来源：http://hz.wangshuangyany.cn/gtibmfkzca.html

print("Hello")
来源：http://hz.jqgfzy.top/gttxszmsti.html

[T17] Swift：变量与常量
来源：http://hz.fzhhl.top/gtyeqqyzif.html

var a = 1;  let b = 2
来源：http://hz.cdnleiting.top/gteqkgoupj.html

[T18] Swift：字符串插值
来源：http://hz.daria6918.cn/gtavttiypq.html

"值: \(b)"
来源：http://hz.zdqjudy.top/gteweyegqv.html

[T19] Swift：可选绑定
来源：http://hz.fzhhl.top/gtizcdvwmq.html

if let n = opt { print(n) }
来源：http://hz.yuanzhike.top/gtkusoqfib.html

[T20] Swift：数组操作
来源：http://hz.chenzaomai.com/gtayllbbkg.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.shzxlz.cn/gtwlcgtfdx.html

[T21] Swift：遍历
来源：http://hz.ydjk.org.cn/gthhjxwrkt.html

for x in a { print(x) }
来源：http://hz.hysaishi.cn/gtvbtnckxu.html

[T22] Swift：字典
来源：http://hz.andypj.xyz/gtncmcecga.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.daria6918.cn/gtskdeatbm.html

[T23] Swift：函数
来源：http://hz.vqdsnc.cn/gtwyobgbtm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jlsjyb.cn/gtilojncrp.html

[T24] Swift：闭包
来源：http://hz.hysaishi.cn/gtuthdfmdx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.fengsongda.top/gtfnlckagj.html

[T25] Swift：结构体
来源：http://hz.andypj.xyz/gtqawaxssq.html

struct P { var x: Int }
来源：http://hz.wangdashe.top/gtfnooziom.html

[T26] Swift：类与重写
来源：http://hz.sufxvd.cn/gtbjuhcxqf.html

class A: Base { override func f() {} }
来源：http://hz.gotoacloud.top/gtrzfuagjg.html

[T27] Swift：错误处理
来源：http://hz.xylfe.cn/gtlowvcvso.html

do { try f() } catch { print(error) }
来源：http://hz.ydzc1.top/gtgydkktxy.html

[T28] Swift：枚举
来源：http://hz.jqgfzy.top/gtafkkggyi.html

enum Color { case red, green }
来源：http://hz.yangfankeji.com/gthnbnwtxp.html

[T29] Swift：guard 提前返回
来源：http://hz.52xcode.cn/gtekthdjzk.html

guard let x = opt else { return }
来源：http://hz.xziqi.cn/gtqinugahe.html

[T30] Swift：协议
来源：http://hz.kuanghao11.cn/gtgcvaqaor.html

protocol Shape { func area() -> Double }
来源：http://hz.fengsongda.top/gtaggigkbz.html

[T31] Lua：Hello World
来源：http://hz.yj202588.top/gtaohjzwrr.html

print("Hello")
来源：http://hz.gaohongyu789.top/gtohskxokl.html

[T32] Lua：局部变量
来源：http://hz.yuxming.cn/gttlwwalai.html

local a = 1
来源：http://hz.jinqigfzy.top/gtnijrykyr.html

[T33] Lua：表（数组）
来源：http://hz.gotoacloud.top/gtwfgctnlm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.hongshengwenyu.top/gtspksqwgb.html

[T34] Lua：遍历表
来源：http://hz.xuetiantiany.cn/gtgxvnnpfi.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.gaohongyu789.top/gtuyxztkli.html

[T35] Lua：字典表
来源：http://hz.zhongyouzk.top/gtnlbsqcfa.html

local d = { a = 1 };  d.b = 2
来源：http://hz.wangshuangyany.cn/gtrnubeusw.html

[T36] Lua：函数
来源：http://hz.zhaomingkeji.xyz/gtfkwofxdc.html

function add(a, b) return a + b end
来源：http://hz.wangshuangyany.cn/gtwbxqenbe.html

[T37] Lua：字符串拼接
来源：http://hz.nanxinkj.top/gtswyhcqbx.html

"a" .. "b"
来源：http://hz.hongshengwenyu.top/gtyndefhag.html

[T38] Lua：条件
来源：http://hz.zdqjudy.top/gtunknpfbc.html

if x > 0 then print("正") end
来源：http://hz.tianlin.xyz/gtnmzuzonj.html

[T39] Lua：模式匹配
来源：http://hz.hnxiangtu.top/gtwzojogxc.html

string.find(s, "%d+")
来源：http://hz.shuidangran.top/gtbionhbdq.html

[T40] Lua：元表
来源：http://hz.yuanzhike.top/gtyluznuex.html

setmetatable({}, { __index = base })
来源：http://hz.zhixingplan.top/gtqymeyaiv.html

[T41] Perl：Hello World
来源：http://hz.jqgfzy.top/gtrmtnoprl.html

print "Hello\n";
来源：http://hz.zhijiandao.cn/gtdgepssic.html

[T42] Perl：变量类型
来源：http://hz.9152youxi.cn/gttiilyzem.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.hnqzz.top/gtpaosxllx.html

[T43] Perl：字符串插值
来源：http://hz.sxryk.cn/gtfwfnayvy.html

"值: $a"
来源：http://hz.fengsongda.top/gthvobdttv.html

[T44] Perl：条件
来源：http://hz.hnxiangtu.top/gtiicsqijk.html

if ($a > 0) { print "正"; }
来源：http://hz.iojbl.cn/gtfjxifaoe.html

[T45] Perl：数组遍历
来源：http://hz.pycfn.com/gtfjrjxlrh.html

for my $x (@arr) { print $x; }
来源：http://hz.hnqzz.top/gthhvllsan.html

[T46] Perl：哈希操作
来源：http://hz.ydzc1.top/gtnnxtczlb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.dianchejie.cn/gtvypumihx.html

[T47] Perl：正则捕获
来源：http://hz.chenzaomai.com/gtygnpsetz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yanxiufei.cn/gtwxuyapxr.html

[T48] Perl：正则替换
来源：http://hz.yonumen.top/gtmdfsatwu.html

$s =~ s/old/new/g;
来源：http://hz.xingfuxueyuan.xyz/gttpthfdyi.html

[T49] Perl：函数
来源：http://hz.guannengcc.top/gtcunauxqp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.pycfn.com/gtuvmqnrtf.html

[T50] Perl：逐行读文件
来源：http://hz.hfpthk.cn/gttrvdyugk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yj20258888.top/gtfoczzfmk.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.smart0.xyz/gtrcesmnsd.html

[T51] Scala：Hello World
来源：http://hz.yvedp.cn/gtakxuaegt.html

println("Hello")
来源：http://hz.ybcxt.top/gthscqcmyg.html

[T52] Scala：变量
来源：http://hz.cdnleiting.top/gtdctkabaw.html

val a = 1;  var b = 2
来源：http://hz.fzhhl.top/gtcjtabhxb.html

[T53] Scala：字符串插值
来源：http://hz.zhaomingkeji.xyz/gtvqherelc.html

s"值: $b"
来源：http://hz.shuidangran.top/gtnlbhyooa.html

[T54] Scala：集合映射
来源：http://hz.tian-w.cn/gtaaxawwaz.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.9152youxi.cn/gteeblubde.html

[T55] Scala：集合过滤
来源：http://hz.xylfe.cn/gtbhnsepru.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.shangyingyoupin.top/gtbhsrxklx.html

[T56] Scala：样例类
来源：http://hz.yvedp.cn/gtlsvqddso.html

case class User(name: String, age: Int)
来源：http://hz.xuetiantiany.cn/gthykdille.html

[T57] Scala：模式匹配
来源：http://hz.nwbrower.top/gtgpkxwnor.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.chenlongwang.top/gtzdbirhgd.html

[T58] Scala：函数定义
来源：http://hz.daria6918.cn/gthiyyrkre.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.shangyingyoupin.top/gtbvhiabhv.html

[T59] Scala：循环
来源：http://hz.pengpengdd.cyou/gtrajreicv.html

for (i <- 1 to 10) println(i)
来源：http://hz.xuetiantiany.cn/gtwnkmgppm.html

[T60] Scala：折叠
来源：http://hz.c1oappe.top/gtrnyiemqr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yonumen.top/gtmagewetn.html

================================================================================
来源：http://hz.gaohongyu789.top/gtsyfhzkjg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jinqigufen.top/gtvqgvyoih.html

================================================================================
来源：http://hz.zhixingplan.top/gtwzecshbk.html

[U01] Py：创建虚拟环境
来源：http://hz.xuanzx.com/gtngbcgpzb.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.0kj1m.cn/gtvbwfxoac.html

[U02] Py：导出 / 安装依赖
来源：http://hz.feifeiyinyue.top/gtomdfhdkm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.haohaochexian.top/gteezoczsu.html

[U03] Py：加载 .env 配置
来源：http://hz.sxryk.cn/gtiujlbofy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.snrcjt.cn/gtfqaiaprn.html

[U04] Py：变量调试打印
来源：http://hz.hnxiangtu.top/gtbebupvqs.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.bjfxy.top/gtnfoyiovt.html

[U05] Py：列表去重且保序
来源：http://hz.nanxinkj.top/gtudphinfz.html

list(dict.fromkeys(arr))
来源：http://hz.shanyushiyangtech.top/gtyzmdhrpc.html

[U06] Py：合并两个字典
来源：http://hz.c1oappe.top/gttwovabcp.html

{**a, **b}
来源：http://hz.tanke756.top/gtdubrtwdf.html

[U07] Py：反转字典键值
来源：http://hz.fzhhl.top/gtvgpcjanf.html

{v: k for k, v in d.items()}
来源：http://hz.nanxuanxn.top/gtsewfcuww.html

[U08] Py：展平二维列表
来源：http://hz.hnqzz.top/gtnmwhfncy.html

[y for x in nested for y in x]
来源：http://hz.c1oappe.top/gtvysuetyp.html

[U09] Py：字典取最大值的键
来源：http://hz.chenlongwang.top/gtvgwiaepn.html

max(d, key=d.get)
来源：http://hz.zhongyouzk.top/gtxgmehznw.html

[U10] Py：按值排序字典
来源：http://hz.jiagoushi.top/gtimcelpvr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.zhaomingkeji.xyz/gtaatuolmo.html

[U11] Py：生成器表达式
来源：http://hz.yuanzhike.top/gtuiwbjytv.html

(x * 2 for x in arr)
来源：http://hz.wangdashe.top/gtcafzacls.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yj202588.top/gtqvyxlfru.html

Counter(arr).most_common(3)
来源：http://hz.nanxuanxn.top/gtynxedsvs.html

[U13] Py：固定长度队列
来源：http://hz.yj20258.top/gtmhclahbb.html

deque(maxlen=10)
来源：http://hz.shuidangran.top/gtxwbnmvam.html

[U14] Py：分组收集到列表
来源：http://hz.cqqwz.cn/gtakxiklhj.html

defaultdict(list)
来源：http://hz.vqdsnc.cn/gtysxzmxwy.html

[U15] Py：高精度计时
来源：http://hz.feifeiyinyue.top/gtcdqyeesq.html

t = time.perf_counter()
来源：http://hz.daxiang520.top/gtqcsryfkg.html

[U16] Py：命令行参数解析
来源：http://hz.gzhubu.top/gtwkfshjzn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.kuanghao11.cn/gtvqhbzssu.html

[U17] Py：初始化日志
来源：http://hz.svipenyu.cn/gtpsncyaoy.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.c1oappe.top/gtxrlwmbqy.html

[U18] Py：预编译正则
来源：http://hz.hammf.cn/gttsmguozg.html

pat = re.compile(r"\d+")
来源：http://hz.smart0.xyz/gtkhezkujp.html

[U19] Py：正则替换带回调
来源：http://hz.havefunace.top/gtkdeqryyc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.ydzc1.top/gtvbmihkiu.html

[U20] Py：缓存函数结果
来源：http://hz.yj202588.top/gtdexcphiq.html

@functools.lru_cache(maxsize=None)
来源：http://hz.redwolf501.top/gtdxfvjllt.html

[U21] Py：自定义上下文管理器
来源：http://hz.kuanghao11.cn/gtehpcebar.html

@contextlib.contextmanager
来源：http://hz.hnxiangtu.top/gtmjcsgrzj.html

[U22] Py：矩阵转置
来源：http://hz.zhijiandao.cn/gtmbunrolt.html

list(zip(*m))
来源：http://hz.hfpthk.cn/gtuvbxqxnu.html

[U23] Py：分块读取大文件
来源：http://hz.zhixingplan.top/gtguadgjtb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.dianchejie.cn/gtjitdllfp.html

[U24] Py：路径操作
来源：http://hz.birdmap.top/gtlqnubkqw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.chenlongwang.top/gtkbbjuyor.html

[U25] Py：CSV 按字典读
来源：http://hz.0kj1m.cn/gtlipygdoe.html

csv.DictReader(f)
来源：http://hz.xinyue.icu/gthvepcmsb.html

[U26] Py：并发下载
来源：http://hz.haohaochexian.top/gtldlegnxj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jinqigufen.top/gtnueuhsxf.html

[U27] Py：异步 HTTP
来源：http://hz.mhx1999.top/gtbcfzbfei.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.quarkkingdee.top/gtnjkiavba.html

[U28] Py：类型别名
来源：http://hz.ydjk.org.cn/gtddjylcuc.html

UserId = int
来源：http://hz.jqgfzy.top/gtijqezbwp.html

[U29] Py：属性校验
来源：http://hz.c1oappe.top/gtrafscbbf.html

@property 与 @x.setter 配合
来源：http://hz.ivvv.top/gtumyttfgm.html

[U30] Py：数据类
来源：http://hz.chenjidiqi.icu/gttjgummif.html

@dataclass(slots=True)
来源：http://hz.tian-w.cn/gtighfsmsj.html


<!-- 参考信息 -->