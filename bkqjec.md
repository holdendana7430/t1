代发 wailian999

int x; scanf("%d", &x);
来源：http://hz.0kj1m.cn/gtxqnsozje.html

[S04] C：字符串复制
来源：http://hz.zhengqikj.top/gtmamnnitf.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.snrcjt.cn/gtilnghtty.html

[S05] C：字符串长度
来源：http://hz.pycfn.com/gtpilxhmrs.html

strlen(s)
来源：http://hz.zhiwuduotai.top/gtzoawytce.html

[S06] C：字符串比较
来源：http://hz.yongpay.top/gtgnqvlenz.html

strcmp(a, b) == 0
来源：http://hz.zhixingplan.top/gtmmmjlolj.html

[S07] C：数组遍历求和
来源：http://hz.jqgfzy.top/gtipfipvqu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jyoumei.cn/gtkogpusho.html

[S08] C：动态内存分配与释放
来源：http://hz.nanxinkj.top/gtcfcgmkdo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ivvv.top/gtmyicpywn.html

[S09] C：结构体定义与初始化
来源：http://hz.nwbrower.top/gthysilzwn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.guowangkeji.top/gtflgbfxko.html

[S10] C：指针与解引用
来源：http://hz.cashguo.top/gtrdeydlhe.html

int *p = &a;  *p = 5;
来源：http://hz.jinqigufen.top/gttizcsgbk.html

[S11] C：逐行读文件
来源：http://hz.jinyuanbaomall.cn/gtpkdatucl.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.xylfe.cn/gtbfatcouc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.sxryk.cn/gtpkobfyfa.html

fclose(f);
来源：http://hz.feifeiyinyue.top/gtrgoeqhiq.html

[S12] C：写文件
来源：http://hz.xylfe.cn/gtegwpnsch.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yuxming.cn/gtzqcyuyhx.html

[S13] C：宏定义
来源：http://hz.zhoulong.xyz/gtkkwwesjg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.shangyingyoupin.top/gtxwdxwmji.html

[S14] C：枚举
来源：http://hz.jyoumei.cn/gtttudqgwl.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.0kj1m.cn/gttxvbqwbj.html

[S15] C：类型转换
来源：http://hz.jlsjyb.cn/gtmifmdxzr.html

(double) a / b
来源：http://hz.meibo888.top/gtwqnltgad.html

[S16] C：位操作置位
来源：http://hz.zycfv.cn/gttxxrdzek.html

x |= (1 << 3);
来源：http://hz.shanyushiyangtech.top/gtkwjkqvsp.html

[S17] C：安全拼接字符串
来源：http://hz.chenlongwang.top/gtpcutjwws.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.havefunace.top/gtgkqxwcsa.html

[S18] C：命令行参数
来源：http://hz.yongpay.top/gthfzudipc.html

int main(int argc, char **argv)
来源：http://hz.yangfankeji.com/gttpnfpgfx.html

[S19] C：快速排序
来源：http://hz.zdqjudy.top/gtirlggpka.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yvedp.cn/gtghruvobd.html

[S20] C：二分查找
来源：http://hz.ydjk.org.cn/gtkrvozsfx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.dianchejie.cn/gtutpepdzc.html

[S21] C：字符类别判断
来源：http://hz.bjfxy.top/gtctkaaxja.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.gogol.net.cn/gtgsdtymyr.html

[S22] C：字符串转数字
来源：http://hz.hnxiangtu.top/gtygwogwpg.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.andypj.xyz/gtftjtbwyg.html

[S23] C：随机数
来源：http://hz.cucudq.cn/gtcgoglyjf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.wangdashe.top/gtxmmspunn.html

[S24] C：获取本地时间
来源：http://hz.mhx1999.top/gtztofpqqe.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.pycfn.com/gtnvmzsmtw.html

[S25] C：内存拷贝
来源：http://hz.jqgufenzy.top/gtcaebcynt.html

memcpy(dst, src, n);
来源：http://hz.gaohongyu789.top/gtczjcqrvy.html

[S26] C：内存清零
来源：http://hz.hongshengwenyu.top/gtufohtukm.html

memset(a, 0, sizeof a);
来源：http://hz.bjfxy.top/gtfjbfmytg.html

[S27] C：定义常量
来源：http://hz.xinyue.icu/gtbnpcaxxj.html

const double PI = 3.14159;
来源：http://hz.yuanzhike.top/gtfworbpex.html

[S28] C：静态变量
来源：http://hz.chenzaomai.com/gttczaqhzp.html

