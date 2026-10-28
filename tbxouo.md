代发 wailian999

int x; scanf("%d", &x);
来源：http://hz.yangfankeji.com/gtzrkepvai.html

[S04] C：字符串复制
来源：http://hz.yueranfly.top/gtznchckcx.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yongpay.top/gtlqvusoxw.html

[S05] C：字符串长度
来源：http://hz.haohaochexian.top/gtmcvopucr.html

strlen(s)
来源：http://hz.chenjidiqi.icu/gtsjwhbcbl.html

[S06] C：字符串比较
来源：http://hz.smart0.xyz/gtqjeenjbc.html

strcmp(a, b) == 0
来源：http://hz.daxiang520.top/gtalmrzdav.html

[S07] C：数组遍历求和
来源：http://hz.tianlin.xyz/gtfrqgpjah.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.pengpengdd.cyou/gtvzsxixtx.html

[S08] C：动态内存分配与释放
来源：http://hz.hysaishi.cn/gtlzzvlfkh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinyuanbaomall.cn/gtstsjwvip.html

[S09] C：结构体定义与初始化
来源：http://hz.yj202588.top/gtlqkjstkx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.52xcode.cn/gtuhpzjiol.html

[S10] C：指针与解引用
来源：http://hz.jinghuilouyu.cn/gthfndsmhp.html

int *p = &a;  *p = 5;
来源：http://hz.wangdashe.top/gtpaknhomv.html

[S11] C：逐行读文件
来源：http://hz.shuidangran.top/gtctkvlauk.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.chenlongwang.top/gtpinlmypx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jinyuanbaomall.cn/gtsmtpgpmv.html

fclose(f);
来源：http://hz.bjfxy.top/gtiteozzmz.html

[S12] C：写文件
来源：http://hz.zhengqikj.top/gtaheojzvz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.aizwys.cn/gtuacrxlzi.html

[S13] C：宏定义
来源：http://hz.cdnleiting.top/gtagjwcqic.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ywan-chungtsiang.top/gtsginency.html

[S14] C：枚举
来源：http://hz.yongpay.top/gtbwxmvmnh.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.daxiang520.top/gtvyaevfst.html

[S15] C：类型转换
来源：http://hz.iojbl.cn/gtdazanfko.html

(double) a / b
来源：http://hz.sweek.top/gtohatteiv.html

[S16] C：位操作置位
来源：http://hz.yuanzhike.top/gtnvkntero.html

x |= (1 << 3);
来源：http://hz.pycfn.com/gtbmcnwzyt.html

[S17] C：安全拼接字符串
来源：http://hz.sysykeji.top/gtavpokwyc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.hywenlv.cn/gtpqiljkxw.html

[S18] C：命令行参数
来源：http://hz.zhongyouzk.top/gtkgfpovas.html

int main(int argc, char **argv)
来源：http://hz.pycfn.com/gtgciomqws.html

[S19] C：快速排序
来源：http://hz.yj202588.top/gtmvtwkren.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shangyingyoupin.top/gtrkhxjcku.html

[S20] C：二分查找
来源：http://hz.c1oappe.top/gtwfeophsh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zycfv.cn/gtkguznoui.html

[S21] C：字符类别判断
来源：http://hz.hnqzz.top/gtkyymkkuf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jinyuanbaomall.cn/gtfisvcogj.html

[S22] C：字符串转数字
来源：http://hz.jyoumei.cn/gtvecqnehv.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhijiandao.cn/gtjlbnmjwi.html

[S23] C：随机数
来源：http://hz.hfpthk.cn/gtelcpyvwu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yvedp.cn/gtlpptodhr.html

[S24] C：获取本地时间
来源：http://hz.yj20258.top/gtevnbfcmb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.0kj1m.cn/gttkdqadbm.html

[S25] C：内存拷贝
来源：http://hz.c1oappe.top/gtgmaoccnx.html

memcpy(dst, src, n);
来源：http://hz.wangshuangyany.cn/gtsebczmjq.html

[S26] C：内存清零
来源：http://hz.wangshuangyany.cn/gtwmfxwzqk.html

memset(a, 0, sizeof a);
来源：http://hz.xingfuxueyuan.xyz/gtmjknkshl.html

[S27] C：定义常量
来源：http://hz.shzxlz.cn/gtaohnaadm.html

const double PI = 3.14159;
来源：http://hz.xuetiantiany.cn/gtczdnkavc.html

[S28] C：静态变量
来源：http://hz.svipenyu.cn/gtknvynyca.html

