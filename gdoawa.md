代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hongshengwenyu.top/gtkibmbkgr.html

[S02] C：变量与格式化输出
来源：http://hz.jlsjyb.cn/gtfdghondf.html

int a = 10; printf("%d\n", a);
来源：http://hz.dianchejie.cn/gtvjcntgfl.html

[S03] C：读入整数
来源：http://hz.vqdsnc.cn/gtrpwlpzio.html

int x; scanf("%d", &x);
来源：http://hz.hysaishi.cn/gtsgtcriti.html

[S04] C：字符串复制
来源：http://hz.xylfe.cn/gtxunyteav.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhixingplan.top/gtadmumhjm.html

[S05] C：字符串长度
来源：http://hz.gzhubu.top/gthmywryjs.html

strlen(s)
来源：http://hz.xuetiantiany.cn/gtdsttwrfo.html

[S06] C：字符串比较
来源：http://hz.tian-w.cn/gtkrhijzyo.html

strcmp(a, b) == 0
来源：http://hz.nwbrower.top/gtmraxilgs.html

[S07] C：数组遍历求和
来源：http://hz.cashguo.top/gtdxjywkdi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.cqqwz.cn/gtxtrddlxp.html

[S08] C：动态内存分配与释放
来源：http://hz.shangyingyoupin.top/gtjejgvogc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhiwuduotai.top/gtwmkyaeqc.html

[S09] C：结构体定义与初始化
来源：http://hz.wangshuangyany.cn/gtcfmpjpol.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jiagoushi.top/gtmvzsfynq.html

[S10] C：指针与解引用
来源：http://hz.tanke756.top/gtcloyyiwh.html

int *p = &a;  *p = 5;
来源：http://hz.yonumen.top/gthyelqzho.html

[S11] C：逐行读文件
来源：http://hz.chenlongwang.top/gtombuxmqs.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.shangyingyoupin.top/gtjckypbfx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.andypj.xyz/gtlrbgtkuj.html

fclose(f);
来源：http://hz.jinqigufen.top/gtkjqqgagb.html

[S12] C：写文件
来源：http://hz.zhiwuduotai.top/gtemjjwiuv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.aibaodan.cn/gtjdthsyqu.html

[S13] C：宏定义
来源：http://hz.iojbl.cn/gtqqgqrffz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.tianlin.xyz/gtgyvtedvk.html

[S14] C：枚举
来源：http://hz.quarkkingdee.top/gtkaowsjdo.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.chenzaomai.com/gtwatbyejt.html

[S15] C：类型转换
来源：http://hz.daxiang520.top/gtenxzzljm.html

(double) a / b
来源：http://hz.smart0.xyz/gtgaeovhhq.html

[S16] C：位操作置位
来源：http://hz.sufxvd.cn/gteoisbnpi.html

x |= (1 << 3);
来源：http://hz.tian-w.cn/gtoyxmviam.html

[S17] C：安全拼接字符串
来源：http://hz.meibo888.top/gthsnvqetp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jiagoushi.top/gtsbjvpybg.html

[S18] C：命令行参数
来源：http://hz.yueranfly.top/gtelqftfxa.html

int main(int argc, char **argv)
来源：http://hz.yonumen.top/gtjoflxime.html

[S19] C：快速排序
来源：http://hz.hnxiangtu.top/gtnxdneulb.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shzxlz.cn/gtyiwpwjxg.html

[S20] C：二分查找
来源：http://hz.zhoulong.xyz/gtkxgjnnns.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.shzxlz.cn/gtjgegygzt.html

[S21] C：字符类别判断
来源：http://hz.cucudq.cn/gtflvuqemu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yanxiufei.cn/gtqviyqveb.html

[S22] C：字符串转数字
来源：http://hz.meibo888.top/gttvymbfcd.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.fzhhl.top/gtfadppukm.html

