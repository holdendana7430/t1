代发 wailian999

strlen(s)
来源：http://hz.jinqigufen.top/gtdtnbkdfx.html

[S06] C：字符串比较
来源：http://hz.sysykeji.top/gttadsvoxl.html

strcmp(a, b) == 0
来源：http://hz.xziqi.cn/gtnxhhzhlu.html

[S07] C：数组遍历求和
来源：http://hz.jinghuilouyu.cn/gtnklqpmiq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.mhx1999.top/gtiuemxswd.html

[S08] C：动态内存分配与释放
来源：http://hz.yanxiufei.cn/gthrajupnw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.gaohongyu789.top/gtlumidrmz.html

[S09] C：结构体定义与初始化
来源：http://hz.zhiwuduotai.top/gtxckoabta.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.snrcjt.cn/gteksmadpg.html

[S10] C：指针与解引用
来源：http://hz.jyoumei.cn/gtgsnfkenb.html

int *p = &a;  *p = 5;
来源：http://hz.jiagoushi.top/gtnwtirrya.html

[S11] C：逐行读文件
来源：http://hz.ivvv.top/gtpkdrvhyv.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.shanyushiyangkeji.top/gtwoejpzxy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.svipenyu.cn/gtsleagxbr.html

fclose(f);
来源：http://hz.hongshengwenyu.top/gtpaavjpws.html

[S12] C：写文件
来源：http://hz.snrcjt.cn/gtlgxgnuag.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.shanyushiyangtech.top/gttcdhtcfb.html

[S13] C：宏定义
来源：http://hz.yanxiufei.cn/gtjrqcnnao.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.dianchejie.cn/gtclsbolih.html

[S14] C：枚举
来源：http://hz.hongshengwenyu.top/gtilkgiwtt.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yvedp.cn/gtjnjicuux.html

[S15] C：类型转换
来源：http://hz.sweek.top/gtwqiutyjj.html

(double) a / b
来源：http://hz.nwbrower.top/gtwbigkwpn.html

[S16] C：位操作置位
来源：http://hz.guannengcc.top/gtzlndhqga.html

x |= (1 << 3);
来源：http://hz.chenlongwang.top/gtxzibcmte.html

[S17] C：安全拼接字符串
来源：http://hz.jiagoushi.top/gtgfivygff.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.meibo888.top/gtprlqwyzq.html

[S18] C：命令行参数
来源：http://hz.cdnleiting.top/gteoqmrlnn.html

int main(int argc, char **argv)
来源：http://hz.jqgufenzy.top/gtdzplgvid.html

[S19] C：快速排序
来源：http://hz.xuanzx.com/gtoylefyab.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yj20258.top/gtkipqozsf.html

[S20] C：二分查找
来源：http://hz.hysaishi.cn/gttsisbrhx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zdqjudy.top/gtxubfgjbd.html

[S21] C：字符类别判断
来源：http://hz.yanxiufei.cn/gtjniztxfn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xylfe.cn/gtpuhpgllf.html

[S22] C：字符串转数字
来源：http://hz.hfpthk.cn/gtoaeigtqd.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yonumen.top/gtvujhfqbu.html

[S23] C：随机数
来源：http://hz.yanxiufei.cn/gtnybxcdap.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.52xcode.cn/gtgqofotpj.html

[S24] C：获取本地时间
来源：http://hz.xuanzx.com/gtblqfrors.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.dashuyun.cn/gthmvecyqs.html

[S25] C：内存拷贝
来源：http://hz.kuanghao11.cn/gtzgacwees.html

memcpy(dst, src, n);
来源：http://hz.c1oappe.top/gtqngulxpf.html

[S26] C：内存清零
来源：http://hz.sweek.top/gtnbmavsxg.html

memset(a, 0, sizeof a);
来源：http://hz.smart0.xyz/gtdpaxmexr.html

[S27] C：定义常量
来源：http://hz.yonumen.top/gthrmjrown.html

const double PI = 3.14159;
来源：http://hz.jiagoushi.top/gtjdltxnqa.html

[S28] C：静态变量
来源：http://hz.jqgufenzy.top/gtpfcrvabz.html

static int counter = 0;
来源：http://hz.feifeiyinyue.top/gtpnbsmids.html

[S29] C：变参函数
来源：http://hz.dashuyun.cn/gtftnmsrer.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ybcxt.top/gtdnprfmbx.html

[S30] C：头文件保护
来源：http://hz.chenlongwang.top/gtjnydwpqn.html

