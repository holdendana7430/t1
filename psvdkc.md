代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.aizwys.cn/gtepkxfryx.html

[S08] C：动态内存分配与释放
来源：http://hz.316326.xyz/gtbhmvdqyw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xinyue.icu/gtgzthgrzn.html

[S09] C：结构体定义与初始化
来源：http://hz.yueranfly.top/gtexrnmnbq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xinyue.icu/gtfqbutobo.html

[S10] C：指针与解引用
来源：http://hz.shzxlz.cn/gtonmcdmog.html

int *p = &a;  *p = 5;
来源：http://hz.nanxuanxn.top/gtoqwjaccg.html

[S11] C：逐行读文件
来源：http://hz.fzhhl.top/gttugfhimn.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jinqigfzy.top/gtifjdooct.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hfpthk.cn/gtfresttmv.html

fclose(f);
来源：http://hz.dashuyun.cn/gtrjqxaygi.html

[S12] C：写文件
来源：http://hz.nanxinkj.top/gtoyermzjp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xuanzx.com/gtwwwnbxsw.html

[S13] C：宏定义
来源：http://hz.smart0.xyz/gthxeqipyh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.shzxlz.cn/gtxbaapeqg.html

[S14] C：枚举
来源：http://hz.meibo888.top/gtzivncvfs.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jinqigfzy.top/gtvrtqnune.html

[S15] C：类型转换
来源：http://hz.sxryk.cn/gtwwbvkffj.html

(double) a / b
来源：http://hz.yonumen.top/gtagtbdtor.html

[S16] C：位操作置位
来源：http://hz.ehwqpu.com/gtyjbinnsf.html

x |= (1 << 3);
来源：http://hz.hnqzz.top/gtngnwkoru.html

[S17] C：安全拼接字符串
来源：http://hz.wangshuangyany.cn/gtxfhbvnkk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yongpay.top/gtxfomauqw.html

[S18] C：命令行参数
来源：http://hz.birdmap.top/gtrxgpsevb.html

int main(int argc, char **argv)
来源：http://hz.316326.xyz/gtdbrymnzk.html

[S19] C：快速排序
来源：http://hz.shanyushiyangtech.top/gtiymzchid.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.daxiang520.top/gtgvhbqkxv.html

[S20] C：二分查找
来源：http://hz.zhijiandao.cn/gtrgrljagq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.xingfuxueyuan.xyz/gtbgieeasu.html

[S21] C：字符类别判断
来源：http://hz.yueranfly.top/gtxkrkgluj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hnxiangtu.top/gtrafustyn.html

[S22] C：字符串转数字
来源：http://hz.shangyingyoupin.top/gtfikhgtwg.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.havefunace.top/gtozsgsmjw.html

[S23] C：随机数
来源：http://hz.0kj1m.cn/gtessghaor.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jinqigufen.top/gtdedagbfd.html

[S24] C：获取本地时间
来源：http://hz.gzhubu.top/gtikrhtnmv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.gotoacloud.top/gtusyugtqo.html

[S25] C：内存拷贝
来源：http://hz.ydzc1.top/gtptfbluuc.html

memcpy(dst, src, n);
来源：http://hz.jqgufenzy.top/gtclssnjjj.html

[S26] C：内存清零
来源：http://hz.sxryk.cn/gtpronevls.html

memset(a, 0, sizeof a);
来源：http://hz.chenzaomai.com/gtkwsbxsvo.html

[S27] C：定义常量
来源：http://hz.316326.xyz/gtfqxfvfhs.html

const double PI = 3.14159;
来源：http://hz.birdmap.top/gtsffpexbr.html

[S28] C：静态变量
来源：http://hz.dashuyun.cn/gtygtgkqav.html

static int counter = 0;
来源：http://hz.shangyingyoupin.top/gtnrrdkmuy.html

[S29] C：变参函数
来源：http://hz.sxryk.cn/gtwzohzttv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jinyuanbaomall.cn/gtquoeuvft.html

[S30] C：头文件保护
来源：http://hz.daria6918.cn/gtdywjxyvm.html

#ifndef X_H
来源：http://hz.vqdsnc.cn/gtoosigrde.html

#define X_H
来源：http://hz.gotoacloud.top/gtjnnjflmx.html

#endif
来源：http://hz.zdqjudy.top/gtvpgxbtxi.html

[S31] C++：Hello World
来源：http://hz.tian-w.cn/gthsjfdzyr.html

#include <iostream>
来源：http://hz.yj20258.top/gtkunlzksg.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yueranfly.top/gtpeluhbod.html