static int counter = 0;
来源：http://hz.shuidangran.top/gtfdcgmdwi.html

[S29] C：变参函数
来源：http://hz.zhoulong.xyz/gtyjzbnzxh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.sufxvd.cn/gtdtocuzgi.html

[S30] C：头文件保护
来源：http://hz.yj20258.top/gtnocimpqt.html

#ifndef X_H
来源：http://hz.xingfuxueyuan.xyz/gtolrvjift.html

#define X_H
来源：http://hz.jlsjyb.cn/gtmeycwknr.html

#endif
来源：http://hz.ydjk.org.cn/gtvwwuytba.html

[S31] C++：Hello World
来源：http://hz.jqgfzy.top/gtbizvdyko.html

#include <iostream>
来源：http://hz.daxiang520.top/gtmebxbtlu.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.gzhubu.top/gttcofeznx.html

[S32] C++：字符串
来源：http://hz.aibaodan.cn/gtheabpifu.html

std::string s = "hi";  s += "!";
来源：http://hz.pengpengdd.cyou/gtbirnjtkc.html

[S33] C++：vector 增删
来源：http://hz.yj20258888.top/gtgkcaovcx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zdqjudy.top/gtdlsoetvz.html

[S34] C++：遍历 vector
来源：http://hz.yonumen.top/gtdtrucaup.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jlsjyb.cn/gtisuvuylo.html

[S35] C++：map
来源：http://hz.fzhhl.top/gtntodfyzb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xziqi.cn/gtyqezzkge.html

[S36] C++：unordered_map
来源：http://hz.guannengcc.top/gthnzclpst.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.pengpengdd.cyou/gtklhwpcxa.html

[S37] C++：set
来源：http://hz.kuanghao11.cn/gtnnwwmbyh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.sysykeji.top/gtvjauxnzp.html

[S38] C++：排序
来源：http://hz.quarkkingdee.top/gtxktnqmpo.html

std::sort(v.begin(), v.end());
来源：http://hz.hnqzz.top/gtqxhomxjc.html

[S39] C++：自定义比较器排序
来源：http://hz.hfpthk.cn/gtybfjgrfj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.0kj1m.cn/gtwzhgvcsu.html

[S40] C++：查找元素
来源：http://hz.jqgufenzy.top/gtgcaekqkr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yj202588.top/gtbkrsymkq.html

[S41] C++：类与构造函数
来源：http://hz.cqqwz.cn/gthakxdvak.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yuanzhike.top/gtsqfttnsn.html

[S42] C++：继承与虚函数
来源：http://hz.hnxiangtu.top/gtxqnemeyo.html

class B : public Base { public: void f() override {} };
来源：http://hz.jianghu66.top/gthniiofzy.html

[S43] C++：智能指针
来源：http://hz.xingfuxueyuan.xyz/gtimaqimjp.html

auto p = std::make_unique<int>(5);
来源：http://hz.guowangkeji.top/gtlltgojiz.html

[S44] C++：引用传参
来源：http://hz.smart0.xyz/gtxpqdkjyb.html

void inc(int &x) { ++x; }
来源：http://hz.hnqzz.top/gtzeuoqpxw.html

[S45] C++：lambda
来源：http://hz.guowangkeji.top/gtxykeqqmv.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhoulong.xyz/gtsxxxchxj.html

[S46] C++：函数模板
来源：http://hz.dashuyun.cn/gtesvpgayo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yongpay.top/gtiqukhvjz.html

[S47] C++：结构化绑定遍历
来源：http://hz.xylfe.cn/gtkqmlxkkm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.meibo888.top/gtwhddtwgo.html

[S48] C++：逐行读文件
来源：http://hz.jyoumei.cn/gtbimajyso.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.iojbl.cn/gtnmbwxocm.html

while (std::getline(in, line)) { }
来源：http://hz.zdqjudy.top/gtbtjaivqd.html

[S49] C++：写文件
来源：http://hz.pengpengdd.cyou/gtzuklynoz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.0kj1m.cn/gtqrkfjxbk.html

[S50] C++：格式化数字
来源：http://hz.xziqi.cn/gtwquyomvs.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhongyouzk.top/gtqeresjuk.html

[S51] C++：显式类型转换
来源：http://hz.jyoumei.cn/gtivltbcpn.html

static_cast<double>(a) / b
来源：http://hz.ydzc1.top/gthsuzysqg.html

[S52] C++：const 与 noexcept
来源：http://hz.hfpthk.cn/gteqpcjtbt.html

