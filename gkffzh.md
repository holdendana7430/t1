代发 wailian999

int x; scanf("%d", &x);
来源：http://hz.zhaomingkeji.xyz/gtfibtzpyg.html

[S04] C：字符串复制
来源：http://hz.yvedp.cn/gtpeiuxswj.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.meibo888.top/gtonwrwmga.html

[S05] C：字符串长度
来源：http://hz.nwbrower.top/gtpqhugrkt.html

strlen(s)
来源：http://hz.cqqwz.cn/gtbyrxjiyq.html

[S06] C：字符串比较
来源：http://hz.hammf.cn/gtizvsbbdm.html

strcmp(a, b) == 0
来源：http://hz.hywenlv.cn/gtcntropcu.html

[S07] C：数组遍历求和
来源：http://hz.zhengqikj.top/gtycfbqdjr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.gogol.net.cn/gtaikebilc.html

[S08] C：动态内存分配与释放
来源：http://hz.yangfankeji.com/gtorybjrff.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.shanyushiyangkeji.top/gtqgvwrpmz.html

[S09] C：结构体定义与初始化
来源：http://hz.svipenyu.cn/gtqdtmrszm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.quarkkingdee.top/gtdlfzfzvc.html

[S10] C：指针与解引用
来源：http://hz.kuanghao11.cn/gtaulhygll.html

int *p = &a;  *p = 5;
来源：http://hz.sysykeji.top/gtwcynzucd.html

[S11] C：逐行读文件
来源：http://hz.shanyushiyangkeji.top/gtovjgkdbv.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.aibaodan.cn/gteeusiztc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.sxryk.cn/gtaynqqjdf.html

fclose(f);
来源：http://hz.wangdashe.top/gtkoolssfe.html

[S12] C：写文件
来源：http://hz.tianlin.xyz/gtlrrfbjsu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.haohaochexian.top/gtecnmjukx.html

[S13] C：宏定义
来源：http://hz.yanxiufei.cn/gttgfeioig.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.gogol.net.cn/gtguygwtcc.html

[S14] C：枚举
来源：http://hz.jinghuilouyu.cn/gtxotrdvmx.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.gzhubu.top/gtqbyqtumc.html

[S15] C：类型转换
来源：http://hz.hfpthk.cn/gtbdemhfnv.html

(double) a / b
来源：http://hz.yj20258888.top/gtqhfkmawb.html

[S16] C：位操作置位
来源：http://hz.jiagoushi.top/gtlnlcgucq.html

x |= (1 << 3);
来源：http://hz.shanyushiyangkeji.top/gttkvnebpr.html

[S17] C：安全拼接字符串
来源：http://hz.yj20258888.top/gtphfbgjsl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.sweek.top/gtqoqlbnfr.html

[S18] C：命令行参数
来源：http://hz.smart0.xyz/gtjxuymkxs.html

int main(int argc, char **argv)
来源：http://hz.kuanghao11.cn/gtlxqczlkv.html

[S19] C：快速排序
来源：http://hz.9152youxi.cn/gtstwzijwz.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.gzhubu.top/gtwxjyifib.html

[S20] C：二分查找
来源：http://hz.hnqzz.top/gtdugemfpf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhijiandao.cn/gtimayrvbc.html

[S21] C：字符类别判断
来源：http://hz.zhaomingkeji.xyz/gtmyfspnnk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ivvv.top/gtduznndwy.html

[S22] C：字符串转数字
来源：http://hz.hysaishi.cn/gthczcmjjj.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.nanxinkj.top/gtplzxdetk.html

[S23] C：随机数
来源：http://hz.zhongyouzk.top/gtzrldqsig.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.daria6918.cn/gtyrmdwtra.html

[S24] C：获取本地时间
来源：http://hz.jianghu66.top/gtygzmonlh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.cucudq.cn/gteehuowuk.html

[S25] C：内存拷贝
来源：http://hz.chenjidiqi.icu/gtbtvdlnqu.html

memcpy(dst, src, n);
来源：http://hz.gotoacloud.top/gtlmrftfeg.html

[S26] C：内存清零
来源：http://hz.gaohongyu789.top/gtpwkfhoep.html

memset(a, 0, sizeof a);
来源：http://hz.chenzaomai.com/gtdneohhpl.html

[S27] C：定义常量
来源：http://hz.xylfe.cn/gtyhfbnsog.html

const double PI = 3.14159;
来源：http://hz.zhijiandao.cn/gtobmrlknz.html

