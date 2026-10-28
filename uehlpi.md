代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.sysykeji.top/gtvxlmutao.html

[S02] C：变量与格式化输出
来源：http://hz.shuidangran.top/gtlvcbfoyj.html

int a = 10; printf("%d\n", a);
来源：http://hz.daria6918.cn/gtrygwulvz.html

[S03] C：读入整数
来源：http://hz.wangdashe.top/gtquisxaoy.html

int x; scanf("%d", &x);
来源：http://hz.xziqi.cn/gtnpjquiqp.html

[S04] C：字符串复制
来源：http://hz.nanxinkj.top/gtcwdjjuif.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhiwuduotai.top/gthvbnjtuo.html

[S05] C：字符串长度
来源：http://hz.vqdsnc.cn/gtlaipgswx.html

strlen(s)
来源：http://hz.cashguo.top/gtjuqyqpgb.html

[S06] C：字符串比较
来源：http://hz.bjfxy.top/gtrurrxrlk.html

strcmp(a, b) == 0
来源：http://hz.smart0.xyz/gtkfpbaabk.html

[S07] C：数组遍历求和
来源：http://hz.xylfe.cn/gttdcdlfep.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.andypj.xyz/gtdpdhnwzy.html

[S08] C：动态内存分配与释放
来源：http://hz.dashuyun.cn/gtnfnkykgr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.aizwys.cn/gtqbbirwzy.html

[S09] C：结构体定义与初始化
来源：http://hz.bjfxy.top/gtkmyuvyaj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.chenlongwang.top/gtijgrsejq.html

[S10] C：指针与解引用
来源：http://hz.dianchejie.cn/gttfplqggd.html

int *p = &a;  *p = 5;
来源：http://hz.haohaochexian.top/gtxfxyvhqh.html

[S11] C：逐行读文件
来源：http://hz.wangshuangyany.cn/gtnilnshrz.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.guannengcc.top/gtsyrawstt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zdqjudy.top/gtxucbmkzh.html

fclose(f);
来源：http://hz.gzhubu.top/gtbgrtbell.html

[S12] C：写文件
来源：http://hz.jinyuanbaomall.cn/gtfbvsdqbf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hysaishi.cn/gtkzbdgnkr.html

[S13] C：宏定义
来源：http://hz.yuanzhike.top/gtbbsnnxeg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhijiandao.cn/gtldalomll.html

[S14] C：枚举
来源：http://hz.ybcxt.top/gtwhpkkxgl.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jianghu66.top/gtqndtmkgv.html

[S15] C：类型转换
来源：http://hz.316326.xyz/gtsexsccue.html

(double) a / b
来源：http://hz.52xcode.cn/gtbpbcmtki.html

[S16] C：位操作置位
来源：http://hz.xuetiantiany.cn/gtovzmuywo.html

x |= (1 << 3);
来源：http://hz.shanyushiyangtech.top/gtbbyflgxx.html

[S17] C：安全拼接字符串
来源：http://hz.fzhhl.top/gtojzsrrlc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.redwolf501.top/gtsjcoqsqh.html

[S18] C：命令行参数
来源：http://hz.andypj.xyz/gtbprwlyep.html

int main(int argc, char **argv)
来源：http://hz.zhaomingkeji.xyz/gtpcjipugs.html

[S19] C：快速排序
来源：http://hz.tian-w.cn/gtdjrmjzmm.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.feifeiyinyue.top/gtuoorgmsh.html

[S20] C：二分查找
来源：http://hz.yuxming.cn/gtsjgnuznb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jinqigufen.top/gtjkdbrsef.html

[S21] C：字符类别判断
来源：http://hz.cheryme.top/gtdwqjhapd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.tanke756.top/gtahvpyyow.html

[S22] C：字符串转数字
来源：http://hz.hfpthk.cn/gtiantupff.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhaomingkeji.xyz/gttornmfbm.html

[S23] C：随机数
来源：http://hz.yvedp.cn/gtbrtplyof.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.mhx1999.top/gtllnpqkmc.html

[S24] C：获取本地时间
来源：http://hz.chenzaomai.com/gtbnxatifa.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hfpthk.cn/gtfnngmasb.html

[S25] C：内存拷贝
来源：http://hz.guannengcc.top/gtwdxalzgk.html

memcpy(dst, src, n);
来源：http://hz.hywenlv.cn/gtpprpitbq.html

[S26] C：内存清零
来源：http://hz.nanxinkj.top/gtlkcjuype.html