[S23] C：随机数
来源：http://hz.dashuyun.cn/gtwwywzwjh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.smart0.xyz/gtwyrhnjxu.html

[S24] C：获取本地时间
来源：http://hz.zdqjudy.top/gtygnxgezx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.tian-w.cn/gtgvdmpjqc.html

[S25] C：内存拷贝
来源：http://hz.tianlin.xyz/gtgharctqq.html

memcpy(dst, src, n);
来源：http://hz.gaohongyu789.top/gtnmxmstom.html

[S26] C：内存清零
来源：http://hz.xingfuxueyuan.xyz/gtkzhsnvwp.html

memset(a, 0, sizeof a);
来源：http://hz.jqgufenzy.top/gtryecexns.html

[S27] C：定义常量
来源：http://hz.hnxiangtu.top/gtptetalxd.html

const double PI = 3.14159;
来源：http://hz.ehwqpu.com/gtfkhivxrg.html

[S28] C：静态变量
来源：http://hz.andypj.xyz/gtqsmwdwws.html

static int counter = 0;
来源：http://hz.shanyushiyangkeji.top/gthlqtynkn.html

[S29] C：变参函数
来源：http://hz.shangyingyoupin.top/gtrsvmmccg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.xingfuxueyuan.xyz/gtwhduaqxy.html

[S30] C：头文件保护
来源：http://hz.smart0.xyz/gtsppoxsmr.html

#ifndef X_H
来源：http://hz.jinqigfzy.top/gtloxbpxvm.html

#define X_H
来源：http://hz.quarkkingdee.top/gtpztczyro.html

#endif
来源：http://hz.meibo888.top/gtgquivvzj.html

[S31] C++：Hello World
来源：http://hz.yonumen.top/gtcpgpipme.html

#include <iostream>
来源：http://hz.nwbrower.top/gtrmtrmhwg.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zhengqikj.top/gtmkiceymm.html

[S32] C++：字符串
来源：http://hz.xziqi.cn/gttgfujkou.html

std::string s = "hi";  s += "!";
来源：http://hz.nanxuanxn.top/gtjgsricnd.html

[S33] C++：vector 增删
来源：http://hz.ppjwa.cn/gtprizytsf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jqgfzy.top/gtwolzjpoi.html

[S34] C++：遍历 vector
来源：http://hz.hnxiangtu.top/gtngkvdcvh.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.gotoacloud.top/gttyukghqw.html

[S35] C++：map
来源：http://hz.yanxiufei.cn/gthuydmtyc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.daxiang520.top/gtrmwlkrbx.html

[S36] C++：unordered_map
来源：http://hz.cashguo.top/gtypgxnbed.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinyuanbaomall.cn/gtcipfyfny.html

[S37] C++：set
来源：http://hz.zhongyouzk.top/gtvfkfkjtb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xuanzx.com/gtusikbugd.html

[S38] C++：排序
来源：http://hz.pengpengdd.cyou/gthyralvse.html

std::sort(v.begin(), v.end());
来源：http://hz.wangshuangyany.cn/gtprycpnwp.html

[S39] C++：自定义比较器排序
来源：http://hz.cqqwz.cn/gtvbhpcfwt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ppjwa.cn/gtyndtjoqn.html

[S40] C++：查找元素
来源：http://hz.tanke756.top/gtzsspzxiv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xuetiantiany.cn/gtbppwgvpl.html

[S41] C++：类与构造函数
来源：http://hz.ehwqpu.com/gtogdhfead.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xinyue.icu/gtjwsggtux.html

[S42] C++：继承与虚函数
来源：http://hz.haohaochexian.top/gtdvvtsfci.html

class B : public Base { public: void f() override {} };
来源：http://hz.9152youxi.cn/gtmobwcgme.html

[S43] C++：智能指针
来源：http://hz.ywan-chungtsiang.top/gtejcerkcs.html

auto p = std::make_unique<int>(5);
来源：http://hz.sxryk.cn/gtsbfuxyxc.html