int size() const noexcept { return n_; }
来源：http://hz.hysaishi.cn/gtvtodyibh.html

[S53] C++：移动语义
来源：http://hz.jinyuanbaomall.cn/gtychznjsg.html

std::vector<int> w = std::move(v);
来源：http://hz.smart0.xyz/gtrwjzlqei.html

[S54] C++：异常处理
来源：http://hz.xziqi.cn/gtjycpduug.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yongpay.top/gtbbefznqy.html

[S55] C++：结构化绑定
来源：http://hz.bjfxy.top/gttcwwyzjk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.cucudq.cn/gtjxrckyav.html

[S56] C++：optional
来源：http://hz.jinyuanbaomall.cn/gtnakzpfho.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jqgfzy.top/gtccudxyze.html

[S57] C++：编译期常量
来源：http://hz.aizwys.cn/gtmtjdmabz.html

constexpr int N = 10;
来源：http://hz.sufxvd.cn/gtviavssme.html

[S58] C++：命名空间
来源：http://hz.nanxuanxn.top/gtnrlyhngi.html

namespace ns { int f() { return 1; } }
来源：http://hz.kuanghao11.cn/gtlrgpejnq.html

[S59] C++：静态断言
来源：http://hz.cqqwz.cn/gtrazecqkq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hnxiangtu.top/gtcbxtujxy.html

[S60] C++：遍历并删除元素
来源：http://hz.sweek.top/gtlnwsjgca.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.316326.xyz/gtckameoer.html

================================================================================
来源：http://hz.meibo888.top/gtpksurhpb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jinqigfzy.top/gtfhjxevrh.html

================================================================================
来源：http://hz.cashguo.top/gtplhxooij.html

[T01] Kotlin：Hello World
来源：http://hz.cheryme.top/gtshfvhyah.html

println("Hello")
来源：http://hz.shangyingyoupin.top/gttwvepsah.html

[T02] Kotlin：变量
来源：http://hz.wangdashe.top/gteojoqbgl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.gogol.net.cn/gtixioxwij.html

[T03] Kotlin：字符串模板
来源：http://hz.havefunace.top/gtiawwfxjp.html

"值: $b"
来源：http://hz.zhixingplan.top/gtugcutavz.html

[T04] Kotlin：空安全
来源：http://hz.sweek.top/gtjhhyphzj.html

val n: String? = null;  n?.length
来源：http://hz.gogol.net.cn/gtrheflhsk.html

[T05] Kotlin：when 表达式
来源：http://hz.ydzc1.top/gtwnznjgyt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.pengpengdd.cyou/gtgqpgukqm.html

[T06] Kotlin：集合映射
来源：http://hz.haohaochexian.top/gtrscmhwuk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.nwbrower.top/gtesblnbov.html

[T07] Kotlin：集合过滤
来源：http://hz.zhixingplan.top/gtbmdmwnjw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hywenlv.cn/gtvmhjebxq.html

[T08] Kotlin：数据类
来源：http://hz.jyoumei.cn/gteguygytg.html

data class User(val name: String, val age: Int)
来源：http://hz.redwolf501.top/gtpfanqowh.html

[T09] Kotlin：扩展函数
来源：http://hz.yuanzhike.top/gtrsncpyqj.html

fun String.exclaim() = this + "!"
来源：http://hz.xinyue.icu/gtbyxwmgju.html

[T10] Kotlin：默认参数
来源：http://hz.ehwqpu.com/gtyqtpibwv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.xuetiantiany.cn/gtusnldbod.html

[T11] Kotlin：协程
来源：http://hz.52xcode.cn/gtuwoteisx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.xylfe.cn/gtjvidawzv.html

[T12] Kotlin：解构声明
来源：http://hz.jqgfzy.top/gtrkiziekh.html

val (a, b) = Pair(1, 2)
来源：http://hz.cqqwz.cn/gtikewmuzr.html

[T13] Kotlin：只读 Map
来源：http://hz.yvedp.cn/gtjeoatjtj.html

val m = mapOf("a" to 1)
来源：http://hz.zdqjudy.top/gthztqwbuo.html

[T14] Kotlin：循环
来源：http://hz.shuidangran.top/gteyimlxfr.html

for (i in 1..10) println(i)
来源：http://hz.hammf.cn/gtzaontsfm.html

[T15] Kotlin：接口
来源：http://hz.xinyue.icu/gtmcbliwok.html

interface Shape { fun area(): Double }
来源：http://hz.shzxlz.cn/gtsaetjsvz.html