#ifndef X_H
来源：http://hz.smart0.xyz/gtkshvgrlc.html

#define X_H
来源：http://hz.ivvv.top/gtrdomtsrx.html

#endif
来源：http://hz.snrcjt.cn/gtzbdsaloi.html

[S31] C++：Hello World
来源：http://hz.tianlin.xyz/gtavjnfobx.html

#include <iostream>
来源：http://hz.yongpay.top/gtwejxidiy.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jqgufenzy.top/gtezkeocje.html

[S32] C++：字符串
来源：http://hz.cqqwz.cn/gtenjnbtos.html

std::string s = "hi";  s += "!";
来源：http://hz.cdnleiting.top/gturyxibgg.html

[S33] C++：vector 增删
来源：http://hz.snrcjt.cn/gtokizkoiu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yonumen.top/gtayijajzu.html

[S34] C++：遍历 vector
来源：http://hz.daxiang520.top/gtmovomfcy.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jinqigufen.top/gtzsedawdm.html

[S35] C++：map
来源：http://hz.xingfuxueyuan.xyz/gtacvohauh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.svipenyu.cn/gtcjyhemww.html

[S36] C++：unordered_map
来源：http://hz.svipenyu.cn/gthpqdqanq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.chenjidiqi.icu/gtirnnfjzg.html

[S37] C++：set
来源：http://hz.daria6918.cn/gtaarjnkkp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yuxming.cn/gtfcytguyb.html

[S38] C++：排序
来源：http://hz.vqdsnc.cn/gtjvgkpzid.html

std::sort(v.begin(), v.end());
来源：http://hz.shanyushiyangkeji.top/gtsuyfjtwy.html

[S39] C++：自定义比较器排序
来源：http://hz.gaohongyu789.top/gtykvsluhc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.xziqi.cn/gtzlsfvgtg.html

[S40] C++：查找元素
来源：http://hz.xinyue.icu/gtqisbwkzz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jinqigufen.top/gtbpgsgkom.html

[S41] C++：类与构造函数
来源：http://hz.0kj1m.cn/gtogkxjjeg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.gzhubu.top/gtbfddrvwu.html

[S42] C++：继承与虚函数
来源：http://hz.fzhhl.top/gteqgldnzw.html

class B : public Base { public: void f() override {} };
来源：http://hz.ybcxt.top/gtinhasmpl.html

[S43] C++：智能指针
来源：http://hz.yj20258.top/gthfymuklu.html

auto p = std::make_unique<int>(5);
来源：http://hz.shanyushiyangkeji.top/gtsugtqwyi.html

[S44] C++：引用传参
来源：http://hz.wangdashe.top/gtlczmniwh.html

void inc(int &x) { ++x; }
来源：http://hz.ehwqpu.com/gtdffrvvot.html

[S45] C++：lambda
来源：http://hz.chenzaomai.com/gtregabiay.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhiwuduotai.top/gtnxakfolv.html

[S46] C++：函数模板
来源：http://hz.jqgufenzy.top/gtryknezba.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhengqikj.top/gtftigaken.html

[S47] C++：结构化绑定遍历
来源：http://hz.pengpengdd.cyou/gtvmvaftww.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.nwbrower.top/gtbxlrxejk.html

[S48] C++：逐行读文件
来源：http://hz.jinqigufen.top/gtmndhplrf.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.dianchejie.cn/gtkbrknesh.html

while (std::getline(in, line)) { }
来源：http://hz.zycfv.cn/gtfktclkcj.html

[S49] C++：写文件
来源：http://hz.sufxvd.cn/gtslhuwiac.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.chenzaomai.com/gtqzewfcjh.html

[S50] C++：格式化数字
来源：http://hz.birdmap.top/gtfplbkeki.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhongyouzk.top/gtveyfxfrj.html

[S51] C++：显式类型转换
来源：http://hz.zhengqikj.top/gtselleusv.html

static_cast<double>(a) / b
来源：http://hz.xuetiantiany.cn/gtdozkaekw.html

[S52] C++：const 与 noexcept
来源：http://hz.9152youxi.cn/gtkdazxglp.html

int size() const noexcept { return n_; }
来源：http://hz.jyoumei.cn/gtfvzrrpgs.html

[S53] C++：移动语义
来源：http://hz.cdnleiting.top/gtesfycneu.html

std::vector<int> w = std::move(v);
来源：http://hz.daxiang520.top/gtlorlhqez.html

[S54] C++：异常处理
来源：http://hz.yonumen.top/gtjpczllus.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.sysykeji.top/gtkieksiac.html