[S28] C：静态变量
来源：http://hz.fzhhl.top/gtqpjbyvgt.html

static int counter = 0;
来源：http://hz.c1oappe.top/gtuuzccwob.html

[S29] C：变参函数
来源：http://hz.jqgfzy.top/gtjrpoajdn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ybcxt.top/gthpqsnmzb.html

[S30] C：头文件保护
来源：http://hz.ydzc1.top/gtzvywtnxa.html

#ifndef X_H
来源：http://hz.ydjk.org.cn/gtqptillca.html

#define X_H
来源：http://hz.andypj.xyz/gteraxjxbk.html

#endif
来源：http://hz.xinyue.icu/gtjeefwavu.html

[S31] C++：Hello World
来源：http://hz.zhoulong.xyz/gtjdwicift.html

#include <iostream>
来源：http://hz.316326.xyz/gtyzxnfhjn.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.kuanghao11.cn/gtrzxkfvfi.html

[S32] C++：字符串
来源：http://hz.0kj1m.cn/gttwbubivf.html

std::string s = "hi";  s += "!";
来源：http://hz.pengpengdd.cyou/gtcdqhhbrg.html

[S33] C++：vector 增删
来源：http://hz.pengpengdd.cyou/gthrosxmuf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zhongyouzk.top/gtuvgawkti.html

[S34] C++：遍历 vector
来源：http://hz.52xcode.cn/gtkwuwdtvy.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhaomingkeji.xyz/gtgmpajwos.html

[S35] C++：map
来源：http://hz.kuanghao11.cn/gtnwtdefpw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj202588.top/gtbdkmmjvu.html

[S36] C++：unordered_map
来源：http://hz.zycfv.cn/gtpofzunme.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhongyouzk.top/gtzedxibxe.html

[S37] C++：set
来源：http://hz.sysykeji.top/gtmswehxuv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jinghuilouyu.cn/gtngwqkbib.html

[S38] C++：排序
来源：http://hz.kuanghao11.cn/gtvqnymlez.html

std::sort(v.begin(), v.end());
来源：http://hz.daria6918.cn/gtyllnwsav.html

[S39] C++：自定义比较器排序
来源：http://hz.ywan-chungtsiang.top/gtvfmzijgb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.guowangkeji.top/gtvxikpkdo.html

[S40] C++：查找元素
来源：http://hz.nanxuanxn.top/gtnnilehxr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zdqjudy.top/gtfisdrisx.html

[S41] C++：类与构造函数
来源：http://hz.yuanzhike.top/gtyygfxphw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.daxiang520.top/gtymwanxth.html

[S42] C++：继承与虚函数
来源：http://hz.chenjidiqi.icu/gtwiqujvyc.html

class B : public Base { public: void f() override {} };
来源：http://hz.zycfv.cn/gtpownczqy.html

[S43] C++：智能指针
来源：http://hz.guannengcc.top/gtyaqcygjh.html

auto p = std::make_unique<int>(5);
来源：http://hz.wangshuangyany.cn/gtqrvfymsg.html

[S44] C++：引用传参
来源：http://hz.hysaishi.cn/gtjbqgfbjw.html

void inc(int &x) { ++x; }
来源：http://hz.ivvv.top/gtdlyribza.html

[S45] C++：lambda
来源：http://hz.bjfxy.top/gtnfmhnkke.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cashguo.top/gtlwpmizqm.html

[S46] C++：函数模板
来源：http://hz.ydjk.org.cn/gtxfuswasm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.quarkkingdee.top/gtvudrgmmb.html

[S47] C++：结构化绑定遍历
来源：http://hz.yvedp.cn/gtjcafxcom.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.hongshengwenyu.top/gtiqcckdfm.html

[S48] C++：逐行读文件
来源：http://hz.jlsjyb.cn/gtobpwsrvo.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.gaohongyu789.top/gtqdjxzwjz.html

while (std::getline(in, line)) { }
来源：http://hz.shangyingyoupin.top/gtsoukdbqh.html

[S49] C++：写文件
来源：http://hz.yanxiufei.cn/gttebdvzii.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.guannengcc.top/gttptlfgbx.html

[S50] C++：格式化数字
来源：http://hz.jinqigfzy.top/gthpztlttz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.guowangkeji.top/gtdxkojugx.html

[S51] C++：显式类型转换
来源：http://hz.jqgfzy.top/gtphhifxft.html

static_cast<double>(a) / b
来源：http://hz.jqgfzy.top/gteggzbfqe.html