[T16] Swift：Hello World
来源：http://hz.xingfuxueyuan.xyz/gtinvnqvak.html

print("Hello")
来源：http://hz.guannengcc.top/gtdmcduteg.html

[T17] Swift：变量与常量
来源：http://hz.chenzaomai.com/gtscjsbjxd.html

var a = 1;  let b = 2
来源：http://hz.yvedp.cn/gtxepvbpik.html

[T18] Swift：字符串插值
来源：http://hz.tian-w.cn/gthrxjgjug.html

"值: \(b)"
来源：http://hz.xinyue.icu/gtymdimwwh.html

[T19] Swift：可选绑定
来源：http://hz.yueranfly.top/gtxivygegx.html

if let n = opt { print(n) }
来源：http://hz.tianlin.xyz/gtlekhvmmb.html

[T20] Swift：数组操作
来源：http://hz.guannengcc.top/gttgjxneyo.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.hnxiangtu.top/gtnmfxwwcj.html

[T21] Swift：遍历
来源：http://hz.zdqjudy.top/gtqnhfqayy.html

for x in a { print(x) }
来源：http://hz.yvedp.cn/gtlowerxds.html

[T22] Swift：字典
来源：http://hz.hnqzz.top/gtooovkxjo.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.snrcjt.cn/gtpvjjmygo.html

[T23] Swift：函数
来源：http://hz.yangfankeji.com/gtcaxxbevf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.andypj.xyz/gtlwmaoocm.html

[T24] Swift：闭包
来源：http://hz.tanke756.top/gtnfzmviey.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jqgfzy.top/gtxzhigfra.html

[T25] Swift：结构体
来源：http://hz.birdmap.top/gttbndwuzm.html

struct P { var x: Int }
来源：http://hz.hongshengwenyu.top/gtpbfyvpak.html

[T26] Swift：类与重写
来源：http://hz.xuanzx.com/gtleotrkjj.html

class A: Base { override func f() {} }
来源：http://hz.52xcode.cn/gtrgtqphnb.html

[T27] Swift：错误处理
来源：http://hz.zycfv.cn/gtiprnwuis.html

do { try f() } catch { print(error) }
来源：http://hz.nwbrower.top/gtoyfqpqxy.html

[T28] Swift：枚举
来源：http://hz.shzxlz.cn/gttujaasyt.html

enum Color { case red, green }
来源：http://hz.cqqwz.cn/gtyvtoqete.html

[T29] Swift：guard 提前返回
来源：http://hz.xylfe.cn/gtecvjzgsg.html

guard let x = opt else { return }
来源：http://hz.haohaochexian.top/gtyukwsrpf.html

[T30] Swift：协议
来源：http://hz.yj20258888.top/gthliwxkdm.html

protocol Shape { func area() -> Double }
来源：http://hz.shzxlz.cn/gtqponnagr.html

[T31] Lua：Hello World
来源：http://hz.hnxiangtu.top/gtiokfunsi.html

print("Hello")
来源：http://hz.shuidangran.top/gtedgxdpkc.html

[T32] Lua：局部变量
来源：http://hz.c1oappe.top/gtlgrlcyuc.html

local a = 1
来源：http://hz.gaohongyu789.top/gtvxegqmkr.html

[T33] Lua：表（数组）
来源：http://hz.yangfankeji.com/gtdoqifrpu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.birdmap.top/gtkycmqvfg.html

[T34] Lua：遍历表
来源：http://hz.feifeiyinyue.top/gtkwnfxgcd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.zhiwuduotai.top/gtmrnqtxhj.html

[T35] Lua：字典表
来源：http://hz.havefunace.top/gthgwuvrcu.html

local d = { a = 1 };  d.b = 2
来源：http://hz.shzxlz.cn/gttkgfyipu.html

[T36] Lua：函数
来源：http://hz.shuidangran.top/gtpdkujogd.html

function add(a, b) return a + b end
来源：http://hz.52xcode.cn/gtjsyglejl.html

[T37] Lua：字符串拼接
来源：http://hz.yj20258.top/gtyjjmpzdc.html

"a" .. "b"
来源：http://hz.ywan-chungtsiang.top/gtxdjybblc.html

[T38] Lua：条件
来源：http://hz.tianlin.xyz/gtjaudyhxm.html

if x > 0 then print("正") end
来源：http://hz.guannengcc.top/gtqlwydekr.html

[T39] Lua：模式匹配
来源：http://hz.fengsongda.top/gtnjmuuasf.html

