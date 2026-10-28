代发 wailian999

int x; scanf("%d", &x);
来源：http://hz.daxiang520.top/gtiijtzcws.html

[S04] C：字符串复制
来源：http://hz.jinyuanbaomall.cn/gtkckigsqf.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.gaohongyu789.top/gtrhfyodtq.html

[S05] C：字符串长度
来源：http://hz.snrcjt.cn/gtsbyvhztf.html

strlen(s)
来源：http://hz.meibo888.top/gtevpsvyip.html

[S06] C：字符串比较
来源：http://hz.chenjidiqi.icu/gtacmrwniz.html

strcmp(a, b) == 0
来源：http://hz.redwolf501.top/gtjdwjkpxs.html

[S07] C：数组遍历求和
来源：http://hz.xylfe.cn/gtddrkxouq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hfpthk.cn/gtnmrydmep.html

[S08] C：动态内存分配与释放
来源：http://hz.zycfv.cn/gttfqrthqf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.cqqwz.cn/gthjsqaaqe.html

[S09] C：结构体定义与初始化
来源：http://hz.guannengcc.top/gtfrppgurn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ydzc1.top/gtkrxpttll.html

[S10] C：指针与解引用
来源：http://hz.zhongyouzk.top/gtulhjwews.html

int *p = &a;  *p = 5;
来源：http://hz.sxryk.cn/gtsscyanyi.html

[S11] C：逐行读文件
来源：http://hz.shanyushiyangtech.top/gtcghlisaf.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ehwqpu.com/gtrvlwvceg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ppjwa.cn/gtahcyydyt.html

fclose(f);
来源：http://hz.fengsongda.top/gtuvxujobx.html

[S12] C：写文件
来源：http://hz.52xcode.cn/gtvujhuygf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.0kj1m.cn/gtwmlvvdah.html

[S13] C：宏定义
来源：http://hz.gogol.net.cn/gtmrutetzi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.smart0.xyz/gtruesacof.html

[S14] C：枚举
来源：http://hz.sufxvd.cn/gtdkvkuifc.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.cashguo.top/gtvhqtajzv.html

[S15] C：类型转换
来源：http://hz.shzxlz.cn/gtamlzfbpv.html

(double) a / b
来源：http://hz.hongshengwenyu.top/gtvesiqcly.html

[S16] C：位操作置位
来源：http://hz.gzhubu.top/gthkdpklfv.html

x |= (1 << 3);
来源：http://hz.hysaishi.cn/gtrlsnwrsj.html

[S17] C：安全拼接字符串
来源：http://hz.xinyue.icu/gtsryrqnxe.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.52xcode.cn/gtbuzpjtqt.html

[S18] C：命令行参数
来源：http://hz.zhixingplan.top/gtvnbybftb.html

int main(int argc, char **argv)
来源：http://hz.birdmap.top/gtjfcrfifm.html

[S19] C：快速排序
来源：http://hz.yj20258.top/gtvqrpdqcy.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jyoumei.cn/gtptrcbzqx.html

[S20] C：二分查找
来源：http://hz.ppjwa.cn/gtasqlaicy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.shzxlz.cn/gtvlaofjlr.html

[S21] C：字符类别判断
来源：http://hz.yuxming.cn/gtuzyxucqt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.fzhhl.top/gthoyzkean.html

[S22] C：字符串转数字
来源：http://hz.yonumen.top/gtjxhuhgwy.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ehwqpu.com/gtzgrbyoue.html

[S23] C：随机数
来源：http://hz.yonumen.top/gtesptoang.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.ydjk.org.cn/gtttprjxca.html

[S24] C：获取本地时间
来源：http://hz.hammf.cn/gtelkafkbs.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jlsjyb.cn/gtriftctca.html

[S25] C：内存拷贝
来源：http://hz.vqdsnc.cn/gtgxavkvzl.html

memcpy(dst, src, n);
来源：http://hz.xziqi.cn/gtagthubtb.html

[S26] C：内存清零
来源：http://hz.xingfuxueyuan.xyz/gtmbjwrmsi.html

memset(a, 0, sizeof a);
来源：http://hz.svipenyu.cn/gtdcvjwidj.html

[S27] C：定义常量
来源：http://hz.hysaishi.cn/gtdtjvtpep.html

const double PI = 3.14159;
来源：http://hz.jinghuilouyu.cn/gtbkreieop.html

[S28] C：静态变量
来源：http://hz.jiagoushi.top/gttebdmohw.html