[S52] C++：const 与 noexcept
来源：http://hz.zhixingplan.top/gtfoehacoj.html

int size() const noexcept { return n_; }
来源：http://hz.yj20258888.top/gtjemiepfw.html

[S53] C++：移动语义
来源：http://hz.shzxlz.cn/gtzciupoxt.html

std::vector<int> w = std::move(v);
来源：http://hz.aizwys.cn/gtntkqgomb.html

[S54] C++：异常处理
来源：http://hz.hfpthk.cn/gtzunhgcld.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ppjwa.cn/gtkkxwazqo.html

[S55] C++：结构化绑定
来源：http://hz.hysaishi.cn/gtjwrotgmy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.fengsongda.top/gtthkbgczy.html

[S56] C++：optional
来源：http://hz.chenzaomai.com/gtqfwffaaa.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.guannengcc.top/gthzbqjdag.html

[S57] C++：编译期常量
来源：http://hz.52xcode.cn/gtjhsmfobg.html

constexpr int N = 10;
来源：http://hz.meibo888.top/gteeiolfbe.html

[S58] C++：命名空间
来源：http://hz.chenlongwang.top/gtcizgugbi.html

namespace ns { int f() { return 1; } }
来源：http://hz.shzxlz.cn/gtpgslqeas.html

[S59] C++：静态断言
来源：http://hz.dashuyun.cn/gtzefqtdca.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xingfuxueyuan.xyz/gtdogjfhax.html

[S60] C++：遍历并删除元素
来源：http://hz.vqdsnc.cn/gtwlknfzwx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.ybcxt.top/gtyuhxllpa.html

================================================================================
来源：http://hz.ivvv.top/gtaursklws.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.gotoacloud.top/gtcwzbsmfs.html

================================================================================
来源：http://hz.redwolf501.top/gtdmzfgfpl.html

[T01] Kotlin：Hello World
来源：http://hz.meibo888.top/gttehkicxp.html

println("Hello")
来源：http://hz.fzhhl.top/gtfibmbhvj.html

[T02] Kotlin：变量
来源：http://hz.gotoacloud.top/gtxbrjzonx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.cheryme.top/gtbpuecaqd.html

[T03] Kotlin：字符串模板
来源：http://hz.iojbl.cn/gtgutkbijl.html

"值: $b"
来源：http://hz.nwbrower.top/gthpnoqknd.html

[T04] Kotlin：空安全
来源：http://hz.hnxiangtu.top/gtakwzgqlh.html

val n: String? = null;  n?.length
来源：http://hz.yuanzhike.top/gtqhvkrrld.html

[T05] Kotlin：when 表达式
来源：http://hz.havefunace.top/gtonsizdcs.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zhijiandao.cn/gtizxrcpmh.html

[T06] Kotlin：集合映射
来源：http://hz.jianghu66.top/gtnsqqfjxx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.chenjidiqi.icu/gtcgebksaz.html

[T07] Kotlin：集合过滤
来源：http://hz.gaohongyu789.top/gttahzqnsd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.daxiang520.top/gtemclcewa.html

[T08] Kotlin：数据类
来源：http://hz.cqqwz.cn/gtwxpknubf.html

data class User(val name: String, val age: Int)
来源：http://hz.jianghu66.top/gtloggvhob.html

[T09] Kotlin：扩展函数
来源：http://hz.cashguo.top/gtfgeokpnw.html

fun String.exclaim() = this + "!"
来源：http://hz.xuetiantiany.cn/gtypxranfx.html

[T10] Kotlin：默认参数
来源：http://hz.yueranfly.top/gtaufrbuno.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.xziqi.cn/gtsebpcrvi.html

[T11] Kotlin：协程
来源：http://hz.wangshuangyany.cn/gtugsbsyaz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.tianlin.xyz/gtdiicwyxh.html

[T12] Kotlin：解构声明
来源：http://hz.havefunace.top/gtqzaobtvx.html

val (a, b) = Pair(1, 2)
来源：http://hz.mhx1999.top/gtlsazasnk.html

[T13] Kotlin：只读 Map
来源：http://hz.yanxiufei.cn/gtuqrqcojk.html

val m = mapOf("a" to 1)
来源：http://hz.tian-w.cn/gtsrqgsntn.html

[T14] Kotlin：循环
来源：http://hz.cqqwz.cn/gttuauckfa.html

for (i in 1..10) println(i)
来源：http://hz.fzhhl.top/gtwezpjhxs.html

[T15] Kotlin：接口
来源：http://hz.pengpengdd.cyou/gtjglikolq.html