static int counter = 0;
来源：http://hz.chenlongwang.top/gtrufbznfu.html

[S29] C：变参函数
来源：http://hz.ppjwa.cn/gtrojyfubx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.xziqi.cn/gtuvuorlix.html

[S30] C：头文件保护
来源：http://hz.xuetiantiany.cn/gtobrdtkhb.html

#ifndef X_H
来源：http://hz.tianlin.xyz/gtqstswqur.html

#define X_H
来源：http://hz.yvedp.cn/gtsefnebsi.html

#endif
来源：http://hz.hnxiangtu.top/gtjtqfpupx.html

[S31] C++：Hello World
来源：http://hz.nanxinkj.top/gtsitfqdhm.html

#include <iostream>
来源：http://hz.haohaochexian.top/gtulwandyn.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.redwolf501.top/gtepefvsyl.html

[S32] C++：字符串
来源：http://hz.bjfxy.top/gtmcwpnwfj.html

std::string s = "hi";  s += "!";
来源：http://hz.hongshengwenyu.top/gtbkavmnga.html

[S33] C++：vector 增删
来源：http://hz.shangyingyoupin.top/gtmjzzghin.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jyoumei.cn/gtbvapmepg.html

[S34] C++：遍历 vector
来源：http://hz.hnqzz.top/gtibugdaih.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.andypj.xyz/gtanhnzepb.html

[S35] C++：map
来源：http://hz.9152youxi.cn/gtjudtvcrf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.dianchejie.cn/gtrwclioxw.html

[S36] C++：unordered_map
来源：http://hz.tanke756.top/gtjcdqnsko.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hnqzz.top/gtwdttrmsm.html

[S37] C++：set
来源：http://hz.dashuyun.cn/gtknadyrrx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.havefunace.top/gthsybnptn.html

[S38] C++：排序
来源：http://hz.wangshuangyany.cn/gtjwymapbh.html

std::sort(v.begin(), v.end());
来源：http://hz.tianlin.xyz/gtqiynugwy.html

[S39] C++：自定义比较器排序
来源：http://hz.shuidangran.top/gtcwajhedw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jianghu66.top/gtxkvzjhdq.html

[S40] C++：查找元素
来源：http://hz.kuanghao11.cn/gtrmflowsn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jianghu66.top/gtqqxghgvj.html

[S41] C++：类与构造函数
来源：http://hz.ivvv.top/gtowqanjoy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.quarkkingdee.top/gtwrpnpgnn.html

[S42] C++：继承与虚函数
来源：http://hz.ydjk.org.cn/gtbkwernpr.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhaomingkeji.xyz/gtqqwexzru.html

[S43] C++：智能指针
来源：http://hz.kuanghao11.cn/gtosbgmkgi.html

auto p = std::make_unique<int>(5);
来源：http://hz.guowangkeji.top/gtrrtqwyva.html

[S44] C++：引用传参
来源：http://hz.c1oappe.top/gtlqeqrxom.html

void inc(int &x) { ++x; }
来源：http://hz.jinghuilouyu.cn/gtktymsxht.html

[S45] C++：lambda
来源：http://hz.snrcjt.cn/gtvoanrqdn.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jyoumei.cn/gtgjyxvliy.html

[S46] C++：函数模板
来源：http://hz.hywenlv.cn/gtdybduuwm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zycfv.cn/gtobymlwgo.html

[S47] C++：结构化绑定遍历
来源：http://hz.yj20258888.top/gtjgcbbppw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.hfpthk.cn/gtuthsgzog.html

[S48] C++：逐行读文件
来源：http://hz.xylfe.cn/gtojkqlqlx.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.nanxinkj.top/gtokriqvid.html

while (std::getline(in, line)) { }
来源：http://hz.wangdashe.top/gtwsndtbkt.html

[S49] C++：写文件
来源：http://hz.aibaodan.cn/gtlshasngd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.iojbl.cn/gtneakjlrg.html

[S50] C++：格式化数字
来源：http://hz.xuetiantiany.cn/gtokkrdend.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.sxryk.cn/gtdadoplmj.html

[S51] C++：显式类型转换
来源：http://hz.snrcjt.cn/gtpuckjxbm.html

static_cast<double>(a) / b
来源：http://hz.xingfuxueyuan.xyz/gtsugotgbv.html

[S52] C++：const 与 noexcept
来源：http://hz.daxiang520.top/gtpegusbkz.html

int size() const noexcept { return n_; }
来源：http://hz.xziqi.cn/gtrttfsxvt.html