[S55] C++：结构化绑定
来源：http://hz.redwolf501.top/gtainmcpzk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhijiandao.cn/gtjiuyjrft.html

[S56] C++：optional
来源：http://hz.gzhubu.top/gtdhtwrcjp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhiwuduotai.top/gtgaqdieva.html

[S57] C++：编译期常量
来源：http://hz.tianlin.xyz/gtquefhkef.html

constexpr int N = 10;
来源：http://hz.haohaochexian.top/gtioryaxit.html

[S58] C++：命名空间
来源：http://hz.jlsjyb.cn/gtzvcrndqf.html

namespace ns { int f() { return 1; } }
来源：http://hz.jinqigufen.top/gttinjvrui.html

[S59] C++：静态断言
来源：http://hz.shuidangran.top/gtvxeyhzww.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.gotoacloud.top/gtzssaunab.html

[S60] C++：遍历并删除元素
来源：http://hz.chenzaomai.com/gtmsfkqptu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.daria6918.cn/gttdgsocup.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtarifmvfk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.mhx1999.top/gtnphjmxjv.html

================================================================================
来源：http://hz.jinqigfzy.top/gtssyweaiq.html

[T01] Kotlin：Hello World
来源：http://hz.chenlongwang.top/gtycbavtfg.html

println("Hello")
来源：http://hz.jqgufenzy.top/gtfjmhyptc.html

[T02] Kotlin：变量
来源：http://hz.gaohongyu789.top/gtkfwhgtld.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.shanyushiyangkeji.top/gtdscwrcrr.html

[T03] Kotlin：字符串模板
来源：http://hz.cucudq.cn/gtmyamoygq.html

"值: $b"
来源：http://hz.zhixingplan.top/gtjjkowyid.html

[T04] Kotlin：空安全
来源：http://hz.xuetiantiany.cn/gtileoqavz.html

val n: String? = null;  n?.length
来源：http://hz.iojbl.cn/gtykfowahc.html

[T05] Kotlin：when 表达式
来源：http://hz.sweek.top/gtlbruloba.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.316326.xyz/gthkwxpswv.html

[T06] Kotlin：集合映射
来源：http://hz.cucudq.cn/gtrqxkgopn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jinqigfzy.top/gtykbchwxr.html

[T07] Kotlin：集合过滤
来源：http://hz.daria6918.cn/gtejooimuo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hfpthk.cn/gtjdwbvcmp.html

[T08] Kotlin：数据类
来源：http://hz.hfpthk.cn/gtmkjlglpf.html

data class User(val name: String, val age: Int)
来源：http://hz.snrcjt.cn/gtocgjsuun.html

[T09] Kotlin：扩展函数
来源：http://hz.ydjk.org.cn/gtjyrjchco.html

fun String.exclaim() = this + "!"
来源：http://hz.jinghuilouyu.cn/gtdtphedrg.html

[T10] Kotlin：默认参数
来源：http://hz.hnqzz.top/gtgspgdbts.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.feifeiyinyue.top/gtquvcgiyj.html

[T11] Kotlin：协程
来源：http://hz.yonumen.top/gteshpyily.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yongpay.top/gtcskjcfcg.html

[T12] Kotlin：解构声明
来源：http://hz.shuidangran.top/gtpzdmofsm.html

val (a, b) = Pair(1, 2)
来源：http://hz.ppjwa.cn/gtbwlbhjxr.html

[T13] Kotlin：只读 Map
来源：http://hz.9152youxi.cn/gtfcqdzshc.html

val m = mapOf("a" to 1)
来源：http://hz.yuxming.cn/gtmmsfoaek.html

[T14] Kotlin：循环
来源：http://hz.shuidangran.top/gtifsxmohq.html

for (i in 1..10) println(i)
来源：http://hz.zhongyouzk.top/gtvskjgjow.html

[T15] Kotlin：接口
来源：http://hz.zhoulong.xyz/gtkvwfkszp.html

interface Shape { fun area(): Double }
来源：http://hz.hnqzz.top/gtwzomcgnx.html

[T16] Swift：Hello World
来源：http://hz.yj20258888.top/gtwribkgkp.html

print("Hello")
来源：http://hz.redwolf501.top/gtlvawsefh.html

[T17] Swift：变量与常量
来源：http://hz.chenzaomai.com/gtgvsdxzno.html

var a = 1;  let b = 2
来源：http://hz.9152youxi.cn/gtstndgadp.html