static int counter = 0;
来源：http://hz.wangshuangyany.cn/gtocrjqnsp.html

[S29] C：变参函数
来源：http://hz.havefunace.top/gtwodsvgdz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.tianlin.xyz/gtgdfohdbk.html

[S30] C：头文件保护
来源：http://hz.mhx1999.top/gtzviqowyl.html

#ifndef X_H
来源：http://hz.jinqigfzy.top/gtyglxxbwf.html

#define X_H
来源：http://hz.fengsongda.top/gtdrnyhcsa.html

#endif
来源：http://hz.gotoacloud.top/gtanipglkd.html

[S31] C++：Hello World
来源：http://hz.cashguo.top/gtvfsjqxzl.html

#include <iostream>
来源：http://hz.jinqigufen.top/gtfdpvdnhn.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yonumen.top/gtfzkbbvom.html

[S32] C++：字符串
来源：http://hz.nanxinkj.top/gtcfezyqod.html

std::string s = "hi";  s += "!";
来源：http://hz.jqgfzy.top/gtjtejlnss.html

[S33] C++：vector 增删
来源：http://hz.jianghu66.top/gtrvnzwwmg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shuidangran.top/gtiolrenmm.html

[S34] C++：遍历 vector
来源：http://hz.yueranfly.top/gtxnsgunfc.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.redwolf501.top/gtxgfaswvq.html

[S35] C++：map
来源：http://hz.iojbl.cn/gtcsswlvvs.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yanxiufei.cn/gtdvbbhxaq.html

[S36] C++：unordered_map
来源：http://hz.shangyingyoupin.top/gtpisemzgx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.aizwys.cn/gtosrzuypp.html

[S37] C++：set
来源：http://hz.daxiang520.top/gtapmohmov.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xinyue.icu/gteqstbbup.html

[S38] C++：排序
来源：http://hz.tanke756.top/gtntiagzsm.html

std::sort(v.begin(), v.end());
来源：http://hz.yonumen.top/gtqezewdnm.html

[S39] C++：自定义比较器排序
来源：http://hz.hnxiangtu.top/gtecyzwhpu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.feifeiyinyue.top/gtggbitgcx.html

[S40] C++：查找元素
来源：http://hz.sufxvd.cn/gtdophzqfu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yonumen.top/gttvrftqcf.html

[S41] C++：类与构造函数
来源：http://hz.shangyingyoupin.top/gtuxuchqkb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jlsjyb.cn/gtrxhtyjyg.html

[S42] C++：继承与虚函数
来源：http://hz.gzhubu.top/gtcsbmtsov.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhoulong.xyz/gtaitxwjxy.html

[S43] C++：智能指针
来源：http://hz.yueranfly.top/gtgisznlev.html

auto p = std::make_unique<int>(5);
来源：http://hz.bjfxy.top/gtgxkvpyjj.html

[S44] C++：引用传参
来源：http://hz.tianlin.xyz/gtezcpjsxm.html

void inc(int &x) { ++x; }
来源：http://hz.gogol.net.cn/gturiougdi.html

[S45] C++：lambda
来源：http://hz.yj20258888.top/gtlrmffcye.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.aizwys.cn/gtzvyulsdi.html

[S46] C++：函数模板
来源：http://hz.sufxvd.cn/gtsmpmtadb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jqgufenzy.top/gtddvwvdwz.html

[S47] C++：结构化绑定遍历
来源：http://hz.hnxiangtu.top/gtesbfhpli.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yj20258888.top/gtfrybkakb.html

[S48] C++：逐行读文件
来源：http://hz.tianlin.xyz/gtkcjmzhtb.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.tian-w.cn/gtzlillxhu.html

while (std::getline(in, line)) { }
来源：http://hz.yanxiufei.cn/gtlvbatngu.html

[S49] C++：写文件
来源：http://hz.nanxinkj.top/gtjdzbhltu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jinqigufen.top/gtamzgredv.html

[S50] C++：格式化数字
来源：http://hz.aizwys.cn/gtamnghpqb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.meibo888.top/gtzmnxtdza.html

[S51] C++：显式类型转换
来源：http://hz.jinghuilouyu.cn/gtcsbcjovl.html

static_cast<double>(a) / b
来源：http://hz.fengsongda.top/gtfkmssfkw.html

[S52] C++：const 与 noexcept
来源：http://hz.yuxming.cn/gtvludwnbl.html