[S44] C++：引用传参
来源：http://hz.yj20258.top/gtvekyrrtm.html

void inc(int &x) { ++x; }
来源：http://hz.bjfxy.top/gtvbroymou.html

[S45] C++：lambda
来源：http://hz.nanxinkj.top/gtizkeekmv.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hongshengwenyu.top/gtycewzimg.html

[S46] C++：函数模板
来源：http://hz.zhongyouzk.top/gtmgjpstnf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.52xcode.cn/gtcelggmje.html

[S47] C++：结构化绑定遍历
来源：http://hz.sxryk.cn/gtaylclgsa.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.nwbrower.top/gtxkyrhkdw.html

[S48] C++：逐行读文件
来源：http://hz.jqgufenzy.top/gtztswtnvx.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yuanzhike.top/gtamsorhfn.html

while (std::getline(in, line)) { }
来源：http://hz.feifeiyinyue.top/gtzvxczdgz.html

[S49] C++：写文件
来源：http://hz.sufxvd.cn/gteccvubml.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.gaohongyu789.top/gtzwqtddph.html

[S50] C++：格式化数字
来源：http://hz.yuanzhike.top/gtxsfdmlyi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.xuanzx.com/gtvvbyukxl.html

[S51] C++：显式类型转换
来源：http://hz.hnqzz.top/gtngrrscgv.html

static_cast<double>(a) / b
来源：http://hz.9152youxi.cn/gttltovoev.html

[S52] C++：const 与 noexcept
来源：http://hz.hongshengwenyu.top/gtapgvprct.html

int size() const noexcept { return n_; }
来源：http://hz.hnxiangtu.top/gtgkndyxyq.html

[S53] C++：移动语义
来源：http://hz.shangyingyoupin.top/gthypqwydk.html

std::vector<int> w = std::move(v);
来源：http://hz.cdnleiting.top/gtyitiobbh.html

[S54] C++：异常处理
来源：http://hz.zhengqikj.top/gtibqngvrm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yj20258888.top/gtbjeqhbvn.html

[S55] C++：结构化绑定
来源：http://hz.yvedp.cn/gttspsbkzz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yonumen.top/gtirjtxdlu.html

[S56] C++：optional
来源：http://hz.ehwqpu.com/gtxewfneex.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.shanyushiyangkeji.top/gtvwtrrdml.html

[S57] C++：编译期常量
来源：http://hz.snrcjt.cn/gtlnlcatku.html

constexpr int N = 10;
来源：http://hz.zhijiandao.cn/gtajeejgrm.html

[S58] C++：命名空间
来源：http://hz.andypj.xyz/gtowfcrgtk.html

namespace ns { int f() { return 1; } }
来源：http://hz.feifeiyinyue.top/gtdsmbtynq.html

[S59] C++：静态断言
来源：http://hz.sxryk.cn/gttdpxlkbi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.cheryme.top/gtywcbvygx.html

[S60] C++：遍历并删除元素
来源：http://hz.guowangkeji.top/gtbhnycfcp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zycfv.cn/gtdjzeoxvn.html

================================================================================
来源：http://hz.cheryme.top/gtboafutnq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.kuanghao11.cn/gttlvcvukm.html

================================================================================
来源：http://hz.hnxiangtu.top/gtdoviyobo.html

[T01] Kotlin：Hello World
来源：http://hz.yangfankeji.com/gtrhywnjsl.html

println("Hello")
来源：http://hz.zhaomingkeji.xyz/gtldpakfhc.html

[T02] Kotlin：变量
来源：http://hz.zhaomingkeji.xyz/gtiihlpaub.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.nanxuanxn.top/gtwsfqyvkm.html

[T03] Kotlin：字符串模板
来源：http://hz.jianghu66.top/gtjiddjfgb.html

"值: $b"
来源：http://hz.nwbrower.top/gtdvvcrith.html