[S32] C++：字符串
来源：http://hz.tianlin.xyz/gtsbftozmx.html

std::string s = "hi";  s += "!";
来源：http://hz.9152youxi.cn/gtxpwmsfns.html

[S33] C++：vector 增删
来源：http://hz.9152youxi.cn/gtdyiivrcs.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.sufxvd.cn/gtpbolflog.html

[S34] C++：遍历 vector
来源：http://hz.kuanghao11.cn/gtsxpsblar.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yueranfly.top/gtjfuzhnhe.html

[S35] C++：map
来源：http://hz.ydzc1.top/gtoeyrxjgu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.316326.xyz/gtaqbvvorc.html

[S36] C++：unordered_map
来源：http://hz.zhixingplan.top/gtsspszuwq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nwbrower.top/gtsmhmjtyx.html

[S37] C++：set
来源：http://hz.yj20258888.top/gtxtbferdj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.vqdsnc.cn/gtcgjxlfdz.html

[S38] C++：排序
来源：http://hz.jinqigfzy.top/gtyveqfdqz.html

std::sort(v.begin(), v.end());
来源：http://hz.gaohongyu789.top/gtotxteurs.html

[S39] C++：自定义比较器排序
来源：http://hz.ydzc1.top/gtgfaxipol.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.316326.xyz/gtyociyqrk.html

[S40] C++：查找元素
来源：http://hz.jinqigfzy.top/gtbwfluyns.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.chenjidiqi.icu/gtfwsuojvm.html

[S41] C++：类与构造函数
来源：http://hz.jinqigufen.top/gtnpbhadqx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.gogol.net.cn/gtkpfuchbq.html

[S42] C++：继承与虚函数
来源：http://hz.mhx1999.top/gtzaeomglv.html

class B : public Base { public: void f() override {} };
来源：http://hz.smart0.xyz/gtaqmigjwu.html

[S43] C++：智能指针
来源：http://hz.sysykeji.top/gtqcgftrot.html

auto p = std::make_unique<int>(5);
来源：http://hz.kuanghao11.cn/gtosayljpa.html

[S44] C++：引用传参
来源：http://hz.vqdsnc.cn/gtmkkqsvjn.html

void inc(int &x) { ++x; }
来源：http://hz.52xcode.cn/gtjfswvnxz.html

[S45] C++：lambda
来源：http://hz.fzhhl.top/gtqhtobpje.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.sysykeji.top/gtxzvsxmlh.html

[S46] C++：函数模板
来源：http://hz.sxryk.cn/gtbfawqoiw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhixingplan.top/gtgaluwomr.html

[S47] C++：结构化绑定遍历
来源：http://hz.wangshuangyany.cn/gtyoswmwfq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.pengpengdd.cyou/gtulgcmjti.html

[S48] C++：逐行读文件
来源：http://hz.zhiwuduotai.top/gtpjoryowa.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.havefunace.top/gtkcgkofes.html

while (std::getline(in, line)) { }
来源：http://hz.jinghuilouyu.cn/gtnbaddfvq.html

[S49] C++：写文件
来源：http://hz.jqgfzy.top/gtiwpnrtkl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.xziqi.cn/gtymwqansa.html

[S50] C++：格式化数字
来源：http://hz.tanke756.top/gtivhvbfel.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.sxryk.cn/gtuitflgsx.html

[S51] C++：显式类型转换
来源：http://hz.guowangkeji.top/gtkfotxyah.html

static_cast<double>(a) / b
来源：http://hz.daxiang520.top/gtbemwnkuz.html

[S52] C++：const 与 noexcept
来源：http://hz.tanke756.top/gtsulxkbjm.html

int size() const noexcept { return n_; }
来源：http://hz.wangshuangyany.cn/gtwhqzmpui.html

[S53] C++：移动语义
来源：http://hz.cdnleiting.top/gtoksmlrvw.html

std::vector<int> w = std::move(v);
来源：http://hz.hfpthk.cn/gtgfnlpokz.html

[S54] C++：异常处理
来源：http://hz.ybcxt.top/gtfkjoysql.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jlsjyb.cn/gtxgtcqoxa.html

[S55] C++：结构化绑定
来源：http://hz.yj202588.top/gtyctwpeos.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.0kj1m.cn/gtxgcuytfk.html

[S56] C++：optional
来源：http://hz.meibo888.top/gtnhtudoyg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hywenlv.cn/gtfbwvbakr.html