int size() const noexcept { return n_; }
来源：http://hz.9152youxi.cn/gtnppfrupi.html

[S53] C++：移动语义
来源：http://hz.xuanzx.com/gtjkabwyvy.html

std::vector<int> w = std::move(v);
来源：http://hz.ivvv.top/gtujpmjypb.html

[S54] C++：异常处理
来源：http://hz.zhijiandao.cn/gtosuvvyro.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hammf.cn/gtfcughekj.html

[S55] C++：结构化绑定
来源：http://hz.svipenyu.cn/gtewjxmgdc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.fengsongda.top/gtdodyzemy.html

[S56] C++：optional
来源：http://hz.redwolf501.top/gtfrpmgdzv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.guannengcc.top/gtkfepnkcm.html

[S57] C++：编译期常量
来源：http://hz.nanxuanxn.top/gtkkoosgyh.html

constexpr int N = 10;
来源：http://hz.daria6918.cn/gtvuylueuz.html

[S58] C++：命名空间
来源：http://hz.cucudq.cn/gtwfqvapju.html

namespace ns { int f() { return 1; } }
来源：http://hz.daxiang520.top/gtnysyzrtu.html

[S59] C++：静态断言
来源：http://hz.gotoacloud.top/gtfitfbwxw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xylfe.cn/gtwdtbtgfb.html

[S60] C++：遍历并删除元素
来源：http://hz.hfpthk.cn/gtedqwdvxw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.sxryk.cn/gtykslcwzt.html

================================================================================
来源：http://hz.52xcode.cn/gtglnmyfpd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yj202588.top/gtwwgetiuz.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtwuxhbvkg.html

[T01] Kotlin：Hello World
来源：http://hz.haohaochexian.top/gtujzdooct.html

println("Hello")
来源：http://hz.quarkkingdee.top/gtjezrcrwl.html

[T02] Kotlin：变量
来源：http://hz.cheryme.top/gtidcjqtof.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.fengsongda.top/gtxxzuetah.html

[T03] Kotlin：字符串模板
来源：http://hz.hnxiangtu.top/gtpzalehnc.html

"值: $b"
来源：http://hz.yanxiufei.cn/gthmiagvvj.html

[T04] Kotlin：空安全
来源：http://hz.wangshuangyany.cn/gtqmjdpbtu.html

val n: String? = null;  n?.length
来源：http://hz.xziqi.cn/gtfddnihek.html

[T05] Kotlin：when 表达式
来源：http://hz.yangfankeji.com/gtjybjdsoc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.cqqwz.cn/gthbqpjtmm.html

[T06] Kotlin：集合映射
来源：http://hz.ehwqpu.com/gtkskmtpxd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.cdnleiting.top/gtydjbonbf.html

[T07] Kotlin：集合过滤
来源：http://hz.zhoulong.xyz/gtgyealuzd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yj20258.top/gtxxjfmqqs.html

[T08] Kotlin：数据类
来源：http://hz.zhijiandao.cn/gtvmcikevj.html

data class User(val name: String, val age: Int)
来源：http://hz.fengsongda.top/gtdgcmeqrn.html

[T09] Kotlin：扩展函数
来源：http://hz.zhijiandao.cn/gtafrleiqy.html

fun String.exclaim() = this + "!"
来源：http://hz.yuanzhike.top/gtsiyecdmu.html

[T10] Kotlin：默认参数
来源：http://hz.hnxiangtu.top/gtijeddvjc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.nwbrower.top/gtqtlxaepo.html

[T11] Kotlin：协程
来源：http://hz.zdqjudy.top/gtwzvghzxv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.cashguo.top/gtyiviacwn.html

[T12] Kotlin：解构声明
来源：http://hz.yvedp.cn/gtjizcgpmk.html

val (a, b) = Pair(1, 2)
来源：http://hz.shanyushiyangtech.top/gtmxealrnp.html

[T13] Kotlin：只读 Map
来源：http://hz.cqqwz.cn/gtihsxsmse.html

val m = mapOf("a" to 1)
来源：http://hz.yj20258888.top/gtfwsrqqvo.html

[T14] Kotlin：循环
来源：http://hz.shanyushiyangtech.top/gtospbwzal.html

for (i in 1..10) println(i)
来源：http://hz.jqgfzy.top/gtqthduscq.html

[T15] Kotlin：接口
来源：http://hz.pengpengdd.cyou/gtzjopzkdl.html

interface Shape { fun area(): Double }
来源：http://hz.bjfxy.top/gtzorfzrqc.html