[S53] C++：移动语义
来源：http://hz.pycfn.com/gtdwjzyokc.html

std::vector<int> w = std::move(v);
来源：http://hz.cqqwz.cn/gtbvhiwcex.html

[S54] C++：异常处理
来源：http://hz.guowangkeji.top/gthgvbnxbc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.0kj1m.cn/gthktabpko.html

[S55] C++：结构化绑定
来源：http://hz.shangyingyoupin.top/gtpznkjkll.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.birdmap.top/gtldsrcare.html

[S56] C++：optional
来源：http://hz.bjfxy.top/gtqyvwunrg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hfpthk.cn/gtetsjydho.html

[S57] C++：编译期常量
来源：http://hz.smart0.xyz/gtdkptucfq.html

constexpr int N = 10;
来源：http://hz.xingfuxueyuan.xyz/gtcmdrhstj.html

[S58] C++：命名空间
来源：http://hz.zdqjudy.top/gtqgwxochl.html

namespace ns { int f() { return 1; } }
来源：http://hz.gzhubu.top/gtehuqqbys.html

[S59] C++：静态断言
来源：http://hz.52xcode.cn/gtvohfcnab.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.daxiang520.top/gtcgiuouri.html

[S60] C++：遍历并删除元素
来源：http://hz.fengsongda.top/gtjotneval.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hammf.cn/gtrjmluhzi.html

================================================================================
来源：http://hz.hnxiangtu.top/gthylsopsf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.birdmap.top/gtokznscpq.html

================================================================================
来源：http://hz.gogol.net.cn/gtrmtdeths.html

[T01] Kotlin：Hello World
来源：http://hz.jinghuilouyu.cn/gtagjkbhbf.html

println("Hello")
来源：http://hz.cdnleiting.top/gtabrakoax.html

[T02] Kotlin：变量
来源：http://hz.birdmap.top/gtsmhivmnf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.ydzc1.top/gtdpnwseew.html

[T03] Kotlin：字符串模板
来源：http://hz.jianghu66.top/gtxuppvmte.html

"值: $b"
来源：http://hz.meibo888.top/gtamnxkrhw.html

[T04] Kotlin：空安全
来源：http://hz.tian-w.cn/gtauokcwzj.html

val n: String? = null;  n?.length
来源：http://hz.kuanghao11.cn/gtdapjhmqx.html

[T05] Kotlin：when 表达式
来源：http://hz.ydzc1.top/gtiqgfeeyv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.9152youxi.cn/gtdzcgbrjv.html

[T06] Kotlin：集合映射
来源：http://hz.mhx1999.top/gtcglggvqy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhengqikj.top/gtbpvlzjoe.html

[T07] Kotlin：集合过滤
来源：http://hz.hnqzz.top/gtwkkuvmuh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hywenlv.cn/gtkrlgvorq.html

[T08] Kotlin：数据类
来源：http://hz.nwbrower.top/gtpsqpefej.html

data class User(val name: String, val age: Int)
来源：http://hz.vqdsnc.cn/gtbfxuimnd.html

[T09] Kotlin：扩展函数
来源：http://hz.zhixingplan.top/gthjrmapzo.html

fun String.exclaim() = this + "!"
来源：http://hz.52xcode.cn/gtqpvfbjog.html

[T10] Kotlin：默认参数
来源：http://hz.mhx1999.top/gtftuqghef.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.shzxlz.cn/gtqsbrfsoi.html

[T11] Kotlin：协程
来源：http://hz.shangyingyoupin.top/gtiidbxcfg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zhongyouzk.top/gtvhezlxpq.html

[T12] Kotlin：解构声明
来源：http://hz.sxryk.cn/gtqmwfiljb.html

val (a, b) = Pair(1, 2)
来源：http://hz.ybcxt.top/gtordqjvhc.html

[T13] Kotlin：只读 Map
来源：http://hz.zhoulong.xyz/gtyumtiqnu.html

val m = mapOf("a" to 1)
来源：http://hz.hongshengwenyu.top/gttiujmcha.html

[T14] Kotlin：循环
来源：http://hz.kuanghao11.cn/gtkowqcvnv.html

for (i in 1..10) println(i)
来源：http://hz.jqgfzy.top/gtqrxiwxmk.html

[T15] Kotlin：接口
来源：http://hz.aizwys.cn/gtabuoiozr.html

interface Shape { fun area(): Double }
来源：http://hz.tanke756.top/gtbjoncuuf.html