[S57] C++：编译期常量
来源：http://hz.smart0.xyz/gtyzjjxgbs.html

constexpr int N = 10;
来源：http://hz.aizwys.cn/gtbcvuzcsm.html

[S58] C++：命名空间
来源：http://hz.ywan-chungtsiang.top/gtoarjlfgy.html

namespace ns { int f() { return 1; } }
来源：http://hz.redwolf501.top/gtvgyvgbtt.html

[S59] C++：静态断言
来源：http://hz.fzhhl.top/gtjxwhnrri.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xinyue.icu/gtnlzimsqj.html

[S60] C++：遍历并删除元素
来源：http://hz.yvedp.cn/gtssvbmkzq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.sufxvd.cn/gtfddvkhpb.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtczhmksix.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cqqwz.cn/gtjljiuips.html

================================================================================
来源：http://hz.yangfankeji.com/gtlfufznmm.html

[T01] Kotlin：Hello World
来源：http://hz.haohaochexian.top/gtusmhhzyc.html

println("Hello")
来源：http://hz.svipenyu.cn/gtwzadylsg.html

[T02] Kotlin：变量
来源：http://hz.cqqwz.cn/gtowxxtuok.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xziqi.cn/gtwaajtpne.html

[T03] Kotlin：字符串模板
来源：http://hz.xuanzx.com/gtxkokjqvf.html

"值: $b"
来源：http://hz.zhaomingkeji.xyz/gtpfizjegt.html

[T04] Kotlin：空安全
来源：http://hz.cqqwz.cn/gtiwxlvlzf.html

val n: String? = null;  n?.length
来源：http://hz.zhaomingkeji.xyz/gtjhtgubtv.html

[T05] Kotlin：when 表达式
来源：http://hz.cucudq.cn/gtntcsbjvh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.0kj1m.cn/gttdffzsrl.html

[T06] Kotlin：集合映射
来源：http://hz.yj20258.top/gtomdlpqhq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.iojbl.cn/gtogdnpudj.html

[T07] Kotlin：集合过滤
来源：http://hz.xziqi.cn/gtokygciri.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhixingplan.top/gtvmypvmsi.html

[T08] Kotlin：数据类
来源：http://hz.yonumen.top/gtkpjqsgfo.html

data class User(val name: String, val age: Int)
来源：http://hz.hnqzz.top/gtlqtstgwx.html

[T09] Kotlin：扩展函数
来源：http://hz.xingfuxueyuan.xyz/gtnwghuxba.html

fun String.exclaim() = this + "!"
来源：http://hz.jinqigufen.top/gtpfgsvsdv.html

[T10] Kotlin：默认参数
来源：http://hz.zycfv.cn/gtbbegvqlw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.gaohongyu789.top/gtmyqkyjcx.html

[T11] Kotlin：协程
来源：http://hz.kuanghao11.cn/gtxozofdbq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.dashuyun.cn/gtnovbljqd.html

[T12] Kotlin：解构声明
来源：http://hz.316326.xyz/gttcpzolnu.html

val (a, b) = Pair(1, 2)
来源：http://hz.sysykeji.top/gttanntvxq.html

[T13] Kotlin：只读 Map
来源：http://hz.yuxming.cn/gtolfmgmbx.html

val m = mapOf("a" to 1)
来源：http://hz.0kj1m.cn/gtwkqwugdg.html

[T14] Kotlin：循环
来源：http://hz.wangshuangyany.cn/gtrmpwdknj.html

for (i in 1..10) println(i)
来源：http://hz.jlsjyb.cn/gtixmoyhoo.html

[T15] Kotlin：接口
来源：http://hz.yj20258888.top/gtybwcjgll.html

interface Shape { fun area(): Double }
来源：http://hz.zhijiandao.cn/gtfmbxfwxl.html

[T16] Swift：Hello World
来源：http://hz.zhongyouzk.top/gtuefzcptd.html

print("Hello")
来源：http://hz.xinyue.icu/gtbixmqcdz.html

[T17] Swift：变量与常量
来源：http://hz.jianghu66.top/gterijjgsb.html

var a = 1;  let b = 2
来源：http://hz.xziqi.cn/gtlbtdzzdw.html

[T18] Swift：字符串插值
来源：http://hz.aibaodan.cn/gtpesztuxh.html

"值: \(b)"
来源：http://hz.gzhubu.top/gtiulrrhfw.html

[T19] Swift：可选绑定
来源：http://hz.cqqwz.cn/gtcllnfrky.html