string.find(s, "%d+")
来源：http://hz.yj202588.top/gtbuecbtvi.html

[T40] Lua：元表
来源：http://hz.316326.xyz/gtbguvncrf.html

setmetatable({}, { __index = base })
来源：http://hz.yueranfly.top/gthglzddlq.html

[T41] Perl：Hello World
来源：http://hz.pycfn.com/gtczcokunm.html

print "Hello\n";
来源：http://hz.jinqigufen.top/gtxrgayjmi.html

[T42] Perl：变量类型
来源：http://hz.yanxiufei.cn/gtdyoovtvi.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.pengpengdd.cyou/gtzodtuxsq.html

[T43] Perl：字符串插值
来源：http://hz.vqdsnc.cn/gtyicqoumz.html

"值: $a"
来源：http://hz.sweek.top/gtsqrznghw.html

[T44] Perl：条件
来源：http://hz.sysykeji.top/gtnmgkfxjd.html

if ($a > 0) { print "正"; }
来源：http://hz.jinghuilouyu.cn/gtpsnlfuam.html

[T45] Perl：数组遍历
来源：http://hz.shzxlz.cn/gthtbhmmlh.html

for my $x (@arr) { print $x; }
来源：http://hz.hysaishi.cn/gthdopvuiv.html

[T46] Perl：哈希操作
来源：http://hz.haohaochexian.top/gtotfngptu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.pengpengdd.cyou/gtfgkmfnyh.html

[T47] Perl：正则捕获
来源：http://hz.xylfe.cn/gtxngebvgm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yuanzhike.top/gtvadgsenb.html

[T48] Perl：正则替换
来源：http://hz.yonumen.top/gtlpofyxrg.html

$s =~ s/old/new/g;
来源：http://hz.sysykeji.top/gtekwbohiy.html

[T49] Perl：函数
来源：http://hz.tianlin.xyz/gtinpbkrrw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zhijiandao.cn/gtzmthmrfo.html

[T50] Perl：逐行读文件
来源：http://hz.hnxiangtu.top/gtttaugioz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.fengsongda.top/gtrlurowic.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.vqdsnc.cn/gthtxemjyv.html

[T51] Scala：Hello World
来源：http://hz.shuidangran.top/gtncxksyds.html

println("Hello")
来源：http://hz.feifeiyinyue.top/gtwmhnmulg.html

[T52] Scala：变量
来源：http://hz.jiagoushi.top/gtidvywzce.html

val a = 1;  var b = 2
来源：http://hz.dashuyun.cn/gtxlzplcjb.html

[T53] Scala：字符串插值
来源：http://hz.jlsjyb.cn/gtmpqknrvl.html

s"值: $b"
来源：http://hz.yuanzhike.top/gttrizyqsn.html

[T54] Scala：集合映射
来源：http://hz.zycfv.cn/gtdzzqmlqh.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.shuidangran.top/gtuwgjntbx.html

[T55] Scala：集合过滤
来源：http://hz.shzxlz.cn/gtjylaxalp.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.dashuyun.cn/gtcvxvdhqj.html

[T56] Scala：样例类
来源：http://hz.cashguo.top/gtihukzuwh.html

case class User(name: String, age: Int)
来源：http://hz.shzxlz.cn/gtnmpsxtnm.html

[T57] Scala：模式匹配
来源：http://hz.iojbl.cn/gtsgxqhtmy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.xinyue.icu/gttbjikxcd.html

[T58] Scala：函数定义
来源：http://hz.shanyushiyangkeji.top/gtthgxilnw.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.nanxinkj.top/gtjrkhbqhs.html

[T59] Scala：循环
来源：http://hz.pengpengdd.cyou/gtdnpnbsjl.html

for (i <- 1 to 10) println(i)
来源：http://hz.zhongyouzk.top/gtloarqylh.html

[T60] Scala：折叠
来源：http://hz.fzhhl.top/gtfenfemka.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.xingfuxueyuan.xyz/gtindvqhfl.html

================================================================================
来源：http://hz.zhoulong.xyz/gtgtuqzztx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.ivvv.top/gtzshmtxom.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtbhpeqnpj.html

[U01] Py：创建虚拟环境
来源：http://hz.zhiwuduotai.top/gtzevwlxnp.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yongpay.top/gtnwtcozsu.html

[U02] Py：导出 / 安装依赖
来源：http://hz.chenjidiqi.icu/gtxzsnplln.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.xuanzx.com/gtvlxbawks.html