[T16] Swift：Hello World
来源：http://hz.kuanghao11.cn/gtmscsjxsi.html

print("Hello")
来源：http://hz.yvedp.cn/gtydwggilz.html

[T17] Swift：变量与常量
来源：http://hz.yuxming.cn/gtxhpetmkg.html

var a = 1;  let b = 2
来源：http://hz.shangyingyoupin.top/gtvhajobxm.html

[T18] Swift：字符串插值
来源：http://hz.xingfuxueyuan.xyz/gtzscznsjz.html

"值: \(b)"
来源：http://hz.wangdashe.top/gtmicldxbb.html

[T19] Swift：可选绑定
来源：http://hz.ivvv.top/gtyufpynvw.html

if let n = opt { print(n) }
来源：http://hz.hfpthk.cn/gtmqoautxb.html

[T20] Swift：数组操作
来源：http://hz.yj20258.top/gthhprsvlz.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jinyuanbaomall.cn/gtotpstcku.html

[T21] Swift：遍历
来源：http://hz.hongshengwenyu.top/gtvzatqmmu.html

for x in a { print(x) }
来源：http://hz.chenlongwang.top/gtiuvfevce.html

[T22] Swift：字典
来源：http://hz.svipenyu.cn/gttqzdhoce.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.wangdashe.top/gtdusfmqec.html

[T23] Swift：函数
来源：http://hz.dashuyun.cn/gtpmsdmsyh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.aizwys.cn/gtoxyrhjwf.html

[T24] Swift：闭包
来源：http://hz.bjfxy.top/gtfihtzerc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.sweek.top/gtvrikayvv.html

[T25] Swift：结构体
来源：http://hz.hnxiangtu.top/gtspvetuiy.html

struct P { var x: Int }
来源：http://hz.nwbrower.top/gtugwxirtr.html

[T26] Swift：类与重写
来源：http://hz.xylfe.cn/gtlxziylkm.html

class A: Base { override func f() {} }
来源：http://hz.yvedp.cn/gttgfdzfpr.html

[T27] Swift：错误处理
来源：http://hz.sxryk.cn/gtchxskwxt.html

do { try f() } catch { print(error) }
来源：http://hz.guowangkeji.top/gthlqhedjq.html

[T28] Swift：枚举
来源：http://hz.jqgufenzy.top/gtixebdqfr.html

enum Color { case red, green }
来源：http://hz.dashuyun.cn/gtvqfligmr.html

[T29] Swift：guard 提前返回
来源：http://hz.hammf.cn/gtpzxdknma.html

guard let x = opt else { return }
来源：http://hz.shuidangran.top/gtwmupquxr.html

[T30] Swift：协议
来源：http://hz.jyoumei.cn/gtwmcsrhxn.html

protocol Shape { func area() -> Double }
来源：http://hz.sweek.top/gtwylvxjkf.html

[T31] Lua：Hello World
来源：http://hz.jinghuilouyu.cn/gtbukkhxjm.html

print("Hello")
来源：http://hz.xuetiantiany.cn/gtfdhmjita.html

[T32] Lua：局部变量
来源：http://hz.cheryme.top/gtcidconrs.html

local a = 1
来源：http://hz.nwbrower.top/gtrnpzgyzx.html

[T33] Lua：表（数组）
来源：http://hz.yvedp.cn/gturxutxpa.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.wangdashe.top/gtymlaysqv.html

[T34] Lua：遍历表
来源：http://hz.shuidangran.top/gtnnxjjhcr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.tanke756.top/gtidpxfqws.html

[T35] Lua：字典表
来源：http://hz.yanxiufei.cn/gtiecpyasa.html

local d = { a = 1 };  d.b = 2
来源：http://hz.gogol.net.cn/gttljkqvkm.html

[T36] Lua：函数
来源：http://hz.pengpengdd.cyou/gtbfehoqye.html

function add(a, b) return a + b end
来源：http://hz.xziqi.cn/gtcyfrglqn.html

[T37] Lua：字符串拼接
来源：http://hz.zhongyouzk.top/gtzfwjxvgl.html

"a" .. "b"
来源：http://hz.fengsongda.top/gtyxnoakzr.html

[T38] Lua：条件
来源：http://hz.vqdsnc.cn/gtgzgtlhem.html

if x > 0 then print("正") end
来源：http://hz.xuetiantiany.cn/gtielodadl.html

[T39] Lua：模式匹配
来源：http://hz.yuanzhike.top/gtqovxlurn.html