memset(a, 0, sizeof a);
来源：http://hz.yanxiufei.cn/gtegpattmk.html

[S27] C：定义常量
来源：http://hz.sxryk.cn/gtycoelpoz.html

const double PI = 3.14159;
来源：http://hz.tian-w.cn/gtvbyrokvh.html

[S28] C：静态变量
来源：http://hz.mhx1999.top/gtsiffvzxh.html

static int counter = 0;
来源：http://hz.shanyushiyangtech.top/gtoxjhvstj.html

[S29] C：变参函数
来源：http://hz.ydjk.org.cn/gtwnsdjjon.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.birdmap.top/gtejdllulm.html

[S30] C：头文件保护
来源：http://hz.zhiwuduotai.top/gtkkkgxcbe.html

#ifndef X_H
来源：http://hz.snrcjt.cn/gtykebcsle.html

#define X_H
来源：http://hz.jinqigfzy.top/gtbbzrqzjq.html

#endif
来源：http://hz.yangfankeji.com/gtxnnftxrd.html

[S31] C++：Hello World
来源：http://hz.fengsongda.top/gtydadrzav.html

#include <iostream>
来源：http://hz.jqgufenzy.top/gturtxhucp.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xuanzx.com/gtwbhpfzea.html

[S32] C++：字符串
来源：http://hz.kuanghao11.cn/gtqdgqxnhs.html

std::string s = "hi";  s += "!";
来源：http://hz.cdnleiting.top/gtkonoqvhq.html

[S33] C++：vector 增删
来源：http://hz.chenlongwang.top/gtzsmtpggc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zhiwuduotai.top/gthzhwllgd.html

[S34] C++：遍历 vector
来源：http://hz.mhx1999.top/gthnfdockv.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.9152youxi.cn/gthasroymo.html

[S35] C++：map
来源：http://hz.meibo888.top/gtulqrknni.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj20258.top/gtatughera.html

[S36] C++：unordered_map
来源：http://hz.xinyue.icu/gtfdsmzjit.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nwbrower.top/gtgkafqwhb.html

[S37] C++：set
来源：http://hz.guowangkeji.top/gtlujpepyq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.dianchejie.cn/gtlcfnpvpc.html

[S38] C++：排序
来源：http://hz.gogol.net.cn/gtttdxyqfs.html

std::sort(v.begin(), v.end());
来源：http://hz.sxryk.cn/gtukvyebgy.html

[S39] C++：自定义比较器排序
来源：http://hz.sweek.top/gtdwimhrxd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.c1oappe.top/gthrhvausf.html

[S40] C++：查找元素
来源：http://hz.hysaishi.cn/gtxwleibty.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.gaohongyu789.top/gtlggxkgdz.html

[S41] C++：类与构造函数
来源：http://hz.xuetiantiany.cn/gtfszctsxx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.meibo888.top/gtykigvrpe.html

[S42] C++：继承与虚函数
来源：http://hz.dashuyun.cn/gtnitgqzrj.html

class B : public Base { public: void f() override {} };
来源：http://hz.ydjk.org.cn/gtacwdrpbt.html

[S43] C++：智能指针
来源：http://hz.smart0.xyz/gtdjfqoeeu.html

auto p = std::make_unique<int>(5);
来源：http://hz.kuanghao11.cn/gtyczziwfy.html

[S44] C++：引用传参
来源：http://hz.pengpengdd.cyou/gtapnyrdek.html

void inc(int &x) { ++x; }
来源：http://hz.zdqjudy.top/gtntuwccqb.html

[S45] C++：lambda
来源：http://hz.yongpay.top/gtfsggkfmi.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.shangyingyoupin.top/gtjkvejmyx.html

[S46] C++：函数模板
来源：http://hz.pengpengdd.cyou/gtutkjkvyy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.pengpengdd.cyou/gtgvayovvu.html

[S47] C++：结构化绑定遍历
来源：http://hz.ydjk.org.cn/gthnnvckkq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.tianlin.xyz/gtlphdlngs.html

[S48] C++：逐行读文件
来源：http://hz.tanke756.top/gtcedixmog.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.sweek.top/gtxhvjarye.html

while (std::getline(in, line)) { }
来源：http://hz.mhx1999.top/gtpofoeyme.html

[S49] C++：写文件
来源：http://hz.jlsjyb.cn/gtpwxpejko.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.9152youxi.cn/gtaidbtpiw.html

[S50] C++：格式化数字
来源：http://hz.xylfe.cn/gtwvhozlmk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zycfv.cn/gtdbooxqic.html