[T04] Kotlin：空安全
来源：http://hz.yj202588.top/gtgohrvgdj.html

val n: String? = null;  n?.length
来源：http://hz.316326.xyz/gtejxnrfqr.html

[T05] Kotlin：when 表达式
来源：http://hz.0kj1m.cn/gtukthopuv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yuxming.cn/gtyknisola.html

[T06] Kotlin：集合映射
来源：http://hz.tian-w.cn/gtiaztetpo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.ybcxt.top/gtutvmlwnl.html

[T07] Kotlin：集合过滤
来源：http://hz.tianlin.xyz/gtpuzjjawl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.nanxuanxn.top/gtfyypsdum.html

[T08] Kotlin：数据类
来源：http://hz.quarkkingdee.top/gtikfamfak.html

data class User(val name: String, val age: Int)
来源：http://hz.meibo888.top/gtlzbwuwjl.html

[T09] Kotlin：扩展函数
来源：http://hz.jinghuilouyu.cn/gtvqbyxyot.html

fun String.exclaim() = this + "!"
来源：http://hz.xuetiantiany.cn/gtzyvjijmw.html

[T10] Kotlin：默认参数
来源：http://hz.zhengqikj.top/gtejmhoaeo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.shzxlz.cn/gtiyrsosyk.html

[T11] Kotlin：协程
来源：http://hz.daria6918.cn/gtdrdmdfxl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jinyuanbaomall.cn/gtiyjtvzkm.html

[T12] Kotlin：解构声明
来源：http://hz.bjfxy.top/gtttzptimq.html

val (a, b) = Pair(1, 2)
来源：http://hz.yuxming.cn/gtagloygxu.html

[T13] Kotlin：只读 Map
来源：http://hz.cqqwz.cn/gtzqzjaohg.html

val m = mapOf("a" to 1)
来源：http://hz.daxiang520.top/gtjncgdwez.html

[T14] Kotlin：循环
来源：http://hz.cheryme.top/gttprsqhui.html

for (i in 1..10) println(i)
来源：http://hz.ivvv.top/gtwlhcgvnr.html

[T15] Kotlin：接口
来源：http://hz.dashuyun.cn/gtrhjcygsn.html

interface Shape { fun area(): Double }
来源：http://hz.jqgufenzy.top/gtqwtlmycd.html

[T16] Swift：Hello World
来源：http://hz.shanyushiyangtech.top/gtrrvzhiga.html

print("Hello")
来源：http://hz.gzhubu.top/gtbldbibcf.html

[T17] Swift：变量与常量
来源：http://hz.hammf.cn/gtleojbafa.html

var a = 1;  let b = 2
来源：http://hz.jyoumei.cn/gtsaaxsjzf.html

[T18] Swift：字符串插值
来源：http://hz.hnqzz.top/gtvszagqqp.html

"值: \(b)"
来源：http://hz.nanxinkj.top/gtqlxesqhi.html

[T19] Swift：可选绑定
来源：http://hz.sysykeji.top/gtnjakbvjt.html

if let n = opt { print(n) }
来源：http://hz.gogol.net.cn/gtszyqqudg.html

[T20] Swift：数组操作
来源：http://hz.wangshuangyany.cn/gtjfbjgnma.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.fzhhl.top/gtkjzqsxju.html

[T21] Swift：遍历
来源：http://hz.tian-w.cn/gtgmbwhsun.html

for x in a { print(x) }
来源：http://hz.xuetiantiany.cn/gtqogmkehl.html

[T22] Swift：字典
来源：http://hz.hfpthk.cn/gthbyqfjgy.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.gaohongyu789.top/gtarzegajx.html

[T23] Swift：函数
来源：http://hz.guowangkeji.top/gtmcrsvcoq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.gogol.net.cn/gtimaszpqz.html

[T24] Swift：闭包
来源：http://hz.yongpay.top/gtgevevguq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhengqikj.top/gttizvbqnd.html