string.find(s, "%d+")
来源：http://hz.jinqigufen.top/gtgvbmtwao.html

[T40] Lua：元表
来源：http://hz.cdnleiting.top/gtebcmmgpa.html

setmetatable({}, { __index = base })
来源：http://hz.cdnleiting.top/gtxonjwhqs.html

[T41] Perl：Hello World
来源：http://hz.jlsjyb.cn/gtndkfgsbq.html

print "Hello\n";
来源：http://hz.xuetiantiany.cn/gtbyafhfyf.html

[T42] Perl：变量类型
来源：http://hz.yuxming.cn/gthxhwtlyg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.sysykeji.top/gtmgujwflr.html

[T43] Perl：字符串插值
来源：http://hz.yangfankeji.com/gttiduwdcd.html

"值: $a"
来源：http://hz.yj20258888.top/gtrlxmnfnu.html

[T44] Perl：条件
来源：http://hz.yanxiufei.cn/gtilhanuja.html

if ($a > 0) { print "正"; }
来源：http://hz.ybcxt.top/gtzsmmxrzb.html

[T45] Perl：数组遍历
来源：http://hz.shanyushiyangtech.top/gtrkgmemmb.html

for my $x (@arr) { print $x; }
来源：http://hz.yj20258888.top/gtbgnyigvu.html

[T46] Perl：哈希操作
来源：http://hz.guowangkeji.top/gtjbevjyhp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.fzhhl.top/gtidbrvqcx.html

[T47] Perl：正则捕获
来源：http://hz.zhiwuduotai.top/gtpvgtplgd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yanxiufei.cn/gtwjkvohfx.html

[T48] Perl：正则替换
来源：http://hz.sufxvd.cn/gtkihyznng.html

$s =~ s/old/new/g;
来源：http://hz.yuxming.cn/gtuaxmadnn.html

[T49] Perl：函数
来源：http://hz.hysaishi.cn/gtbgeyonvj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.wangshuangyany.cn/gtruvdlyto.html

[T50] Perl：逐行读文件
来源：http://hz.ydzc1.top/gtdfborxvs.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jinyuanbaomall.cn/gtxmyarqyz.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.gogol.net.cn/gtsypmcdfg.html

[T51] Scala：Hello World
来源：http://hz.jinqigufen.top/gtysrenaro.html

println("Hello")
来源：http://hz.nanxinkj.top/gtljrnwpyn.html

[T52] Scala：变量
来源：http://hz.sufxvd.cn/gtzdngcpxp.html

val a = 1;  var b = 2
来源：http://hz.feifeiyinyue.top/gtulyxijsp.html

[T53] Scala：字符串插值
来源：http://hz.pengpengdd.cyou/gtivbjdwsw.html

s"值: $b"
来源：http://hz.zycfv.cn/gtnmofugdj.html

[T54] Scala：集合映射
来源：http://hz.ydjk.org.cn/gtjzweupnn.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.shzxlz.cn/gtfgibdofs.html

[T55] Scala：集合过滤
来源：http://hz.jlsjyb.cn/gtnjxxylro.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.yj20258888.top/gtsuxwyjcb.html

[T56] Scala：样例类
来源：http://hz.jianghu66.top/gtcopilinq.html

case class User(name: String, age: Int)
来源：http://hz.chenjidiqi.icu/gtrsbdhgfh.html

[T57] Scala：模式匹配
来源：http://hz.cucudq.cn/gtfdvbotuc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.cheryme.top/gtjlrsygoj.html

[T58] Scala：函数定义
来源：http://hz.ivvv.top/gtoxrycxbt.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.tanke756.top/gtbqqwpuuc.html

[T59] Scala：循环
来源：http://hz.daxiang520.top/gtqsayoweu.html

for (i <- 1 to 10) println(i)
来源：http://hz.cucudq.cn/gtagueqrmd.html

[T60] Scala：折叠
来源：http://hz.snrcjt.cn/gtvmuxmgqf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.havefunace.top/gtjfzrvbeq.html

================================================================================
来源：http://hz.mhx1999.top/gtlevuvzlw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.shuidangran.top/gtvpsvjsyt.html

================================================================================
来源：http://hz.zhoulong.xyz/gtugtgrfez.html

[U01] Py：创建虚拟环境
来源：http://hz.zhengqikj.top/gtoqlpqjgy.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.fengsongda.top/gtuxwxiozt.html

[U02] Py：导出 / 安装依赖
来源：http://hz.chenjidiqi.icu/gtdrfgktja.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jinyuanbaomall.cn/gtfxujvocg.html