[S51] C++：显式类型转换
来源：http://hz.wangdashe.top/gtxqweouvz.html

static_cast<double>(a) / b
来源：http://hz.jinqigfzy.top/gtnepjazni.html

[S52] C++：const 与 noexcept
来源：http://hz.meibo888.top/gtlyhubcfh.html

int size() const noexcept { return n_; }
来源：http://hz.ybcxt.top/gtllclsmqm.html

[S53] C++：移动语义
来源：http://hz.birdmap.top/gtbyrgtolq.html

std::vector<int> w = std::move(v);
来源：http://hz.daxiang520.top/gtexgdsubf.html

[S54] C++：异常处理
来源：http://hz.xingfuxueyuan.xyz/gteptucaed.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhoulong.xyz/gtpmuibgfx.html

[S55] C++：结构化绑定
来源：http://hz.wangdashe.top/gtgaevgodb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.pycfn.com/gtnjjltdau.html

[S56] C++：optional
来源：http://hz.pycfn.com/gtkwsrxjul.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.gotoacloud.top/gtwuubacfs.html

[S57] C++：编译期常量
来源：http://hz.zhiwuduotai.top/gtrrixhkwm.html

constexpr int N = 10;
来源：http://hz.chenzaomai.com/gtwdqcwuay.html

[S58] C++：命名空间
来源：http://hz.quarkkingdee.top/gtpfglhbbs.html

namespace ns { int f() { return 1; } }
来源：http://hz.ivvv.top/gtuehazjzd.html

[S59] C++：静态断言
来源：http://hz.sxryk.cn/gtgtptdylr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.guowangkeji.top/gtfppjjilw.html

[S60] C++：遍历并删除元素
来源：http://hz.shzxlz.cn/gtttqpzfrc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.aibaodan.cn/gtsukqlqvm.html

================================================================================
来源：http://hz.zhixingplan.top/gtglunyrvo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.iojbl.cn/gtaeohhuyo.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtsxfletab.html

[T01] Kotlin：Hello World
来源：http://hz.chenjidiqi.icu/gtifipmnzt.html

println("Hello")
来源：http://hz.kuanghao11.cn/gttegzbzug.html

[T02] Kotlin：变量
来源：http://hz.xuanzx.com/gtzdtdkjkj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xingfuxueyuan.xyz/gtiigyqbqq.html

[T03] Kotlin：字符串模板
来源：http://hz.tianlin.xyz/gteuvmiaku.html

"值: $b"
来源：http://hz.zhijiandao.cn/gtjlxscjku.html

[T04] Kotlin：空安全
来源：http://hz.feifeiyinyue.top/gtzvpofwus.html

val n: String? = null;  n?.length
来源：http://hz.cdnleiting.top/gtqivcsuid.html

[T05] Kotlin：when 表达式
来源：http://hz.ywan-chungtsiang.top/gtiyitdxap.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.fengsongda.top/gtuxfqcbrc.html

[T06] Kotlin：集合映射
来源：http://hz.cashguo.top/gtgeuvznly.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.xuetiantiany.cn/gtmcmwuqad.html

[T07] Kotlin：集合过滤
来源：http://hz.yongpay.top/gtdkylwczj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yueranfly.top/gtjoeqwcli.html

[T08] Kotlin：数据类
来源：http://hz.daxiang520.top/gtppjhajiz.html

data class User(val name: String, val age: Int)
来源：http://hz.zhengqikj.top/gtbdazewca.html

[T09] Kotlin：扩展函数
来源：http://hz.hywenlv.cn/gtchokpxch.html

fun String.exclaim() = this + "!"
来源：http://hz.dianchejie.cn/gtwbnaktdj.html

[T10] Kotlin：默认参数
来源：http://hz.jqgufenzy.top/gtjmoyvhfq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yongpay.top/gtfdtyxafa.html

[T11] Kotlin：协程
来源：http://hz.shuidangran.top/gtcfiltemx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.svipenyu.cn/gtryqholvm.html

[T12] Kotlin：解构声明
来源：http://hz.hysaishi.cn/gtwgwqndpn.html

val (a, b) = Pair(1, 2)
来源：http://hz.daxiang520.top/gtkxudlcii.html

[T13] Kotlin：只读 Map
来源：http://hz.shangyingyoupin.top/gtgkplaiku.html

val m = mapOf("a" to 1)
来源：http://hz.zhixingplan.top/gtxfzqetnv.html

[T14] Kotlin：循环
来源：http://hz.hysaishi.cn/gtxyrjjczv.html