interface Shape { fun area(): Double }
来源：http://hz.pengpengdd.cyou/gtrsfcbveb.html

[T16] Swift：Hello World
来源：http://hz.snrcjt.cn/gtmgbhtbpy.html

print("Hello")
来源：http://hz.cucudq.cn/gtmsznhxho.html

[T17] Swift：变量与常量
来源：http://hz.dashuyun.cn/gtuiqoefbw.html

var a = 1;  let b = 2
来源：http://hz.daxiang520.top/gtpvabcdyp.html

[T18] Swift：字符串插值
来源：http://hz.jqgufenzy.top/gtoyobexag.html

"值: \(b)"
来源：http://hz.hysaishi.cn/gtraikcqds.html

[T19] Swift：可选绑定
来源：http://hz.yongpay.top/gtrujtakhu.html

if let n = opt { print(n) }
来源：http://hz.gogol.net.cn/gtyqrqteib.html

[T20] Swift：数组操作
来源：http://hz.xziqi.cn/gtwhrrypao.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yvedp.cn/gtccdywbvl.html

[T21] Swift：遍历
来源：http://hz.hywenlv.cn/gtrefqjuqi.html

for x in a { print(x) }
来源：http://hz.hnqzz.top/gtduajjhkc.html

[T22] Swift：字典
来源：http://hz.sxryk.cn/gtrsrowwyx.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hysaishi.cn/gtpaglbpxs.html

[T23] Swift：函数
来源：http://hz.aibaodan.cn/gtfpijmxvo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ivvv.top/gtsexhjfdp.html

[T24] Swift：闭包
来源：http://hz.shzxlz.cn/gtcwecxjff.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yuanzhike.top/gtbnoupfea.html

[T25] Swift：结构体
来源：http://hz.chenzaomai.com/gtprsxfqzb.html

struct P { var x: Int }
来源：http://hz.ydzc1.top/gtqvvmnduo.html

[T26] Swift：类与重写
来源：http://hz.birdmap.top/gttlevdcub.html

class A: Base { override func f() {} }
来源：http://hz.guannengcc.top/gtvkjdkjih.html

[T27] Swift：错误处理
来源：http://hz.birdmap.top/gtlgjsuflt.html

do { try f() } catch { print(error) }
来源：http://hz.fzhhl.top/gtzznmukdj.html

[T28] Swift：枚举
来源：http://hz.yangfankeji.com/gtxacgoxcm.html

enum Color { case red, green }
来源：http://hz.nanxinkj.top/gtofyyzpyj.html

[T29] Swift：guard 提前返回
来源：http://hz.jiagoushi.top/gtukmjsseq.html

guard let x = opt else { return }
来源：http://hz.zhiwuduotai.top/gtfssxkots.html

[T30] Swift：协议
来源：http://hz.wangdashe.top/gtlyhtldfm.html

protocol Shape { func area() -> Double }
来源：http://hz.316326.xyz/gtbmaffwrx.html

[T31] Lua：Hello World
来源：http://hz.vqdsnc.cn/gtaxhlhjys.html

print("Hello")
来源：http://hz.vqdsnc.cn/gtepnlmuwm.html

[T32] Lua：局部变量
来源：http://hz.pycfn.com/gtfayjdpxk.html

local a = 1
来源：http://hz.zhaomingkeji.xyz/gteygkdwxj.html

[T33] Lua：表（数组）
来源：http://hz.zdqjudy.top/gtoraegocb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.0kj1m.cn/gtgkdfxbhx.html

[T34] Lua：遍历表
来源：http://hz.aizwys.cn/gtjdtnbqdv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.shangyingyoupin.top/gtoukhgpzo.html

[T35] Lua：字典表
来源：http://hz.guannengcc.top/gtqydmsofw.html

local d = { a = 1 };  d.b = 2
来源：http://hz.zhoulong.xyz/gtltwyiwqm.html

[T36] Lua：函数
来源：http://hz.316326.xyz/gtfebicfis.html

function add(a, b) return a + b end
来源：http://hz.guowangkeji.top/gttnmpxyvu.html

[T37] Lua：字符串拼接
来源：http://hz.nanxinkj.top/gtspxdsuoh.html

"a" .. "b"
来源：http://hz.hongshengwenyu.top/gtoikgibql.html

[T38] Lua：条件
来源：http://hz.jinghuilouyu.cn/gtntrqmsdj.html

if x > 0 then print("正") end
来源：http://hz.zycfv.cn/gtntzletoz.html