[T16] Swift：Hello World
来源：http://hz.c1oappe.top/gttitzeolm.html

print("Hello")
来源：http://hz.svipenyu.cn/gtawtxiset.html

[T17] Swift：变量与常量
来源：http://hz.hongshengwenyu.top/gtjnsbejga.html

var a = 1;  let b = 2
来源：http://hz.yvedp.cn/gtpohextgz.html

[T18] Swift：字符串插值
来源：http://hz.cheryme.top/gtnlujhkqx.html

"值: \(b)"
来源：http://hz.hysaishi.cn/gtktpacttp.html

[T19] Swift：可选绑定
来源：http://hz.dianchejie.cn/gtpwgmdnhg.html

if let n = opt { print(n) }
来源：http://hz.hfpthk.cn/gtzsvrpvxs.html

[T20] Swift：数组操作
来源：http://hz.shuidangran.top/gtnwblfnwb.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.cheryme.top/gtoadaclvf.html

[T21] Swift：遍历
来源：http://hz.hnqzz.top/gtdimzgafc.html

for x in a { print(x) }
来源：http://hz.xziqi.cn/gtinkwqafl.html

[T22] Swift：字典
来源：http://hz.fzhhl.top/gtupkghfdk.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.gotoacloud.top/gthmzmxqhk.html

[T23] Swift：函数
来源：http://hz.yangfankeji.com/gtpfvjienj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jyoumei.cn/gtyqefusvi.html

[T24] Swift：闭包
来源：http://hz.xylfe.cn/gtgszegmhk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yuanzhike.top/gtcrijcqrx.html

[T25] Swift：结构体
来源：http://hz.quarkkingdee.top/gthfoxawcw.html

struct P { var x: Int }
来源：http://hz.shangyingyoupin.top/gtmplapokk.html

[T26] Swift：类与重写
来源：http://hz.zhaomingkeji.xyz/gtdcklnptu.html

class A: Base { override func f() {} }
来源：http://hz.havefunace.top/gtugbdfzmz.html

[T27] Swift：错误处理
来源：http://hz.andypj.xyz/gtbxuxcbmc.html

do { try f() } catch { print(error) }
来源：http://hz.yanxiufei.cn/gtihvhalre.html

[T28] Swift：枚举
来源：http://hz.quarkkingdee.top/gtemktqnxq.html

enum Color { case red, green }
来源：http://hz.jiagoushi.top/gtdkznxbdb.html

[T29] Swift：guard 提前返回
来源：http://hz.fzhhl.top/gtjxrmbciq.html

guard let x = opt else { return }
来源：http://hz.hammf.cn/gtobrlfpel.html

[T30] Swift：协议
来源：http://hz.chenzaomai.com/gtgfwqyctc.html

protocol Shape { func area() -> Double }
来源：http://hz.sweek.top/gthtyxmads.html

[T31] Lua：Hello World
来源：http://hz.nanxinkj.top/gtzvujvdyy.html

print("Hello")
来源：http://hz.ybcxt.top/gtlsslanfr.html

[T32] Lua：局部变量
来源：http://hz.9152youxi.cn/gtmvtbajdj.html

local a = 1
来源：http://hz.ydjk.org.cn/gtrcdyuond.html

[T33] Lua：表（数组）
来源：http://hz.yangfankeji.com/gtlwmsadyx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yanxiufei.cn/gtfrdbhbsd.html

[T34] Lua：遍历表
来源：http://hz.sxryk.cn/gtompkhdiy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.xziqi.cn/gtopqrrddg.html

[T35] Lua：字典表
来源：http://hz.nanxuanxn.top/gtrnpqodeo.html

local d = { a = 1 };  d.b = 2
来源：http://hz.xuetiantiany.cn/gtkstjgbvi.html

[T36] Lua：函数
来源：http://hz.gogol.net.cn/gttrztmizc.html

function add(a, b) return a + b end
来源：http://hz.jqgfzy.top/gtpspobfrq.html

[T37] Lua：字符串拼接
来源：http://hz.smart0.xyz/gthffxpyxb.html

"a" .. "b"
来源：http://hz.aizwys.cn/gthktghqrw.html

[T38] Lua：条件
来源：http://hz.meibo888.top/gtikirrxdd.html

if x > 0 then print("正") end
来源：http://hz.shangyingyoupin.top/gtrrcvlpdv.html

[T39] Lua：模式匹配
来源：http://hz.316326.xyz/gtlmoqxskn.html