[T25] Swift：结构体
来源：http://hz.sweek.top/gtbjzsenei.html

struct P { var x: Int }
来源：http://hz.yanxiufei.cn/gtqcaztyzw.html

[T26] Swift：类与重写
来源：http://hz.hysaishi.cn/gttrqwzgnj.html

class A: Base { override func f() {} }
来源：http://hz.c1oappe.top/gtfodyqyyv.html

[T27] Swift：错误处理
来源：http://hz.nanxuanxn.top/gtagyvppew.html

do { try f() } catch { print(error) }
来源：http://hz.ywan-chungtsiang.top/gtmqbohpvv.html

[T28] Swift：枚举
来源：http://hz.sweek.top/gtlzjxbpeu.html

enum Color { case red, green }
来源：http://hz.zhijiandao.cn/gtcgngwdec.html

[T29] Swift：guard 提前返回
来源：http://hz.chenjidiqi.icu/gtquvfcwgx.html

guard let x = opt else { return }
来源：http://hz.yanxiufei.cn/gtbcpmrjpm.html

[T30] Swift：协议
来源：http://hz.tian-w.cn/gtoochbozq.html

protocol Shape { func area() -> Double }
来源：http://hz.52xcode.cn/gtiniokvxb.html

[T31] Lua：Hello World
来源：http://hz.chenzaomai.com/gtmwtfanoh.html

print("Hello")
来源：http://hz.ydjk.org.cn/gthqtmtgao.html

[T32] Lua：局部变量
来源：http://hz.meibo888.top/gtdomntufn.html

local a = 1
来源：http://hz.tanke756.top/gtyuzpjxwd.html

[T33] Lua：表（数组）
来源：http://hz.zhijiandao.cn/gtjovxeyxs.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.birdmap.top/gtuktbcebu.html

[T34] Lua：遍历表
来源：http://hz.sufxvd.cn/gtcenzynyb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.zhiwuduotai.top/gtgxfcjqgk.html

[T35] Lua：字典表
来源：http://hz.jianghu66.top/gtjeozzrsb.html

local d = { a = 1 };  d.b = 2
来源：http://hz.guannengcc.top/gtrqjkeojf.html

[T36] Lua：函数
来源：http://hz.xingfuxueyuan.xyz/gtkkwuhpab.html

function add(a, b) return a + b end
来源：http://hz.ydjk.org.cn/gtherwlomc.html

[T37] Lua：字符串拼接
来源：http://hz.yonumen.top/gtgixfpnny.html

"a" .. "b"
来源：http://hz.smart0.xyz/gtztwymtyx.html

[T38] Lua：条件
来源：http://hz.shanyushiyangtech.top/gtbirobcnm.html

if x > 0 then print("正") end
来源：http://hz.nanxuanxn.top/gtgmazufbz.html

[T39] Lua：模式匹配
来源：http://hz.smart0.xyz/gtvfvlqtje.html

string.find(s, "%d+")
来源：http://hz.dashuyun.cn/gtpepzwkch.html

[T40] Lua：元表
来源：http://hz.9152youxi.cn/gtcsivfpgp.html

setmetatable({}, { __index = base })
来源：http://hz.cdnleiting.top/gtwavwehda.html

[T41] Perl：Hello World
来源：http://hz.hfpthk.cn/gtlyknqouj.html

print "Hello\n";
来源：http://hz.nwbrower.top/gtojmhafhm.html

[T42] Perl：变量类型
来源：http://hz.gaohongyu789.top/gtkeuwxuxu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.fzhhl.top/gtvtvjgvae.html

[T43] Perl：字符串插值
来源：http://hz.jinyuanbaomall.cn/gtzuvhefax.html

"值: $a"
来源：http://hz.kuanghao11.cn/gtfwefrtll.html

[T44] Perl：条件
来源：http://hz.jqgfzy.top/gttwtfzoli.html