[T39] Lua：模式匹配
来源：http://hz.9152youxi.cn/gtbeuplojf.html

string.find(s, "%d+")
来源：http://hz.yuanzhike.top/gttkswvrqq.html

[T40] Lua：元表
来源：http://hz.cqqwz.cn/gtcadmzfqy.html

setmetatable({}, { __index = base })
来源：http://hz.chenzaomai.com/gtlukmiqzw.html

[T41] Perl：Hello World
来源：http://hz.havefunace.top/gttktlgkin.html

print "Hello\n";
来源：http://hz.0kj1m.cn/gtcbbmmezp.html

[T42] Perl：变量类型
来源：http://hz.havefunace.top/gtzvzyitdo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zhoulong.xyz/gtnmnhnakl.html

[T43] Perl：字符串插值
来源：http://hz.sxryk.cn/gtvqcigwhu.html

"值: $a"
来源：http://hz.mhx1999.top/gtmzyxptcb.html

[T44] Perl：条件
来源：http://hz.316326.xyz/gtvkkunxet.html

if ($a > 0) { print "正"; }
来源：http://hz.ivvv.top/gtgzbcysut.html

[T45] Perl：数组遍历
来源：http://hz.guannengcc.top/gtuhegiwpd.html

for my $x (@arr) { print $x; }
来源：http://hz.jianghu66.top/gtchoarika.html

[T46] Perl：哈希操作
来源：http://hz.yonumen.top/gtrkfiycqo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.iojbl.cn/gtyfjxmdna.html

[T47] Perl：正则捕获
来源：http://hz.ppjwa.cn/gtwnmmrbex.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.hongshengwenyu.top/gtffdaoxeo.html

[T48] Perl：正则替换
来源：http://hz.sysykeji.top/gtiinpkvbq.html

$s =~ s/old/new/g;
来源：http://hz.sysykeji.top/gtrxpvhkrv.html

[T49] Perl：函数
来源：http://hz.jinqigfzy.top/gtukhkjncx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yvedp.cn/gttuotnsra.html

[T50] Perl：逐行读文件
来源：http://hz.yj20258888.top/gtamijfddb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.snrcjt.cn/gtabrjcbha.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yangfankeji.com/gtniehfivf.html

[T51] Scala：Hello World
来源：http://hz.iojbl.cn/gtnuonzhxf.html

println("Hello")
来源：http://hz.shzxlz.cn/gtjhwvvsjp.html

[T52] Scala：变量
来源：http://hz.chenlongwang.top/gtdookhvfu.html

val a = 1;  var b = 2
来源：http://hz.nanxuanxn.top/gtgioeridg.html

[T53] Scala：字符串插值
来源：http://hz.cashguo.top/gtmcbuvurs.html

s"值: $b"
来源：http://hz.yuanzhike.top/gtpwoeibbf.html

[T54] Scala：集合映射
来源：http://hz.jinyuanbaomall.cn/gtidbiojlm.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.52xcode.cn/gtbtxuhbdi.html

[T55] Scala：集合过滤
来源：http://hz.zhiwuduotai.top/gtnkpnhvno.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jianghu66.top/gttwawhvnl.html

[T56] Scala：样例类
来源：http://hz.ppjwa.cn/gtmkuhbeva.html

case class User(name: String, age: Int)
来源：http://hz.dianchejie.cn/gtdakmblfr.html

[T57] Scala：模式匹配
来源：http://hz.yongpay.top/gtgbhymfnk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.cucudq.cn/gtxijavtwb.html

[T58] Scala：函数定义
来源：http://hz.shuidangran.top/gtilocsvak.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.ppjwa.cn/gtzetavswp.html

[T59] Scala：循环
来源：http://hz.316326.xyz/gtodqaahnp.html

for (i <- 1 to 10) println(i)
来源：http://hz.mhx1999.top/gtjbspdcks.html

[T60] Scala：折叠
来源：http://hz.ppjwa.cn/gttqonqzcr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.shzxlz.cn/gtyyhfmntv.html

================================================================================
来源：http://hz.aizwys.cn/gtlmpldphc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhixingplan.top/gthjctahyw.html

================================================================================
来源：http://hz.guannengcc.top/gthythsunr.html

[U01] Py：创建虚拟环境
来源：http://hz.nanxuanxn.top/gtuoxqhytf.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.pengpengdd.cyou/gtpvqdjzqh.html

[U02] Py：导出 / 安装依赖
来源：http://hz.haohaochexian.top/gtbmkwdmha.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.zhixingplan.top/gtqkyvqcth.html