[T18] Swift：字符串插值
来源：http://hz.yongpay.top/gtrvgblfee.html

"值: \(b)"
来源：http://hz.zhoulong.xyz/gtpgxezthe.html

[T19] Swift：可选绑定
来源：http://hz.chenzaomai.com/gtkrucnkxf.html

if let n = opt { print(n) }
来源：http://hz.wangdashe.top/gtvpmqsjfv.html

[T20] Swift：数组操作
来源：http://hz.gzhubu.top/gtmmjyglvp.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.tianlin.xyz/gtnolrkrwu.html

[T21] Swift：遍历
来源：http://hz.hysaishi.cn/gtpqwqtjhd.html

for x in a { print(x) }
来源：http://hz.aibaodan.cn/gtkayojqmj.html

[T22] Swift：字典
来源：http://hz.dashuyun.cn/gthrjvsuig.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.gogol.net.cn/gtlthnmxim.html

[T23] Swift：函数
来源：http://hz.chenlongwang.top/gtmiwafahd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.tianlin.xyz/gtuibfohhf.html

[T24] Swift：闭包
来源：http://hz.zhixingplan.top/gtkbrgzbym.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.sufxvd.cn/gtpiqztvdm.html

[T25] Swift：结构体
来源：http://hz.hammf.cn/gtbvesosat.html

struct P { var x: Int }
来源：http://hz.9152youxi.cn/gtlpfabaqz.html

[T26] Swift：类与重写
来源：http://hz.0kj1m.cn/gtoqohojfc.html

class A: Base { override func f() {} }
来源：http://hz.jqgfzy.top/gtbiwbovyk.html

[T27] Swift：错误处理
来源：http://hz.gotoacloud.top/gtvieujjea.html

do { try f() } catch { print(error) }
来源：http://hz.cucudq.cn/gtxjmfzoqe.html

[T28] Swift：枚举
来源：http://hz.yj20258.top/gtfnrcwyeg.html

enum Color { case red, green }
来源：http://hz.yongpay.top/gtuskyfbpi.html

[T29] Swift：guard 提前返回
来源：http://hz.gogol.net.cn/gtfcmeatau.html

guard let x = opt else { return }
来源：http://hz.svipenyu.cn/gteobdzijz.html

[T30] Swift：协议
来源：http://hz.zhaomingkeji.xyz/gtrckkqiad.html

protocol Shape { func area() -> Double }
来源：http://hz.jinqigfzy.top/gteoqwcfuq.html

[T31] Lua：Hello World
来源：http://hz.gzhubu.top/gtzumlcjhc.html

print("Hello")
来源：http://hz.shangyingyoupin.top/gtsvfwporf.html

[T32] Lua：局部变量
来源：http://hz.tanke756.top/gtjwnxcspg.html

local a = 1
来源：http://hz.jlsjyb.cn/gtompxenzr.html

[T33] Lua：表（数组）
来源：http://hz.wangdashe.top/gtrjqtupbo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.cheryme.top/gtdhfqedmp.html

[T34] Lua：遍历表
来源：http://hz.aibaodan.cn/gtbosoxbfp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yuanzhike.top/gteooxtkqp.html

[T35] Lua：字典表
来源：http://hz.yuanzhike.top/gtbsgcblvz.html

local d = { a = 1 };  d.b = 2
来源：http://hz.guowangkeji.top/gtoykilfta.html

[T36] Lua：函数
来源：http://hz.jinyuanbaomall.cn/gtrydzasrm.html

function add(a, b) return a + b end
来源：http://hz.ydzc1.top/gtbieeiicz.html

[T37] Lua：字符串拼接
来源：http://hz.jinqigufen.top/gtmgrkupkq.html

"a" .. "b"
来源：http://hz.quarkkingdee.top/gtknnfrlls.html

[T38] Lua：条件
来源：http://hz.shangyingyoupin.top/gtulcxdfqb.html

if x > 0 then print("正") end
来源：http://hz.hnqzz.top/gtlsrqvija.html

[T39] Lua：模式匹配
来源：http://hz.nwbrower.top/gtrprcpfsu.html

string.find(s, "%d+")
来源：http://hz.shanyushiyangkeji.top/gtcgcxkemq.html

[T40] Lua：元表
来源：http://hz.shanyushiyangtech.top/gtdogihpim.html

setmetatable({}, { __index = base })
来源：http://hz.ywan-chungtsiang.top/gtjhiidsuh.html

[T41] Perl：Hello World
来源：http://hz.ywan-chungtsiang.top/gtrnzyjevw.html