string.find(s, "%d+")
来源：http://hz.cashguo.top/gtmveyewjj.html

[T40] Lua：元表
来源：http://hz.snrcjt.cn/gtksbkgcwo.html

setmetatable({}, { __index = base })
来源：http://hz.yuanzhike.top/gtzbzpuqgs.html

[T41] Perl：Hello World
来源：http://hz.daxiang520.top/gtekktrpbm.html

print "Hello\n";
来源：http://hz.jinqigfzy.top/gttzebqfxs.html

[T42] Perl：变量类型
来源：http://hz.kuanghao11.cn/gthyoyrhen.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.xingfuxueyuan.xyz/gtsawedkka.html

[T43] Perl：字符串插值
来源：http://hz.yvedp.cn/gtjzmyocmu.html

"值: $a"
来源：http://hz.zhaomingkeji.xyz/gtejuohcgs.html

[T44] Perl：条件
来源：http://hz.nanxinkj.top/gtvkyghfzv.html

if ($a > 0) { print "正"; }
来源：http://hz.guannengcc.top/gtbufbvyyg.html

[T45] Perl：数组遍历
来源：http://hz.iojbl.cn/gtekyuvryf.html

for my $x (@arr) { print $x; }
来源：http://hz.tian-w.cn/gtkhmnofmo.html

[T46] Perl：哈希操作
来源：http://hz.jinqigufen.top/gtnwlajaok.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.fengsongda.top/gteibeduqj.html

[T47] Perl：正则捕获
来源：http://hz.aibaodan.cn/gtueroyhfs.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.shanyushiyangtech.top/gtvgjapipw.html

[T48] Perl：正则替换
来源：http://hz.smart0.xyz/gttqnijxrn.html

$s =~ s/old/new/g;
来源：http://hz.sweek.top/gtjhoacikm.html

[T49] Perl：函数
来源：http://hz.ppjwa.cn/gtybakgjas.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yangfankeji.com/gtaaquswqa.html

[T50] Perl：逐行读文件
来源：http://hz.9152youxi.cn/gtlqjofpnv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.hfpthk.cn/gteaokagtn.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.andypj.xyz/gtyocykbbt.html

[T51] Scala：Hello World
来源：http://hz.haohaochexian.top/gtntasvfjn.html

println("Hello")
来源：http://hz.cdnleiting.top/gtnzfcvhoz.html

[T52] Scala：变量
来源：http://hz.wangshuangyany.cn/gtgxdlorgo.html

val a = 1;  var b = 2
来源：http://hz.zycfv.cn/gtisjgwlnx.html

[T53] Scala：字符串插值
来源：http://hz.shuidangran.top/gthczrjkdz.html

s"值: $b"
来源：http://hz.nanxuanxn.top/gtwpiupmez.html

[T54] Scala：集合映射
来源：http://hz.jqgufenzy.top/gtipgokusx.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yj20258.top/gttsvxukob.html

[T55] Scala：集合过滤
来源：http://hz.gzhubu.top/gtkkaanker.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.yj20258888.top/gtjaadjckj.html

[T56] Scala：样例类
来源：http://hz.hongshengwenyu.top/gtjqauownm.html

case class User(name: String, age: Int)
来源：http://hz.yuanzhike.top/gtmekcjycb.html

[T57] Scala：模式匹配
来源：http://hz.jiagoushi.top/gtzawwcxnl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.aibaodan.cn/gtrauvwnus.html

[T58] Scala：函数定义
来源：http://hz.jinqigufen.top/gtgfykkgpd.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.sufxvd.cn/gttkpalhxf.html

[T59] Scala：循环
来源：http://hz.ivvv.top/gthmhpingu.html

for (i <- 1 to 10) println(i)
来源：http://hz.9152youxi.cn/gtdkcifyar.html

[T60] Scala：折叠
来源：http://hz.iojbl.cn/gttnxubdzi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.andypj.xyz/gtpblypqjm.html

================================================================================
来源：http://hz.tian-w.cn/gtcgqwdmrn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.fzhhl.top/gtgxajkawl.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtinpdtwlu.html

[U01] Py：创建虚拟环境
来源：http://hz.guowangkeji.top/gtxtjlvckb.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.smart0.xyz/gtymkdpzrm.html

[U02] Py：导出 / 安装依赖
来源：http://hz.316326.xyz/gterpwaivz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.hongshengwenyu.top/gtjpwxuewp.html