[U03] Py：加载 .env 配置
来源：http://hz.xziqi.cn/gtoyttspas.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.bjfxy.top/gtadxpnaps.html

[U04] Py：变量调试打印
来源：http://hz.nanxuanxn.top/gtsbohnqzk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.nwbrower.top/gtzcgunodr.html

[U05] Py：列表去重且保序
来源：http://hz.ivvv.top/gtpdhliemb.html

list(dict.fromkeys(arr))
来源：http://hz.xingfuxueyuan.xyz/gtxceoyhla.html

[U06] Py：合并两个字典
来源：http://hz.zhongyouzk.top/gtktunmyxy.html

{**a, **b}
来源：http://hz.chenlongwang.top/gtkhsjgcre.html

[U07] Py：反转字典键值
来源：http://hz.xuetiantiany.cn/gtkshwyicx.html

{v: k for k, v in d.items()}
来源：http://hz.dianchejie.cn/gtvxiyxoyu.html

[U08] Py：展平二维列表
来源：http://hz.wangdashe.top/gtisqdqlmj.html

[y for x in nested for y in x]
来源：http://hz.xuetiantiany.cn/gtllnwezib.html

[U09] Py：字典取最大值的键
来源：http://hz.hywenlv.cn/gtzddnluad.html

max(d, key=d.get)
来源：http://hz.yangfankeji.com/gtohmkhypo.html

[U10] Py：按值排序字典
来源：http://hz.xuanzx.com/gtncyxcrkn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yueranfly.top/gtfbsijdhz.html

[U11] Py：生成器表达式
来源：http://hz.hnxiangtu.top/gtoliuwmku.html

(x * 2 for x in arr)
来源：http://hz.jyoumei.cn/gtyqcikobr.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.aibaodan.cn/gtrjbbrtkr.html

Counter(arr).most_common(3)
来源：http://hz.jianghu66.top/gtuzggevnr.html

[U13] Py：固定长度队列
来源：http://hz.xziqi.cn/gtexzwqpjk.html

deque(maxlen=10)
来源：http://hz.redwolf501.top/gttalelbia.html

[U14] Py：分组收集到列表
来源：http://hz.yj20258.top/gtuvvzvmkj.html

defaultdict(list)
来源：http://hz.tianlin.xyz/gtvliupmal.html

[U15] Py：高精度计时
来源：http://hz.yj202588.top/gtwxgxdaop.html

t = time.perf_counter()
来源：http://hz.jqgufenzy.top/gtiboxfwfl.html

[U16] Py：命令行参数解析
来源：http://hz.316326.xyz/gtxtbdmvhq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.zdqjudy.top/gtohqhirlq.html

[U17] Py：初始化日志
来源：http://hz.gaohongyu789.top/gtvqjrrmzx.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.daxiang520.top/gtzrogmbpu.html

[U18] Py：预编译正则
来源：http://hz.xuanzx.com/gtjplhmprw.html

pat = re.compile(r"\d+")
来源：http://hz.pycfn.com/gtyufqixlg.html

[U19] Py：正则替换带回调
来源：http://hz.shzxlz.cn/gtczdguibd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.ehwqpu.com/gtlzotyouz.html

[U20] Py：缓存函数结果
来源：http://hz.guannengcc.top/gteiqwygde.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zhixingplan.top/gtfpqupsvn.html

[U21] Py：自定义上下文管理器
来源：http://hz.yj202588.top/gtjomwwekl.html

@contextlib.contextmanager
来源：http://hz.dianchejie.cn/gtpuzdybou.html

[U22] Py：矩阵转置
来源：http://hz.zdqjudy.top/gtvbetgedq.html

list(zip(*m))
来源：http://hz.cheryme.top/gtvctyamlw.html

[U23] Py：分块读取大文件
来源：http://hz.jinqigufen.top/gttohvgblo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.hnqzz.top/gtcocxfjli.html

[U24] Py：路径操作
来源：http://hz.vqdsnc.cn/gtlrrzkffp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.c1oappe.top/gtqeylysxu.html

[U25] Py：CSV 按字典读
来源：http://hz.zhengqikj.top/gthcufnzrl.html

csv.DictReader(f)
来源：http://hz.tianlin.xyz/gttbjtuctt.html

[U26] Py：并发下载
来源：http://hz.svipenyu.cn/gtthjybtgl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.bjfxy.top/gtpnpvlbjo.html


<!-- 参考信息 -->