for (i in 1..10) println(i)
来源：http://hz.tian-w.cn/gtqheebodt.html

[T15] Kotlin：接口
来源：http://hz.hysaishi.cn/gtvpzqourb.html

interface Shape { fun area(): Double }
来源：http://hz.sysykeji.top/gtobywlvbx.html

[T16] Swift：Hello World
来源：http://hz.svipenyu.cn/gthfnghhih.html

print("Hello")
来源：http://hz.daria6918.cn/gtabypvmug.html

[T17] Swift：变量与常量
来源：http://hz.cdnleiting.top/gtkzujpere.html

var a = 1;  let b = 2
来源：http://hz.tianlin.xyz/gtzalolsix.html

[T18] Swift：字符串插值
来源：http://hz.fengsongda.top/gtbgybtkei.html

"值: \(b)"
来源：http://hz.shanyushiyangkeji.top/gtxowjpjvn.html

[T19] Swift：可选绑定
来源：http://hz.cdnleiting.top/gtsylnjpvk.html

if let n = opt { print(n) }
来源：http://hz.yangfankeji.com/gtuvcypjlo.html

[T20] Swift：数组操作
来源：http://hz.jqgfzy.top/gtnrfeqrpt.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.svipenyu.cn/gtgjlzpbtu.html

[T21] Swift：遍历
来源：http://hz.daria6918.cn/gtvjthhugm.html

for x in a { print(x) }
来源：http://hz.jinqigfzy.top/gtgrhebaqf.html

[T22] Swift：字典
来源：http://hz.zhixingplan.top/gtgenygcnt.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.52xcode.cn/gtjvthhkyz.html

[T23] Swift：函数
来源：http://hz.yvedp.cn/gtpqgvrndf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.wangdashe.top/gtkldxpuyh.html

[T24] Swift：闭包
来源：http://hz.zhaomingkeji.xyz/gtmtoczvso.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yuanzhike.top/gtntanrunl.html

[T25] Swift：结构体
来源：http://hz.tanke756.top/gtsfblkxrg.html

struct P { var x: Int }
来源：http://hz.vqdsnc.cn/gtybehplht.html

[T26] Swift：类与重写
来源：http://hz.meibo888.top/gtanqwmdhi.html

class A: Base { override func f() {} }
来源：http://hz.yanxiufei.cn/gtwreoxekl.html

[T27] Swift：错误处理
来源：http://hz.shanyushiyangtech.top/gtpkxcrmrm.html

do { try f() } catch { print(error) }
来源：http://hz.hnqzz.top/gtrmqgprpt.html

[T28] Swift：枚举
来源：http://hz.jlsjyb.cn/gtfeigvqnt.html

enum Color { case red, green }
来源：http://hz.jlsjyb.cn/gtrenetknz.html

[T29] Swift：guard 提前返回
来源：http://hz.gogol.net.cn/gtklqtmhni.html

guard let x = opt else { return }
来源：http://hz.xuetiantiany.cn/gtmitjnklg.html

[T30] Swift：协议
来源：http://hz.shzxlz.cn/gtyoulabpe.html

protocol Shape { func area() -> Double }
来源：http://hz.xylfe.cn/gtsvxzuynx.html

[T31] Lua：Hello World
来源：http://hz.dashuyun.cn/gtdrmuookz.html

print("Hello")
来源：http://hz.gzhubu.top/gtjxgaymye.html

[T32] Lua：局部变量
来源：http://hz.0kj1m.cn/gtpmrtmmun.html

local a = 1
来源：http://hz.yanxiufei.cn/gtfchhzxmd.html

[T33] Lua：表（数组）
来源：http://hz.jinghuilouyu.cn/gtlzatujuq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.52xcode.cn/gtfzqdvzmi.html

[T34] Lua：遍历表
来源：http://hz.xuetiantiany.cn/gtukvckbqv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.chenzaomai.com/gtuzweqjrz.html

[T35] Lua：字典表
来源：http://hz.smart0.xyz/gtcqydwfmx.html

local d = { a = 1 };  d.b = 2
来源：http://hz.pengpengdd.cyou/gtdezoaqrr.html

[T36] Lua：函数
来源：http://hz.svipenyu.cn/gtivmnjcnw.html

function add(a, b) return a + b end
来源：http://hz.zhoulong.xyz/gtbyukibzc.html

[T37] Lua：字符串拼接
来源：http://hz.cqqwz.cn/gthazpetwx.html