print "Hello\n";
来源：http://hz.guannengcc.top/gtlfkdasyy.html

[T42] Perl：变量类型
来源：http://hz.fzhhl.top/gtyeyambxx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.birdmap.top/gtqarxsywt.html

[T43] Perl：字符串插值
来源：http://hz.shuidangran.top/gtwtxcdfth.html

"值: $a"
来源：http://hz.9152youxi.cn/gtxqrznztc.html

[T44] Perl：条件
来源：http://hz.guannengcc.top/gtlgtkvdix.html

if ($a > 0) { print "正"; }
来源：http://hz.chenjidiqi.icu/gtgtggzpti.html

[T45] Perl：数组遍历
来源：http://hz.gaohongyu789.top/gtjagpxkrw.html

for my $x (@arr) { print $x; }
来源：http://hz.hywenlv.cn/gtdiucxffk.html

[T46] Perl：哈希操作
来源：http://hz.havefunace.top/gtwhgleuau.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.mhx1999.top/gtvuckkpez.html

[T47] Perl：正则捕获
来源：http://hz.shzxlz.cn/gtcqmtzeav.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.zhoulong.xyz/gttexgomkt.html

[T48] Perl：正则替换
来源：http://hz.shangyingyoupin.top/gtacoaqutx.html

$s =~ s/old/new/g;
来源：http://hz.sufxvd.cn/gtroorufpk.html

[T49] Perl：函数
来源：http://hz.yangfankeji.com/gtabfmclox.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.ywan-chungtsiang.top/gteehdfyde.html

[T50] Perl：逐行读文件
来源：http://hz.cqqwz.cn/gtkcqlkdsh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yvedp.cn/gtqzlotxxy.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.gzhubu.top/gtyfzbvccg.html

[T51] Scala：Hello World
来源：http://hz.shuidangran.top/gtuaarfahz.html

println("Hello")
来源：http://hz.sysykeji.top/gtmlgkrpkv.html

[T52] Scala：变量
来源：http://hz.chenlongwang.top/gtknjakekt.html

val a = 1;  var b = 2
来源：http://hz.hnqzz.top/gtttgijmyv.html

[T53] Scala：字符串插值
来源：http://hz.ywan-chungtsiang.top/gthmgmcurw.html

s"值: $b"
来源：http://hz.cheryme.top/gtjayexlcq.html

[T54] Scala：集合映射
来源：http://hz.nanxinkj.top/gtsuedbazu.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.dianchejie.cn/gtmgzipsim.html

[T55] Scala：集合过滤
来源：http://hz.yj20258.top/gtwqrumapp.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jyoumei.cn/gtdsehlupl.html

[T56] Scala：样例类
来源：http://hz.pengpengdd.cyou/gtqetwrkrx.html

case class User(name: String, age: Int)
来源：http://hz.cucudq.cn/gtlhqvhvrf.html

[T57] Scala：模式匹配
来源：http://hz.jianghu66.top/gtkmwvrjsp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.shuidangran.top/gtayxztnrs.html

[T58] Scala：函数定义
来源：http://hz.meibo888.top/gtudlpxgwa.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.shanyushiyangtech.top/gtwidmfcbt.html

[T59] Scala：循环
来源：http://hz.vqdsnc.cn/gtsqatoyxq.html

for (i <- 1 to 10) println(i)
来源：http://hz.shanyushiyangtech.top/gtbonunmys.html

[T60] Scala：折叠
来源：http://hz.haohaochexian.top/gtdpiiimzr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.zhongyouzk.top/gtwsvopwsl.html

================================================================================
来源：http://hz.xylfe.cn/gtmqkhlinn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.xinyue.icu/gtaismkzux.html

================================================================================
来源：http://hz.yangfankeji.com/gthezzxzdb.html

[U01] Py：创建虚拟环境
来源：http://hz.ehwqpu.com/gtejpdfeqh.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yvedp.cn/gtupsxxtiq.html

[U02] Py：导出 / 安装依赖
来源：http://hz.pengpengdd.cyou/gtewfaeqag.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jlsjyb.cn/gtmqrzrmtw.html

[U03] Py：加载 .env 配置
来源：http://hz.hnxiangtu.top/gtxnjfbgkv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.ehwqpu.com/gtwavniqfi.html

[U04] Py：变量调试打印
来源：http://hz.nanxuanxn.top/gthwkzwllw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.shanyushiyangkeji.top/gttofwwpxo.html

[U05] Py：列表去重且保序
来源：http://hz.pycfn.com/gtnreuwnmg.html