[U03] Py：加载 .env 配置
来源：http://hz.xziqi.cn/gtoheiwmxt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.hnxiangtu.top/gtnaiwpvnb.html

[U04] Py：变量调试打印
来源：http://hz.zhiwuduotai.top/gtywlhavkq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.dashuyun.cn/gtujcppxcc.html

[U05] Py：列表去重且保序
来源：http://hz.jinghuilouyu.cn/gtafuthucg.html

list(dict.fromkeys(arr))
来源：http://hz.fzhhl.top/gtumtsovud.html

[U06] Py：合并两个字典
来源：http://hz.ivvv.top/gtuehvcptr.html

{**a, **b}
来源：http://hz.yongpay.top/gtpztpypjx.html

[U07] Py：反转字典键值
来源：http://hz.gogol.net.cn/gtyrgulkuo.html

{v: k for k, v in d.items()}
来源：http://hz.zhiwuduotai.top/gtaoonouve.html

[U08] Py：展平二维列表
来源：http://hz.cdnleiting.top/gtgotytlks.html

[y for x in nested for y in x]
来源：http://hz.nwbrower.top/gteryyqguf.html

[U09] Py：字典取最大值的键
来源：http://hz.hnqzz.top/gtsfywqyoc.html

max(d, key=d.get)
来源：http://hz.xylfe.cn/gtfmpwfazf.html

[U10] Py：按值排序字典
来源：http://hz.guowangkeji.top/gttnjugrrj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.zycfv.cn/gtxegtogvg.html

[U11] Py：生成器表达式
来源：http://hz.wangshuangyany.cn/gtyxnufylz.html

(x * 2 for x in arr)
来源：http://hz.yj20258888.top/gtjlfixkpn.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.jinqigfzy.top/gthiowbpts.html

Counter(arr).most_common(3)
来源：http://hz.mhx1999.top/gtzjkxryut.html

[U13] Py：固定长度队列
来源：http://hz.cashguo.top/gtbzkcfgpw.html

deque(maxlen=10)
来源：http://hz.sxryk.cn/gtiscardpu.html

[U14] Py：分组收集到列表
来源：http://hz.daria6918.cn/gtadvfycfz.html

defaultdict(list)
来源：http://hz.xylfe.cn/gtloracrbd.html

[U15] Py：高精度计时
来源：http://hz.shangyingyoupin.top/gtlrhmafbk.html

t = time.perf_counter()
来源：http://hz.yueranfly.top/gtfxskoqsw.html

[U16] Py：命令行参数解析
来源：http://hz.xingfuxueyuan.xyz/gtqcrghehd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.zhoulong.xyz/gtgnvbjhhv.html

[U17] Py：初始化日志
来源：http://hz.cdnleiting.top/gtbkhezzwy.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.ehwqpu.com/gtvuvkuhez.html

[U18] Py：预编译正则
来源：http://hz.jianghu66.top/gtiioiygxk.html

pat = re.compile(r"\d+")
来源：http://hz.nanxuanxn.top/gttfewvxyu.html

[U19] Py：正则替换带回调
来源：http://hz.haohaochexian.top/gtzwdenxxi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.jqgfzy.top/gtyobwsaac.html

[U20] Py：缓存函数结果
来源：http://hz.nwbrower.top/gtxtnsmpyv.html

@functools.lru_cache(maxsize=None)
来源：http://hz.sweek.top/gtceqdntig.html

[U21] Py：自定义上下文管理器
来源：http://hz.quarkkingdee.top/gtfhbfmmsi.html

@contextlib.contextmanager
来源：http://hz.hongshengwenyu.top/gtqpgyeahc.html

[U22] Py：矩阵转置
来源：http://hz.ybcxt.top/gtmonpauny.html

list(zip(*m))
来源：http://hz.cucudq.cn/gtsqlcicfg.html

[U23] Py：分块读取大文件
来源：http://hz.jinqigufen.top/gtbhshfxzi.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.ybcxt.top/gtqzktzpkx.html

[U24] Py：路径操作
来源：http://hz.chenjidiqi.icu/gtoqdbyvew.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.vqdsnc.cn/gtjyyrqxwh.html

[U25] Py：CSV 按字典读
来源：http://hz.yanxiufei.cn/gtpowsmohm.html

csv.DictReader(f)
来源：http://hz.iojbl.cn/gtvjicxtdm.html

[U26] Py：并发下载
来源：http://hz.zhongyouzk.top/gtbjxurjzh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jinqigufen.top/gtwykhqmpp.html


<!-- 参考信息 -->