if let n = opt { print(n) }
来源：http://hz.jianghu66.top/gtwcjjotdd.html

[T20] Swift：数组操作
来源：http://hz.feifeiyinyue.top/gtfvnqjffw.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.sxryk.cn/gtlyvnpooy.html

[T21] Swift：遍历
来源：http://hz.xingfuxueyuan.xyz/gtmzqexeha.html

for x in a { print(x) }
来源：http://hz.aizwys.cn/gtghjlossj.html

[T22] Swift：字典
来源：http://hz.xuanzx.com/gtwhjmawgn.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.chenzaomai.com/gtkdwqvtpu.html

[T23] Swift：函数
来源：http://hz.zycfv.cn/gtuoxnpjft.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.kuanghao11.cn/gtpkcnfazl.html

[T24] Swift：闭包
来源：http://hz.chenjidiqi.icu/gtfzffxtoe.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.smart0.xyz/gtcmxmqkre.html

[T25] Swift：结构体
来源：http://hz.nanxinkj.top/gtxzjdvzrf.html

struct P { var x: Int }
来源：http://hz.gzhubu.top/gtcukkyumt.html

[T26] Swift：类与重写
来源：http://hz.guannengcc.top/gtlcllnlsx.html

class A: Base { override func f() {} }
来源：http://hz.sxryk.cn/gtxiakgbad.html

[T27] Swift：错误处理
来源：http://hz.vqdsnc.cn/gthlswwswm.html

do { try f() } catch { print(error) }
来源：http://hz.snrcjt.cn/gtyppwceaq.html

[T28] Swift：枚举
来源：http://hz.zdqjudy.top/gtnfbjtaye.html

enum Color { case red, green }
来源：http://hz.gotoacloud.top/gtargzuczu.html

[T29] Swift：guard 提前返回
来源：http://hz.guowangkeji.top/gtzkiolbri.html

guard let x = opt else { return }
来源：http://hz.jlsjyb.cn/gttlxkitmh.html

[T30] Swift：协议
来源：http://hz.yj20258888.top/gtylvszaaw.html

protocol Shape { func area() -> Double }
来源：http://hz.jiagoushi.top/gtcqxnzfaa.html

[T31] Lua：Hello World
来源：http://hz.cqqwz.cn/gttigthqcy.html

print("Hello")
来源：http://hz.shanyushiyangtech.top/gtzopjpuyr.html

[T32] Lua：局部变量
来源：http://hz.hfpthk.cn/gtqsjedszh.html

local a = 1
来源：http://hz.iojbl.cn/gtdjewrsia.html

[T33] Lua：表（数组）
来源：http://hz.xingfuxueyuan.xyz/gtqloxwqbd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.dashuyun.cn/gtndfpfuff.html

[T34] Lua：遍历表
来源：http://hz.hnxiangtu.top/gtluduyyvu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.gogol.net.cn/gtydnpbsec.html

[T35] Lua：字典表
来源：http://hz.xziqi.cn/gthfngphbc.html

local d = { a = 1 };  d.b = 2
来源：http://hz.ehwqpu.com/gthluujypg.html

[T36] Lua：函数
来源：http://hz.ywan-chungtsiang.top/gtybsjmlcm.html

function add(a, b) return a + b end
来源：http://hz.shuidangran.top/gtchadzwaj.html

[T37] Lua：字符串拼接
来源：http://hz.gogol.net.cn/gtcxslgcpx.html

"a" .. "b"
来源：http://hz.sufxvd.cn/gtrombdvus.html

[T38] Lua：条件
来源：http://hz.chenzaomai.com/gtbxhvukuq.html

if x > 0 then print("正") end
来源：http://hz.guowangkeji.top/gtvdzozkxu.html

[T39] Lua：模式匹配
来源：http://hz.svipenyu.cn/gtewpqapmd.html

string.find(s, "%d+")
来源：http://hz.bjfxy.top/gteqsbnthv.html

[T40] Lua：元表
来源：http://hz.yj20258888.top/gtyaeinooj.html

setmetatable({}, { __index = base })
来源：http://hz.cashguo.top/gtzsbrvaeg.html

[T41] Perl：Hello World
来源：http://hz.smart0.xyz/gtikfephhn.html

print "Hello\n";
来源：http://hz.cqqwz.cn/gtxcswkyvh.html

[T42] Perl：变量类型
来源：http://hz.dashuyun.cn/gthsxfvnpk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.hywenlv.cn/gtdelqghdp.html

[T43] Perl：字符串插值
来源：http://hz.vqdsnc.cn/gtuzkilvij.html