list(dict.fromkeys(arr))
来源：http://hz.zhiwuduotai.top/gtzkzhjkuz.html

[U06] Py：合并两个字典
来源：http://hz.zhixingplan.top/gtcybdylwo.html

{**a, **b}
来源：http://hz.havefunace.top/gtwkkqbwzm.html

[U07] Py：反转字典键值
来源：http://hz.meibo888.top/gthhdycjci.html

{v: k for k, v in d.items()}
来源：http://hz.aizwys.cn/gtrdatnkiz.html

[U08] Py：展平二维列表
来源：http://hz.jlsjyb.cn/gtyaayhqkh.html

[y for x in nested for y in x]
来源：http://hz.yj20258888.top/gtdrqojjlu.html

[U09] Py：字典取最大值的键
来源：http://hz.shangyingyoupin.top/gtjjtdagup.html

max(d, key=d.get)
来源：http://hz.cheryme.top/gtlpogidpf.html

[U10] Py：按值排序字典
来源：http://hz.52xcode.cn/gthetndimw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.birdmap.top/gtizplkyrw.html

[U11] Py：生成器表达式
来源：http://hz.zhijiandao.cn/gtrvbbhcol.html

(x * 2 for x in arr)
来源：http://hz.chenjidiqi.icu/gtmembxbhh.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.xuetiantiany.cn/gtpsdfebii.html

Counter(arr).most_common(3)
来源：http://hz.aizwys.cn/gtxyvibotd.html

[U13] Py：固定长度队列
来源：http://hz.aibaodan.cn/gtryekytgq.html

deque(maxlen=10)
来源：http://hz.jlsjyb.cn/gtdntpazyu.html

[U14] Py：分组收集到列表
来源：http://hz.yuxming.cn/gtawkhyyia.html

defaultdict(list)
来源：http://hz.jyoumei.cn/gtotxllexa.html

[U15] Py：高精度计时
来源：http://hz.fzhhl.top/gtifhjplqm.html

t = time.perf_counter()
来源：http://hz.yuanzhike.top/gttffulmnh.html

[U16] Py：命令行参数解析
来源：http://hz.cdnleiting.top/gthbdjssxy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.xuetiantiany.cn/gtlxnoymnq.html

[U17] Py：初始化日志
来源：http://hz.yj202588.top/gtfxlouhnr.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.jinyuanbaomall.cn/gtpwiwerzo.html

[U18] Py：预编译正则
来源：http://hz.xuetiantiany.cn/gtuiwoseuk.html

pat = re.compile(r"\d+")
来源：http://hz.shuidangran.top/gtkewuyqmo.html

[U19] Py：正则替换带回调
来源：http://hz.jinghuilouyu.cn/gtudhagyra.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.jqgufenzy.top/gtnivskzcf.html

[U20] Py：缓存函数结果
来源：http://hz.jlsjyb.cn/gtcqcctmxl.html

@functools.lru_cache(maxsize=None)
来源：http://hz.sysykeji.top/gtwxgmdgtz.html

[U21] Py：自定义上下文管理器
来源：http://hz.jqgfzy.top/gtypqwnbvm.html

@contextlib.contextmanager
来源：http://hz.feifeiyinyue.top/gtzuynibzs.html

[U22] Py：矩阵转置
来源：http://hz.jinyuanbaomall.cn/gtvsiojhik.html

list(zip(*m))
来源：http://hz.quarkkingdee.top/gtqtmprwog.html

[U23] Py：分块读取大文件
来源：http://hz.nanxuanxn.top/gtupftazll.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yangfankeji.com/gtrqkztlhx.html

[U24] Py：路径操作
来源：http://hz.9152youxi.cn/gtrxxvtbij.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.tianlin.xyz/gtosoawpkc.html

[U25] Py：CSV 按字典读
来源：http://hz.jqgfzy.top/gtdmuibdfe.html

csv.DictReader(f)
来源：http://hz.tianlin.xyz/gtqgolgarc.html

[U26] Py：并发下载
来源：http://hz.jianghu66.top/gtxfkrosfg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.nwbrower.top/gtvmimytti.html

[U27] Py：异步 HTTP
来源：http://hz.jiagoushi.top/gtxowxmxve.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.zhixingplan.top/gtxqigdvpz.html

[U28] Py：类型别名
来源：http://hz.gaohongyu789.top/gtxkuxilaw.html

UserId = int
来源：http://hz.hysaishi.cn/gtupawtqqm.html


<!-- 参考信息 -->