if ($a > 0) { print "正"; }
来源：http://hz.zhixingplan.top/gtbkpdcdwr.html

[T45] Perl：数组遍历
来源：http://hz.xingfuxueyuan.xyz/gtbfpbberi.html

for my $x (@arr) { print $x; }
来源：http://hz.daxiang520.top/gtihimdxwu.html

[T46] Perl：哈希操作
来源：http://hz.fengsongda.top/gtaqmmhrwh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.vqdsnc.cn/gtvesolnrx.html

[T47] Perl：正则捕获
来源：http://hz.gaohongyu789.top/gtnhzlaxrj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.sufxvd.cn/gtvneftymj.html

[T48] Perl：正则替换
来源：http://hz.jinqigufen.top/gtudxksgzm.html

$s =~ s/old/new/g;
来源：http://hz.316326.xyz/gtoojjucyt.html

[T49] Perl：函数
来源：http://hz.andypj.xyz/gtiywiziev.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zhijiandao.cn/gtxruhgecd.html

[T50] Perl：逐行读文件
来源：http://hz.hfpthk.cn/gtnhhpwpsj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.sxryk.cn/gtpphmvbsr.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.ehwqpu.com/gtfvefrifb.html

[T51] Scala：Hello World
来源：http://hz.jinghuilouyu.cn/gtrfxwkeot.html

println("Hello")
来源：http://hz.feifeiyinyue.top/gtajbrwnfv.html

[T52] Scala：变量
来源：http://hz.ehwqpu.com/gtkeqlomdw.html

val a = 1;  var b = 2
来源：http://hz.xuanzx.com/gtinlkxplf.html

[T53] Scala：字符串插值
来源：http://hz.hnxiangtu.top/gtpjfavfjj.html

s"值: $b"
来源：http://hz.xuanzx.com/gtbauvcwwv.html

[T54] Scala：集合映射
来源：http://hz.dashuyun.cn/gtolxzdesw.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.hammf.cn/gtinufsxyy.html

[T55] Scala：集合过滤
来源：http://hz.chenzaomai.com/gtplwdetqu.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.wangshuangyany.cn/gtorpbkgde.html

[T56] Scala：样例类
来源：http://hz.shzxlz.cn/gtenpuulwj.html

case class User(name: String, age: Int)
来源：http://hz.svipenyu.cn/gtisgtcrcm.html

[T57] Scala：模式匹配
来源：http://hz.hnxiangtu.top/gtnhatctgp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.haohaochexian.top/gtawjyslho.html

[T58] Scala：函数定义
来源：http://hz.smart0.xyz/gtoopdmemy.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jinghuilouyu.cn/gtfsupdapg.html

[T59] Scala：循环
来源：http://hz.yuxming.cn/gttxtpocqm.html

for (i <- 1 to 10) println(i)
来源：http://hz.jyoumei.cn/gtwkllbycs.html

[T60] Scala：折叠
来源：http://hz.meibo888.top/gttfehbfwp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.fzhhl.top/gtduyebyna.html

================================================================================
来源：http://hz.jlsjyb.cn/gtjxfqqwnw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.cdnleiting.top/gtsxlpktsz.html

================================================================================
来源：http://hz.haohaochexian.top/gttnurfrsm.html

[U01] Py：创建虚拟环境
来源：http://hz.jinqigufen.top/gtedohzzcr.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yongpay.top/gtjwxyifpq.html

[U02] Py：导出 / 安装依赖
来源：http://hz.cdnleiting.top/gtmnlhctpa.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.cdnleiting.top/gtmogfaxsx.html

[U03] Py：加载 .env 配置
来源：http://hz.fzhhl.top/gteptjnuth.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.cucudq.cn/gtqeaoqfsb.html

[U04] Py：变量调试打印
来源：http://hz.daria6918.cn/gtarujpqix.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.hnqzz.top/gttningqsy.html