"值: $a"
来源：http://hz.hnxiangtu.top/gtmusibrer.html

[T44] Perl：条件
来源：http://hz.fzhhl.top/gtmwyjdynq.html

if ($a > 0) { print "正"; }
来源：http://hz.yuxming.cn/gtiuvztida.html

[T45] Perl：数组遍历
来源：http://hz.zhongyouzk.top/gtbdxadudl.html

for my $x (@arr) { print $x; }
来源：http://hz.yongpay.top/gtkcewykbw.html

[T46] Perl：哈希操作
来源：http://hz.dianchejie.cn/gtilhjhenw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.gogol.net.cn/gtgykhmocb.html

[T47] Perl：正则捕获
来源：http://hz.nwbrower.top/gtueigwbfw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.iojbl.cn/gtytcidicb.html

[T48] Perl：正则替换
来源：http://hz.aizwys.cn/gtcpffjirs.html

$s =~ s/old/new/g;
来源：http://hz.tian-w.cn/gtmqcithtd.html

[T49] Perl：函数
来源：http://hz.redwolf501.top/gtdeqfsdie.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.dianchejie.cn/gtjhqdtnvv.html

[T50] Perl：逐行读文件
来源：http://hz.snrcjt.cn/gttjvytqfx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.cashguo.top/gtirbbjftl.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.meibo888.top/gtmwiuvwxl.html

[T51] Scala：Hello World
来源：http://hz.dianchejie.cn/gtqmhncqlj.html

println("Hello")
来源：http://hz.gzhubu.top/gtwerbutgu.html

[T52] Scala：变量
来源：http://hz.sxryk.cn/gtmlbzhchg.html

val a = 1;  var b = 2
来源：http://hz.gotoacloud.top/gtbhjknfnz.html

[T53] Scala：字符串插值
来源：http://hz.xuetiantiany.cn/gtonmjzdeq.html

s"值: $b"
来源：http://hz.nanxinkj.top/gtmfxgivcr.html

[T54] Scala：集合映射
来源：http://hz.hammf.cn/gtecwczdum.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.guowangkeji.top/gtlbmrzfnw.html

[T55] Scala：集合过滤
来源：http://hz.zycfv.cn/gtfhtdylli.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.svipenyu.cn/gtrvmxywck.html

[T56] Scala：样例类
来源：http://hz.zhixingplan.top/gtpfkmgwgk.html

case class User(name: String, age: Int)
来源：http://hz.smart0.xyz/gtrbzeofpl.html

[T57] Scala：模式匹配
来源：http://hz.hammf.cn/gtixkucsan.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.jyoumei.cn/gtxhgwgpos.html

[T58] Scala：函数定义
来源：http://hz.bjfxy.top/gtzhhsppjp.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zhongyouzk.top/gtsxhpgxdk.html

[T59] Scala：循环
来源：http://hz.zhaomingkeji.xyz/gtxjgtiwkq.html

for (i <- 1 to 10) println(i)
来源：http://hz.yj202588.top/gtgdxuitju.html

[T60] Scala：折叠
来源：http://hz.yuxming.cn/gtosdhderj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.jiagoushi.top/gtlsbzqied.html

================================================================================
来源：http://hz.snrcjt.cn/gtjtiofata.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.xingfuxueyuan.xyz/gtrgpffglp.html

================================================================================
来源：http://hz.kuanghao11.cn/gtgjjgtdgd.html

[U01] Py：创建虚拟环境
来源：http://hz.gaohongyu789.top/gtwubzqfur.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.fzhhl.top/gtdzfshbgl.html

[U02] Py：导出 / 安装依赖
来源：http://hz.zycfv.cn/gtbumotwmb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jlsjyb.cn/gtxhdefcyw.html

[U03] Py：加载 .env 配置
来源：http://hz.zhijiandao.cn/gtypeuxdrh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zdqjudy.top/gtjutkelfx.html

[U04] Py：变量调试打印
来源：http://hz.zhongyouzk.top/gtngfbvqrh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.nwbrower.top/gtscslkbcz.html

[U05] Py：列表去重且保序
来源：http://hz.cqqwz.cn/gtaqafpgyv.html

list(dict.fromkeys(arr))
来源：http://hz.nwbrower.top/gttaocjoxj.html

[U06] Py：合并两个字典
来源：http://hz.guowangkeji.top/gtwvjoeubz.html

{**a, **b}
来源：http://hz.xingfuxueyuan.xyz/gtaxzugxpq.html