"a" .. "b"
来源：http://hz.smart0.xyz/gtvvcwxvep.html

[T38] Lua：条件
来源：http://hz.cucudq.cn/gthcwstzul.html

if x > 0 then print("正") end
来源：http://hz.jinghuilouyu.cn/gtsfqpgcey.html

[T39] Lua：模式匹配
来源：http://hz.aizwys.cn/gtuayyywdd.html

string.find(s, "%d+")
来源：http://hz.gaohongyu789.top/gtvtxxlwrq.html

[T40] Lua：元表
来源：http://hz.shanyushiyangtech.top/gtnjwodoye.html

setmetatable({}, { __index = base })
来源：http://hz.gzhubu.top/gtufodslxu.html

[T41] Perl：Hello World
来源：http://hz.snrcjt.cn/gtbnqiytcp.html

print "Hello\n";
来源：http://hz.cucudq.cn/gthknyjbka.html

[T42] Perl：变量类型
来源：http://hz.ybcxt.top/gtonrknzng.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.fzhhl.top/gtffogstqg.html

[T43] Perl：字符串插值
来源：http://hz.cheryme.top/gtjflyyxnd.html

"值: $a"
来源：http://hz.hfpthk.cn/gtgbxvxnzh.html

[T44] Perl：条件
来源：http://hz.gogol.net.cn/gtasvpneky.html

if ($a > 0) { print "正"; }
来源：http://hz.vqdsnc.cn/gtdqgrxpgu.html

[T45] Perl：数组遍历
来源：http://hz.ydzc1.top/gtboadgzar.html

for my $x (@arr) { print $x; }
来源：http://hz.cucudq.cn/gtzilcskez.html

[T46] Perl：哈希操作
来源：http://hz.chenzaomai.com/gtsxfpygpr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.gogol.net.cn/gtznqtahrd.html

[T47] Perl：正则捕获
来源：http://hz.ehwqpu.com/gtzettmvqu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.gzhubu.top/gtbiefnylj.html

[T48] Perl：正则替换
来源：http://hz.daxiang520.top/gtprfxlsqf.html

$s =~ s/old/new/g;
来源：http://hz.jinqigfzy.top/gtohtljptc.html

[T49] Perl：函数
来源：http://hz.wangshuangyany.cn/gtjtuanypp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.haohaochexian.top/gtxhmqwrdl.html

[T50] Perl：逐行读文件
来源：http://hz.jinghuilouyu.cn/gtkgdikklf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yvedp.cn/gttrncgrbr.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.ydjk.org.cn/gtqzjmxtwu.html

[T51] Scala：Hello World
来源：http://hz.nanxuanxn.top/gtalugeuil.html

println("Hello")
来源：http://hz.shanyushiyangtech.top/gtioddrmqa.html

[T52] Scala：变量
来源：http://hz.cucudq.cn/gtuzirutrz.html

val a = 1;  var b = 2
来源：http://hz.daxiang520.top/gtqlrjehsn.html

[T53] Scala：字符串插值
来源：http://hz.jinqigufen.top/gttqmvwuln.html

s"值: $b"
来源：http://hz.yj202588.top/gtsvltohfu.html

[T54] Scala：集合映射
来源：http://hz.xinyue.icu/gtynacjaiy.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.jyoumei.cn/gtqugdmggm.html

[T55] Scala：集合过滤
来源：http://hz.hfpthk.cn/gtzdizcuyq.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.haohaochexian.top/gtwfzpxibz.html

[T56] Scala：样例类
来源：http://hz.9152youxi.cn/gtiybvvzmv.html

case class User(name: String, age: Int)
来源：http://hz.jinyuanbaomall.cn/gtmmzterop.html

[T57] Scala：模式匹配
来源：http://hz.vqdsnc.cn/gtfnyfamhw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.vqdsnc.cn/gturespxmr.html

[T58] Scala：函数定义
来源：http://hz.yongpay.top/gthsgkpujn.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.feifeiyinyue.top/gturigarbm.html

[T59] Scala：循环
来源：http://hz.yuanzhike.top/gtycemledl.html

for (i <- 1 to 10) println(i)
来源：http://hz.daxiang520.top/gtlojvkozk.html

[T60] Scala：折叠
来源：http://hz.gaohongyu789.top/gtrhkijghv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.nanxinkj.top/gtiojbatcw.html

================================================================================
来源：http://hz.yangfankeji.com/gtfmsrfges.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jlsjyb.cn/gtlahclhac.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtvnqmwilm.html