[U05] Py：列表去重且保序
来源：http://hz.sweek.top/gtsutbqzqy.html

list(dict.fromkeys(arr))
来源：http://hz.gzhubu.top/gtptjosbvq.html

[U06] Py：合并两个字典
来源：http://hz.zhiwuduotai.top/gtaoaqktqi.html

{**a, **b}
来源：http://hz.yuxming.cn/gtcrtwqmyz.html

[U07] Py：反转字典键值
来源：http://hz.hywenlv.cn/gtyyeqldha.html

{v: k for k, v in d.items()}
来源：http://hz.yuxming.cn/gtmbutgppc.html

[U08] Py：展平二维列表
来源：http://hz.dashuyun.cn/gtrcwmuroq.html

[y for x in nested for y in x]
来源：http://hz.xylfe.cn/gtxadpueac.html

[U09] Py：字典取最大值的键
来源：http://hz.chenjidiqi.icu/gtqitgiwri.html

max(d, key=d.get)
来源：http://hz.smart0.xyz/gtjvonemgz.html

[U10] Py：按值排序字典
来源：http://hz.redwolf501.top/gtjxmbpkyc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.hnxiangtu.top/gtiuytmosw.html

[U11] Py：生成器表达式
来源：http://hz.gotoacloud.top/gtjbxtvdkb.html

(x * 2 for x in arr)
来源：http://hz.jqgufenzy.top/gtdzdffsyn.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.feifeiyinyue.top/gtyboqwitt.html

Counter(arr).most_common(3)
来源：http://hz.jinqigufen.top/gtyzgsfvcd.html

[U13] Py：固定长度队列
来源：http://hz.zhiwuduotai.top/gtogexvviu.html

deque(maxlen=10)
来源：http://hz.ehwqpu.com/gtflrinigk.html

[U14] Py：分组收集到列表
来源：http://hz.svipenyu.cn/gtxozfimhf.html

defaultdict(list)
来源：http://hz.havefunace.top/gtvjyhbplw.html

[U15] Py：高精度计时
来源：http://hz.ybcxt.top/gtwbupuxmk.html

t = time.perf_counter()
来源：http://hz.wangdashe.top/gtlsoddxov.html

[U16] Py：命令行参数解析
来源：http://hz.yj202588.top/gtjcndiado.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jinghuilouyu.cn/gtkypydnts.html

[U17] Py：初始化日志
来源：http://hz.52xcode.cn/gtkawfwpao.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.guannengcc.top/gtaoaoroae.html

[U18] Py：预编译正则
来源：http://hz.haohaochexian.top/gtbkmnpuhw.html

pat = re.compile(r"\d+")
来源：http://hz.chenzaomai.com/gtdtxmcxhg.html

[U19] Py：正则替换带回调
来源：http://hz.chenzaomai.com/gteirqvwra.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.birdmap.top/gtvbhhejld.html

[U20] Py：缓存函数结果
来源：http://hz.jinghuilouyu.cn/gtbnlxybye.html

@functools.lru_cache(maxsize=None)
来源：http://hz.sxryk.cn/gtcxzmrpgx.html

[U21] Py：自定义上下文管理器
来源：http://hz.shanyushiyangkeji.top/gtovqnjaiv.html

@contextlib.contextmanager
来源：http://hz.hnqzz.top/gtauoyjqmg.html

[U22] Py：矩阵转置
来源：http://hz.hnqzz.top/gtbmrilfiy.html

list(zip(*m))
来源：http://hz.yangfankeji.com/gtjufqsqzd.html

[U23] Py：分块读取大文件
来源：http://hz.cdnleiting.top/gtpcwtwlza.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.pengpengdd.cyou/gtztizllik.html

[U24] Py：路径操作
来源：http://hz.xingfuxueyuan.xyz/gttslozntn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.birdmap.top/gtnezgytoh.html


<!-- 参考信息 -->