[U07] Py：反转字典键值
来源：http://hz.xuetiantiany.cn/gtmdeiwflh.html

{v: k for k, v in d.items()}
来源：http://hz.ydzc1.top/gtmjnwewvf.html

[U08] Py：展平二维列表
来源：http://hz.zhengqikj.top/gtazeomjwo.html

[y for x in nested for y in x]
来源：http://hz.sweek.top/gthipwuosr.html

[U09] Py：字典取最大值的键
来源：http://hz.fzhhl.top/gtkmwehfew.html

max(d, key=d.get)
来源：http://hz.yj20258.top/gthjwhhasd.html

[U10] Py：按值排序字典
来源：http://hz.chenjidiqi.icu/gtmtoioloa.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.kuanghao11.cn/gthiqlinev.html

[U11] Py：生成器表达式
来源：http://hz.zhiwuduotai.top/gtrdmhbrmu.html

(x * 2 for x in arr)
来源：http://hz.cheryme.top/gtouxczjvw.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.chenlongwang.top/gtebytitjd.html

Counter(arr).most_common(3)
来源：http://hz.9152youxi.cn/gtgntemrva.html

[U13] Py：固定长度队列
来源：http://hz.shanyushiyangkeji.top/gtjxkcmnfx.html

deque(maxlen=10)
来源：http://hz.sufxvd.cn/gtxjsvvqin.html

[U14] Py：分组收集到列表
来源：http://hz.zdqjudy.top/gtyitzsoza.html

defaultdict(list)
来源：http://hz.hammf.cn/gtssjhefmh.html

[U15] Py：高精度计时
来源：http://hz.daxiang520.top/gtmpvcrfnx.html

t = time.perf_counter()
来源：http://hz.zhaomingkeji.xyz/gtdelmxiqf.html

[U16] Py：命令行参数解析
来源：http://hz.meibo888.top/gtwjqvoayw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.gogol.net.cn/gtrjsuxifu.html

[U17] Py：初始化日志
来源：http://hz.jinyuanbaomall.cn/gtylacauwy.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.svipenyu.cn/gtfrhigdoq.html

[U18] Py：预编译正则
来源：http://hz.316326.xyz/gthhibuzdk.html

pat = re.compile(r"\d+")
来源：http://hz.cashguo.top/gthflvrqax.html

[U19] Py：正则替换带回调
来源：http://hz.sxryk.cn/gtafcqrnbi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.hywenlv.cn/gtloqpqjez.html

[U20] Py：缓存函数结果
来源：http://hz.feifeiyinyue.top/gtbufhldlu.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jiagoushi.top/gtgsnfohbr.html

[U21] Py：自定义上下文管理器
来源：http://hz.dianchejie.cn/gtriowczbq.html

@contextlib.contextmanager
来源：http://hz.yanxiufei.cn/gtdrahiwwe.html

[U22] Py：矩阵转置
来源：http://hz.zycfv.cn/gtetjhyaxq.html

list(zip(*m))
来源：http://hz.jinyuanbaomall.cn/gthmdkwgmv.html

[U23] Py：分块读取大文件
来源：http://hz.smart0.xyz/gtfrqompga.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.0kj1m.cn/gttuywwzlz.html

[U24] Py：路径操作
来源：http://hz.yueranfly.top/gtxybwosfo.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.316326.xyz/gteypnhujq.html

[U25] Py：CSV 按字典读
来源：http://hz.aibaodan.cn/gtuyvsaylj.html

csv.DictReader(f)
来源：http://hz.daxiang520.top/gtgwucjanl.html

[U26] Py：并发下载
来源：http://hz.jinghuilouyu.cn/gtsppvhbez.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jinqigfzy.top/gtbntuotxc.html

[U27] Py：异步 HTTP
来源：http://hz.nwbrower.top/gtcqytmooz.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.shanyushiyangkeji.top/gtaotngehf.html

[U28] Py：类型别名
来源：http://hz.bjfxy.top/gtvkivscyq.html

UserId = int
来源：http://hz.xuetiantiany.cn/gtzmyicgwe.html

[U29] Py：属性校验
来源：http://hz.ybcxt.top/gtsbgyzrcs.html

@property 与 @x.setter 配合
来源：http://hz.zycfv.cn/gtpvfthsrz.html

[U30] Py：数据类
来源：http://hz.zhijiandao.cn/gtshmadkal.html

@dataclass(slots=True)
来源：http://hz.shangyingyoupin.top/gtswzgghsx.html


<!-- 参考信息 -->