[U03] Py：加载 .env 配置
来源：http://hz.yvedp.cn/gtockmifog.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.quarkkingdee.top/gtgndydajq.html

[U04] Py：变量调试打印
来源：http://hz.yongpay.top/gtdzbnoddg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yonumen.top/gtunwnubnd.html

[U05] Py：列表去重且保序
来源：http://hz.aizwys.cn/gtwzxpzazb.html

list(dict.fromkeys(arr))
来源：http://hz.havefunace.top/gtaevmydyt.html

[U06] Py：合并两个字典
来源：http://hz.xuanzx.com/gtyuaqinyq.html

{**a, **b}
来源：http://hz.chenzaomai.com/gtniosgtdo.html

[U07] Py：反转字典键值
来源：http://hz.zhijiandao.cn/gtudhcwhex.html

{v: k for k, v in d.items()}
来源：http://hz.wangshuangyany.cn/gttnaqswdv.html

[U08] Py：展平二维列表
来源：http://hz.chenzaomai.com/gttdqxbrjb.html

[y for x in nested for y in x]
来源：http://hz.birdmap.top/gtzjhuqtul.html

[U09] Py：字典取最大值的键
来源：http://hz.316326.xyz/gtxnukoqqg.html

max(d, key=d.get)
来源：http://hz.hywenlv.cn/gtstxhlero.html

[U10] Py：按值排序字典
来源：http://hz.svipenyu.cn/gtgmqhajjd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.chenzaomai.com/gtuvwevrvb.html

[U11] Py：生成器表达式
来源：http://hz.hfpthk.cn/gtatcihext.html

(x * 2 for x in arr)
来源：http://hz.aizwys.cn/gtmmtgasxs.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.gogol.net.cn/gtijozavlo.html

Counter(arr).most_common(3)
来源：http://hz.ppjwa.cn/gtsowcxtug.html

[U13] Py：固定长度队列
来源：http://hz.meibo888.top/gtpmimkupf.html

deque(maxlen=10)
来源：http://hz.daxiang520.top/gtmzvjejor.html

[U14] Py：分组收集到列表
来源：http://hz.c1oappe.top/gtolfuvsgl.html

defaultdict(list)
来源：http://hz.shanyushiyangkeji.top/gtxgjstbpk.html

[U15] Py：高精度计时
来源：http://hz.xuanzx.com/gtnllaerfm.html

t = time.perf_counter()
来源：http://hz.bjfxy.top/gtkskyvbdz.html

[U16] Py：命令行参数解析
来源：http://hz.chenlongwang.top/gtjdlydhwa.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.sysykeji.top/gteqwyinxo.html

[U17] Py：初始化日志
来源：http://hz.jinyuanbaomall.cn/gtbptufwbo.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.chenlongwang.top/gtgotwjmje.html

[U18] Py：预编译正则
来源：http://hz.hysaishi.cn/gtrsmaxtbf.html

pat = re.compile(r"\d+")
来源：http://hz.ivvv.top/gtmfsywugk.html

[U19] Py：正则替换带回调
来源：http://hz.guowangkeji.top/gtcarmuepd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.9152youxi.cn/gtujnoloda.html

[U20] Py：缓存函数结果
来源：http://hz.smart0.xyz/gtumbfeebe.html

@functools.lru_cache(maxsize=None)
来源：http://hz.ydzc1.top/gtekvkgccm.html

[U21] Py：自定义上下文管理器
来源：http://hz.ivvv.top/gtebzvxehq.html

@contextlib.contextmanager
来源：http://hz.c1oappe.top/gtglkfqynh.html

[U22] Py：矩阵转置
来源：http://hz.zhengqikj.top/gtehaxopqz.html

list(zip(*m))
来源：http://hz.jinqigfzy.top/gtrsmaxypn.html

[U23] Py：分块读取大文件
来源：http://hz.xuetiantiany.cn/gtqtqlvwor.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.shzxlz.cn/gtmzwrrcso.html

[U24] Py：路径操作
来源：http://hz.tian-w.cn/gtglokqxsn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.zhongyouzk.top/gttghtuxjq.html

[U25] Py：CSV 按字典读
来源：http://hz.iojbl.cn/gtbmkwoxya.html

csv.DictReader(f)
来源：http://hz.xylfe.cn/gtgqyhzcgg.html

[U26] Py：并发下载
来源：http://hz.jiagoushi.top/gtsmkxsxjg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.ppjwa.cn/gtfygzefyl.html


<!-- 参考信息 -->