[U03] Py：加载 .env 配置
来源：http://hz.shuidangran.top/gthumoihll.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.sysykeji.top/gtjejikaut.html

[U04] Py：变量调试打印
来源：http://hz.chenzaomai.com/gtghiktrkp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.gaohongyu789.top/gtswcpzhtq.html

[U05] Py：列表去重且保序
来源：http://hz.jinyuanbaomall.cn/gtlybhlzpw.html

list(dict.fromkeys(arr))
来源：http://hz.zdqjudy.top/gtlqxfpwcx.html

[U06] Py：合并两个字典
来源：http://hz.cqqwz.cn/gteiepvkhf.html

{**a, **b}
来源：http://hz.bjfxy.top/gtimkurrat.html

[U07] Py：反转字典键值
来源：http://hz.cucudq.cn/gtyklvyzlg.html

{v: k for k, v in d.items()}
来源：http://hz.tanke756.top/gthugrcmts.html

[U08] Py：展平二维列表
来源：http://hz.cheryme.top/gtvrylholr.html

[y for x in nested for y in x]
来源：http://hz.chenjidiqi.icu/gtbskyghti.html

[U09] Py：字典取最大值的键
来源：http://hz.zhijiandao.cn/gtjvckbnec.html

max(d, key=d.get)
来源：http://hz.jinqigfzy.top/gtdehqphfw.html

[U10] Py：按值排序字典
来源：http://hz.mhx1999.top/gtuwcraimk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.bjfxy.top/gtgltqszbs.html

[U11] Py：生成器表达式
来源：http://hz.jianghu66.top/gtxxjkypky.html

(x * 2 for x in arr)
来源：http://hz.mhx1999.top/gtcejozmaf.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.cheryme.top/gtwphvupgf.html

Counter(arr).most_common(3)
来源：http://hz.sysykeji.top/gtsxmhuwtp.html

[U13] Py：固定长度队列
来源：http://hz.havefunace.top/gtkpduxrxb.html

deque(maxlen=10)
来源：http://hz.9152youxi.cn/gtzjzyvzcq.html

[U14] Py：分组收集到列表
来源：http://hz.yongpay.top/gtxrjwujtm.html

defaultdict(list)
来源：http://hz.52xcode.cn/gtzzdfpnie.html

[U15] Py：高精度计时
来源：http://hz.yj20258888.top/gtjqblxksa.html

t = time.perf_counter()
来源：http://hz.snrcjt.cn/gtyrtmzyoc.html

[U16] Py：命令行参数解析
来源：http://hz.hammf.cn/gtbbypwlck.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.ydjk.org.cn/gtpeuoxjwj.html

[U17] Py：初始化日志
来源：http://hz.jiagoushi.top/gtohuuiizm.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.chenjidiqi.icu/gtczkiumis.html

[U18] Py：预编译正则
来源：http://hz.bjfxy.top/gtfmkgfjts.html

pat = re.compile(r"\d+")
来源：http://hz.jqgfzy.top/gtpkkxamrc.html

[U19] Py：正则替换带回调
来源：http://hz.yonumen.top/gtdgefybqh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.zhijiandao.cn/gtxeenjcie.html

[U20] Py：缓存函数结果
来源：http://hz.jqgufenzy.top/gtnvlpndzh.html

@functools.lru_cache(maxsize=None)
来源：http://hz.ybcxt.top/gtoxceksrd.html

[U21] Py：自定义上下文管理器
来源：http://hz.shzxlz.cn/gtgxhemmci.html

@contextlib.contextmanager
来源：http://hz.redwolf501.top/gtzokmlnoj.html

[U22] Py：矩阵转置
来源：http://hz.sxryk.cn/gtwmuvchkj.html

list(zip(*m))
来源：http://hz.kuanghao11.cn/gtkszuqwhs.html

[U23] Py：分块读取大文件
来源：http://hz.yj202588.top/gtvtymdipt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.aizwys.cn/gtwnnurdjj.html

[U24] Py：路径操作
来源：http://hz.316326.xyz/gtkewkngjy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.yj20258888.top/gttijpkrsp.html

[U25] Py：CSV 按字典读
来源：http://hz.haohaochexian.top/gtzpbcakyt.html

csv.DictReader(f)
来源：http://hz.fzhhl.top/gtbfpugtng.html

[U26] Py：并发下载
来源：http://hz.hywenlv.cn/gtuyfbbkiu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.zdqjudy.top/gtwjtwvygx.html


<!-- 参考信息 -->