[U01] Py：创建虚拟环境
来源：http://hz.snrcjt.cn/gtehgjxegp.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.feifeiyinyue.top/gtutahywhu.html

[U02] Py：导出 / 安装依赖
来源：http://hz.sxryk.cn/gtjvorymny.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.ydjk.org.cn/gtgwgvgart.html

[U03] Py：加载 .env 配置
来源：http://hz.bjfxy.top/gtucfzsacd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.wangshuangyany.cn/gtoktxrxvr.html

[U04] Py：变量调试打印
来源：http://hz.guannengcc.top/gttfmddgnk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.hnxiangtu.top/gtorymnnyh.html

[U05] Py：列表去重且保序
来源：http://hz.zhengqikj.top/gtawhfjfbi.html

list(dict.fromkeys(arr))
来源：http://hz.jlsjyb.cn/gtuftwwxxf.html

[U06] Py：合并两个字典
来源：http://hz.svipenyu.cn/gtsfxfxzjk.html

{**a, **b}
来源：http://hz.cdnleiting.top/gtjothgwve.html

[U07] Py：反转字典键值
来源：http://hz.wangshuangyany.cn/gthxkscilf.html

{v: k for k, v in d.items()}
来源：http://hz.jianghu66.top/gtsmgnlhxh.html

[U08] Py：展平二维列表
来源：http://hz.shzxlz.cn/gtdfszentq.html

[y for x in nested for y in x]
来源：http://hz.tanke756.top/gtcuwbwoxt.html

[U09] Py：字典取最大值的键
来源：http://hz.xinyue.icu/gtprhdekhd.html

max(d, key=d.get)
来源：http://hz.hywenlv.cn/gtnpcmfcrt.html

[U10] Py：按值排序字典
来源：http://hz.yongpay.top/gtmkhzzdjb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.cashguo.top/gtbfvcjbma.html

[U11] Py：生成器表达式
来源：http://hz.yanxiufei.cn/gtdhjcgjjj.html

(x * 2 for x in arr)
来源：http://hz.shzxlz.cn/gtkpabhtpf.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.zhijiandao.cn/gtnmgdlmht.html

Counter(arr).most_common(3)
来源：http://hz.jqgfzy.top/gtvahxccuk.html

[U13] Py：固定长度队列
来源：http://hz.cdnleiting.top/gtnlqznnfv.html

deque(maxlen=10)
来源：http://hz.ywan-chungtsiang.top/gtrwupehjb.html

[U14] Py：分组收集到列表
来源：http://hz.ppjwa.cn/gtsycxkotd.html

defaultdict(list)
来源：http://hz.jinghuilouyu.cn/gtczgrzltp.html

[U15] Py：高精度计时
来源：http://hz.jqgfzy.top/gtvpadshtq.html

t = time.perf_counter()
来源：http://hz.yonumen.top/gtemftkasf.html

[U16] Py：命令行参数解析
来源：http://hz.xuanzx.com/gtufxanozw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.chenjidiqi.icu/gtlephdsvh.html

[U17] Py：初始化日志
来源：http://hz.yuxming.cn/gtgmpbiiuf.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.zhaomingkeji.xyz/gtpphwedun.html

[U18] Py：预编译正则
来源：http://hz.jyoumei.cn/gtijcbhark.html

pat = re.compile(r"\d+")
来源：http://hz.jinqigfzy.top/gtskxoprdo.html

[U19] Py：正则替换带回调
来源：http://hz.sxryk.cn/gtgihrkjyl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.zdqjudy.top/gtlvjknvvg.html

[U20] Py：缓存函数结果
来源：http://hz.sxryk.cn/gtisufergh.html

@functools.lru_cache(maxsize=None)
来源：http://hz.xziqi.cn/gthveaqrdd.html

[U21] Py：自定义上下文管理器
来源：http://hz.sweek.top/gtovwwxloe.html

@contextlib.contextmanager
来源：http://hz.feifeiyinyue.top/gtiwdmrlcv.html

[U22] Py：矩阵转置
来源：http://hz.pengpengdd.cyou/gtrgackglp.html

list(zip(*m))
来源：http://hz.quarkkingdee.top/gtpnyyhtoi.html

[U23] Py：分块读取大文件
来源：http://hz.tianlin.xyz/gtksomezsy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.0kj1m.cn/gtiondxgco.html

[U24] Py：路径操作
来源：http://hz.hywenlv.cn/gtyhpqvzgv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.zhixingplan.top/gtwkbkyeij.html


<!-- 参考信息 -->