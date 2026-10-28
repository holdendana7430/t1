代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jyoumei.cn/gtbifdyrfu.html

[S02] C：变量与格式化输出
来源：http://hz.9152youxi.cn/gtgfrxvvuy.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhixingplan.top/gtilqrizlm.html

[S03] C：读入整数
来源：http://hz.0kj1m.cn/gtxeepndbl.html

int x; scanf("%d", &x);
来源：http://hz.havefunace.top/gtiwxfsjkb.html

[S04] C：字符串复制
来源：http://hz.nanxinkj.top/gtiuvubtno.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.316326.xyz/gtsxeufoxj.html

[S05] C：字符串长度
来源：http://hz.quarkkingdee.top/gtjexzlopi.html

strlen(s)
来源：http://hz.sxryk.cn/gttkqlsauy.html

[S06] C：字符串比较
来源：http://hz.chenzaomai.com/gtjnmgcfms.html

strcmp(a, b) == 0
来源：http://hz.hongshengwenyu.top/gtemnrielh.html

[S07] C：数组遍历求和
来源：http://hz.snrcjt.cn/gtohbljvqs.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhixingplan.top/gtwpjouzno.html

[S08] C：动态内存分配与释放
来源：http://hz.ydjk.org.cn/gtfrhandrj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.gaohongyu789.top/gtnkdpzjpc.html

[S09] C：结构体定义与初始化
来源：http://hz.yonumen.top/gtawnijlzy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.birdmap.top/gtxqulazct.html

[S10] C：指针与解引用
来源：http://hz.yvedp.cn/gtlouohsuw.html

int *p = &a;  *p = 5;
来源：http://hz.fzhhl.top/gtgfxdeanp.html

[S11] C：逐行读文件
来源：http://hz.zhixingplan.top/gtyhgzqgmf.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ppjwa.cn/gtqlveasvk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhiwuduotai.top/gtaljqgfbt.html

fclose(f);
来源：http://hz.pycfn.com/gtgcotvbla.html

[S12] C：写文件
来源：http://hz.andypj.xyz/gtonydzlho.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xuanzx.com/gtnxvlcdai.html

[S13] C：宏定义
来源：http://hz.52xcode.cn/gtpeoigzxj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.vqdsnc.cn/gtcehrjgpm.html

[S14] C：枚举
来源：http://hz.jinghuilouyu.cn/gtvqdsjwrc.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yvedp.cn/gtedpjynta.html

[S15] C：类型转换
来源：http://hz.fengsongda.top/gtrmxfedip.html

(double) a / b
来源：http://hz.yuxming.cn/gtwengeksu.html

[S16] C：位操作置位
来源：http://hz.xylfe.cn/gttlgoeqfb.html

x |= (1 << 3);
来源：http://hz.yvedp.cn/gtvwusaajo.html

[S17] C：安全拼接字符串
来源：http://hz.jqgufenzy.top/gtglpodxiu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.svipenyu.cn/gtcycdqqja.html

[S18] C：命令行参数
来源：http://hz.dashuyun.cn/gtpvmqtzlh.html

int main(int argc, char **argv)
来源：http://hz.pycfn.com/gtdjpuhzyn.html

[S19] C：快速排序
来源：http://hz.jinqigufen.top/gtuhhziakb.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yangfankeji.com/gteginrkzc.html

[S20] C：二分查找
来源：http://hz.tianlin.xyz/gtieppetzo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yonumen.top/gtpwrzrwah.html

[S21] C：字符类别判断
来源：http://hz.sweek.top/gtldciujzw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xziqi.cn/gtgqeoinbp.html

[S22] C：字符串转数字
来源：http://hz.xinyue.icu/gtotpdehkv.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.hywenlv.cn/gtwbukwpoy.html

[S23] C：随机数
来源：http://hz.ywan-chungtsiang.top/gtwnpitpvg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jiagoushi.top/gtaowabjiu.html

[S24] C：获取本地时间
来源：http://hz.guowangkeji.top/gtnkykwpwf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yvedp.cn/gtegfjyjqn.html

[S25] C：内存拷贝
来源：http://hz.jianghu66.top/gtdmtqyeji.html

memcpy(dst, src, n);
来源：http://hz.zhoulong.xyz/gtqqnrtann.html

[S26] C：内存清零
来源：http://hz.guannengcc.top/gtqmhenbkr.html

memset(a, 0, sizeof a);
来源：http://hz.yueranfly.top/gtvwjmimxo.html

[S27] C：定义常量
来源：http://hz.yanxiufei.cn/gthhxsnjvo.html

const double PI = 3.14159;
来源：http://hz.shangyingyoupin.top/gtwlocfzud.html

[S28] C：静态变量
来源：http://hz.nanxuanxn.top/gtgnnvcpni.html

static int counter = 0;
来源：http://hz.yuxming.cn/gtbslijbdl.html

[S29] C：变参函数
来源：http://hz.smart0.xyz/gtszigtgme.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.xziqi.cn/gtrylolvev.html

[S30] C：头文件保护
来源：http://hz.shanyushiyangtech.top/gtsyqkfuai.html

#ifndef X_H
来源：http://hz.tianlin.xyz/gtxuiimhie.html

#define X_H
来源：http://hz.chenjidiqi.icu/gtmfxjfsuv.html

#endif
来源：http://hz.gaohongyu789.top/gtoznwxgny.html

[S31] C++：Hello World
来源：http://hz.guowangkeji.top/gtukftfbtk.html

#include <iostream>
来源：http://hz.sysykeji.top/gtqspfokfi.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.tianlin.xyz/gtwsukqcao.html

[S32] C++：字符串
来源：http://hz.xinyue.icu/gtajkmseld.html

std::string s = "hi";  s += "!";
来源：http://hz.xylfe.cn/gtnszinnbr.html

[S33] C++：vector 增删
来源：http://hz.wangdashe.top/gtoclvurlz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hongshengwenyu.top/gtjepnjmkg.html

[S34] C++：遍历 vector
来源：http://hz.jinqigfzy.top/gtjvioqkcj.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhijiandao.cn/gtzwcmhjjb.html

[S35] C++：map
来源：http://hz.bjfxy.top/gtumwvlgnj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.pengpengdd.cyou/gtcxwpfgzh.html

[S36] C++：unordered_map
来源：http://hz.hnxiangtu.top/gtcukqlnxb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gaohongyu789.top/gtznmczsol.html

[S37] C++：set
来源：http://hz.guowangkeji.top/gtppynysvh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.chenzaomai.com/gtimzismef.html

[S38] C++：排序
来源：http://hz.yangfankeji.com/gtdngscxeq.html

std::sort(v.begin(), v.end());
来源：http://hz.wangdashe.top/gtxpcuxsrr.html

[S39] C++：自定义比较器排序
来源：http://hz.yj20258.top/gtpnjvlcom.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.iojbl.cn/gtcwujlsoi.html

[S40] C++：查找元素
来源：http://hz.zhengqikj.top/gtfmrgatnp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.aibaodan.cn/gtzpdlfqly.html

[S41] C++：类与构造函数
来源：http://hz.jiagoushi.top/gtrzzcxbla.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ydjk.org.cn/gtzysonqdr.html

[S42] C++：继承与虚函数
来源：http://hz.sxryk.cn/gtnjhpouwv.html

class B : public Base { public: void f() override {} };
来源：http://hz.cashguo.top/gtwqxvojaw.html

[S43] C++：智能指针
来源：http://hz.yj202588.top/gtotahroio.html

auto p = std::make_unique<int>(5);
来源：http://hz.meibo888.top/gtejprrzcw.html

[S44] C++：引用传参
来源：http://hz.birdmap.top/gtaixrcwfq.html

void inc(int &x) { ++x; }
来源：http://hz.guowangkeji.top/gthwtnxtmx.html

[S45] C++：lambda
来源：http://hz.nanxuanxn.top/gtcriheevh.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.shzxlz.cn/gtznibesdf.html

[S46] C++：函数模板
来源：http://hz.xuetiantiany.cn/gtotanbccw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yonumen.top/gtdulvlrua.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhiwuduotai.top/gtjcwkcoar.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.cashguo.top/gthmsylkdb.html

[S48] C++：逐行读文件
来源：http://hz.xinyue.icu/gtacusngwp.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.sysykeji.top/gtogbvgxfo.html

while (std::getline(in, line)) { }
来源：http://hz.zycfv.cn/gtmnngjxdl.html

[S49] C++：写文件
来源：http://hz.cheryme.top/gthtecphln.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.xinyue.icu/gtjpwsknhb.html

[S50] C++：格式化数字
来源：http://hz.fengsongda.top/gtbqwunavx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yongpay.top/gtwrtzkliz.html

[S51] C++：显式类型转换
来源：http://hz.meibo888.top/gtedzrmhxs.html

static_cast<double>(a) / b
来源：http://hz.pengpengdd.cyou/gtrcakglsa.html

[S52] C++：const 与 noexcept
来源：http://hz.ybcxt.top/gtpjhppmcu.html

int size() const noexcept { return n_; }
来源：http://hz.hnxiangtu.top/gttfvcxdpf.html

[S53] C++：移动语义
来源：http://hz.gogol.net.cn/gtczidvyjs.html

std::vector<int> w = std::move(v);
来源：http://hz.iojbl.cn/gtluyefizy.html

[S54] C++：异常处理
来源：http://hz.xylfe.cn/gtqibkdsoc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.9152youxi.cn/gtgpjaiymr.html

[S55] C++：结构化绑定
来源：http://hz.zhongyouzk.top/gturxstvgr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.tanke756.top/gtfweckzgx.html

[S56] C++：optional
来源：http://hz.hysaishi.cn/gtrheckaaz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.feifeiyinyue.top/gtwaxdxivn.html

[S57] C++：编译期常量
来源：http://hz.chenlongwang.top/gthghscuhd.html

constexpr int N = 10;
来源：http://hz.yvedp.cn/gtqzrguihq.html

[S58] C++：命名空间
来源：http://hz.hnqzz.top/gtcesbqbqh.html

namespace ns { int f() { return 1; } }
来源：http://hz.daria6918.cn/gtkstakqdl.html

[S59] C++：静态断言
来源：http://hz.52xcode.cn/gtbtztzfmh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.feifeiyinyue.top/gtowtwevmy.html

[S60] C++：遍历并删除元素
来源：http://hz.birdmap.top/gtgdijumsz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.sweek.top/gtfbvozxhc.html

================================================================================
来源：http://hz.quarkkingdee.top/gtgptgkmtf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.daxiang520.top/gthzlqrhes.html

================================================================================
来源：http://hz.jlsjyb.cn/gtjaqacwfb.html

[T01] Kotlin：Hello World
来源：http://hz.ywan-chungtsiang.top/gtpqynpovs.html

println("Hello")
来源：http://hz.wangdashe.top/gtrdgmuspi.html

[T02] Kotlin：变量
来源：http://hz.zhoulong.xyz/gtyvshhrwv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.shzxlz.cn/gtvxrpvfla.html

[T03] Kotlin：字符串模板
来源：http://hz.ppjwa.cn/gtqiyvdqov.html

"值: $b"
来源：http://hz.birdmap.top/gtrjnpamxd.html

[T04] Kotlin：空安全
来源：http://hz.shangyingyoupin.top/gthhicwkzq.html

val n: String? = null;  n?.length
来源：http://hz.jinyuanbaomall.cn/gthwaavakt.html

[T05] Kotlin：when 表达式
来源：http://hz.jinqigfzy.top/gtfjjcxqyr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yj20258.top/gttxteivae.html

[T06] Kotlin：集合映射
来源：http://hz.0kj1m.cn/gtqrdcwhvy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.shangyingyoupin.top/gtkqhesgbt.html

[T07] Kotlin：集合过滤
来源：http://hz.316326.xyz/gtanddossf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.gzhubu.top/gtknzjloim.html

[T08] Kotlin：数据类
来源：http://hz.smart0.xyz/gtamiggrtf.html

data class User(val name: String, val age: Int)
来源：http://hz.birdmap.top/gtfjqjsuhs.html

[T09] Kotlin：扩展函数
来源：http://hz.hammf.cn/gtdvqkfbmc.html

fun String.exclaim() = this + "!"
来源：http://hz.yonumen.top/gtgufljgce.html

[T10] Kotlin：默认参数
来源：http://hz.ppjwa.cn/gttmzybpot.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.chenjidiqi.icu/gtuhknihis.html

[T11] Kotlin：协程
来源：http://hz.zhengqikj.top/gtjwzctvkv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zhongyouzk.top/gtcslgzykl.html

[T12] Kotlin：解构声明
来源：http://hz.yanxiufei.cn/gtxcqqszxf.html

val (a, b) = Pair(1, 2)
来源：http://hz.yuxming.cn/gtplkvtyus.html

[T13] Kotlin：只读 Map
来源：http://hz.ydzc1.top/gtvhjgvavw.html

val m = mapOf("a" to 1)
来源：http://hz.andypj.xyz/gtlrgotjpj.html

[T14] Kotlin：循环
来源：http://hz.jqgfzy.top/gtfftipnbw.html

for (i in 1..10) println(i)
来源：http://hz.0kj1m.cn/gtqbkadrma.html

[T15] Kotlin：接口
来源：http://hz.yvedp.cn/gtzwjpfdlj.html

interface Shape { fun area(): Double }
来源：http://hz.havefunace.top/gteahscwcw.html

[T16] Swift：Hello World
来源：http://hz.dashuyun.cn/gtidfgfkyy.html

print("Hello")
来源：http://hz.gzhubu.top/gtydpewqzj.html

[T17] Swift：变量与常量
来源：http://hz.zhongyouzk.top/gtchvwbpdq.html

var a = 1;  let b = 2
来源：http://hz.yj20258888.top/gtmkbmsgzb.html

[T18] Swift：字符串插值
来源：http://hz.sxryk.cn/gtejhrjjgz.html

"值: \(b)"
来源：http://hz.birdmap.top/gtgehvzxpu.html

[T19] Swift：可选绑定
来源：http://hz.aibaodan.cn/gtaabpknzb.html

if let n = opt { print(n) }
来源：http://hz.shuidangran.top/gtfedqzdtj.html

[T20] Swift：数组操作
来源：http://hz.yanxiufei.cn/gtgbaceenp.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.shanyushiyangkeji.top/gtibegebxm.html

[T21] Swift：遍历
来源：http://hz.ppjwa.cn/gteokohfol.html

for x in a { print(x) }
来源：http://hz.ywan-chungtsiang.top/gtqzqzrfuq.html

[T22] Swift：字典
来源：http://hz.jianghu66.top/gtproflzad.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hnqzz.top/gtidrlgkhh.html

[T23] Swift：函数
来源：http://hz.hnqzz.top/gtrsikqqfq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.chenzaomai.com/gtwbsgvxjx.html

[T24] Swift：闭包
来源：http://hz.wangdashe.top/gtvtevxcif.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yangfankeji.com/gtdjqbkoow.html

[T25] Swift：结构体
来源：http://hz.yangfankeji.com/gtueucowwy.html

struct P { var x: Int }
来源：http://hz.sufxvd.cn/gtazefakkd.html

[T26] Swift：类与重写
来源：http://hz.xingfuxueyuan.xyz/gtshjxrupm.html

class A: Base { override func f() {} }
来源：http://hz.snrcjt.cn/gtcwgcfjmf.html

[T27] Swift：错误处理
来源：http://hz.shangyingyoupin.top/gtqtukmtni.html

do { try f() } catch { print(error) }
来源：http://hz.jianghu66.top/gtdooiokpn.html

[T28] Swift：枚举
来源：http://hz.aizwys.cn/gtejvpnnuy.html

enum Color { case red, green }
来源：http://hz.svipenyu.cn/gtbeczpkqp.html

[T29] Swift：guard 提前返回
来源：http://hz.ywan-chungtsiang.top/gthzzujbfi.html

guard let x = opt else { return }
来源：http://hz.sweek.top/gtzphhscjr.html

[T30] Swift：协议
来源：http://hz.zhiwuduotai.top/gtvzxzvigx.html

protocol Shape { func area() -> Double }
来源：http://hz.ydjk.org.cn/gtdcnofizj.html

[T31] Lua：Hello World
来源：http://hz.andypj.xyz/gtgqrpklyr.html

print("Hello")
来源：http://hz.ehwqpu.com/gtulzgkgar.html

[T32] Lua：局部变量
来源：http://hz.hywenlv.cn/gtfxiieobd.html

local a = 1
来源：http://hz.yj20258888.top/gtlipqaapg.html

[T33] Lua：表（数组）
来源：http://hz.guowangkeji.top/gtjdgwawjo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.ivvv.top/gtatzbdgrh.html

[T34] Lua：遍历表
来源：http://hz.jqgufenzy.top/gtvucisqae.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.hnxiangtu.top/gtayungxst.html

[T35] Lua：字典表
来源：http://hz.hnxiangtu.top/gtosqkhccj.html

local d = { a = 1 };  d.b = 2
来源：http://hz.ywan-chungtsiang.top/gtgbcdhzjk.html

[T36] Lua：函数
来源：http://hz.yueranfly.top/gtpvqcubsu.html

function add(a, b) return a + b end
来源：http://hz.gzhubu.top/gtlfdoswui.html

[T37] Lua：字符串拼接
来源：http://hz.shangyingyoupin.top/gtpkydnize.html

"a" .. "b"
来源：http://hz.jiagoushi.top/gtruiykwmg.html

[T38] Lua：条件
来源：http://hz.yueranfly.top/gtcnjuymlh.html

if x > 0 then print("正") end
来源：http://hz.hongshengwenyu.top/gtksahhzky.html

[T39] Lua：模式匹配
来源：http://hz.zhijiandao.cn/gtlifufocy.html

string.find(s, "%d+")
来源：http://hz.jiagoushi.top/gtwngqgibc.html

[T40] Lua：元表
来源：http://hz.yonumen.top/gtkpnqsnre.html

setmetatable({}, { __index = base })
来源：http://hz.fzhhl.top/gtelpspbyu.html

[T41] Perl：Hello World
来源：http://hz.chenjidiqi.icu/gtfzvuzjzd.html

print "Hello\n";
来源：http://hz.nanxinkj.top/gtbuilpgmp.html

[T42] Perl：变量类型
来源：http://hz.quarkkingdee.top/gtcuofanoa.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.shuidangran.top/gtbnxamrad.html

[T43] Perl：字符串插值
来源：http://hz.yj20258888.top/gtrikxjkbw.html

"值: $a"
来源：http://hz.andypj.xyz/gtxtepatni.html

[T44] Perl：条件
来源：http://hz.0kj1m.cn/gtyjcrwutq.html

if ($a > 0) { print "正"; }
来源：http://hz.dianchejie.cn/gtyymgoxdm.html

[T45] Perl：数组遍历
来源：http://hz.yanxiufei.cn/gtgekynvqf.html

for my $x (@arr) { print $x; }
来源：http://hz.jiagoushi.top/gtslusoyox.html

[T46] Perl：哈希操作
来源：http://hz.sweek.top/gttcotegmt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.hongshengwenyu.top/gtttgoqtuc.html

[T47] Perl：正则捕获
来源：http://hz.cqqwz.cn/gtnzcxypqb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.9152youxi.cn/gtmocpvzxq.html

[T48] Perl：正则替换
来源：http://hz.zhongyouzk.top/gtssepapfi.html

$s =~ s/old/new/g;
来源：http://hz.9152youxi.cn/gtqsfrmxyy.html

[T49] Perl：函数
来源：http://hz.ybcxt.top/gtixudfvym.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.shanyushiyangtech.top/gtdcnyngwi.html

[T50] Perl：逐行读文件
来源：http://hz.snrcjt.cn/gtvkfpwiev.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.chenlongwang.top/gtypbbxlvc.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.fzhhl.top/gtwxwecraq.html

[T51] Scala：Hello World
来源：http://hz.xinyue.icu/gtudsxsgkn.html

println("Hello")
来源：http://hz.jiagoushi.top/gtbjfphleh.html

[T52] Scala：变量
来源：http://hz.kuanghao11.cn/gtafucxbpw.html

val a = 1;  var b = 2
来源：http://hz.gaohongyu789.top/gtwgbdtfcy.html

[T53] Scala：字符串插值
来源：http://hz.cqqwz.cn/gtcmyxdfkt.html

s"值: $b"
来源：http://hz.yueranfly.top/gttyymfxhu.html

[T54] Scala：集合映射
来源：http://hz.jlsjyb.cn/gtpybcjlpg.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.dashuyun.cn/gthccogkcl.html

[T55] Scala：集合过滤
来源：http://hz.tanke756.top/gtajtiriru.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.andypj.xyz/gtbtpqkldu.html

[T56] Scala：样例类
来源：http://hz.jqgfzy.top/gtwhjjkplw.html

case class User(name: String, age: Int)
来源：http://hz.hysaishi.cn/gtwrzoykcs.html

[T57] Scala：模式匹配
来源：http://hz.ybcxt.top/gtbfrhaehw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.gotoacloud.top/gtgsvorsoj.html

[T58] Scala：函数定义
来源：http://hz.ydjk.org.cn/gtvperahpp.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.shanyushiyangkeji.top/gtfkyvxpzk.html

[T59] Scala：循环
来源：http://hz.bjfxy.top/gtaraqckkq.html

for (i <- 1 to 10) println(i)
来源：http://hz.chenlongwang.top/gtqvaevklc.html

[T60] Scala：折叠
来源：http://hz.fzhhl.top/gtlxouhyrk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yongpay.top/gtjcrxdzyy.html

================================================================================
来源：http://hz.ehwqpu.com/gthsxekbjf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.xziqi.cn/gteaeomhsa.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtxyjxjmdh.html

[U01] Py：创建虚拟环境
来源：http://hz.tanke756.top/gtjbtwkfad.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.xuetiantiany.cn/gtyvhifunr.html

[U02] Py：导出 / 安装依赖
来源：http://hz.nanxinkj.top/gtmlmgedzi.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.bjfxy.top/gtcedelphs.html

[U03] Py：加载 .env 配置
来源：http://hz.0kj1m.cn/gtzwefraai.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.cdnleiting.top/gtmgrevylh.html

[U04] Py：变量调试打印
来源：http://hz.xuetiantiany.cn/gtggrwhcby.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.tian-w.cn/gtzitkqnpj.html

[U05] Py：列表去重且保序
来源：http://hz.yj20258888.top/gtbphyeplr.html

list(dict.fromkeys(arr))
来源：http://hz.zhongyouzk.top/gtuiidvwde.html

[U06] Py：合并两个字典
来源：http://hz.xylfe.cn/gtmrrdzntg.html

{**a, **b}
来源：http://hz.pycfn.com/gtbhbjdvtz.html

[U07] Py：反转字典键值
来源：http://hz.yj20258.top/gtfranpdic.html

{v: k for k, v in d.items()}
来源：http://hz.ivvv.top/gthfyusdno.html

[U08] Py：展平二维列表
来源：http://hz.ydjk.org.cn/gtylbavhwx.html

[y for x in nested for y in x]
来源：http://hz.xylfe.cn/gtegfxddak.html

[U09] Py：字典取最大值的键
来源：http://hz.chenjidiqi.icu/gtgzsfqqcr.html

max(d, key=d.get)
来源：http://hz.sxryk.cn/gtmpxeicys.html

[U10] Py：按值排序字典
来源：http://hz.jyoumei.cn/gtgcnqcpxu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.ywan-chungtsiang.top/gtwcoogfdc.html

[U11] Py：生成器表达式
来源：http://hz.snrcjt.cn/gttbysyrts.html

(x * 2 for x in arr)
来源：http://hz.feifeiyinyue.top/gtalbeplps.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.nwbrower.top/gtoesbhpjz.html

Counter(arr).most_common(3)
来源：http://hz.zdqjudy.top/gtvpylqoci.html

[U13] Py：固定长度队列
来源：http://hz.shzxlz.cn/gtywpsqaiz.html

deque(maxlen=10)
来源：http://hz.jlsjyb.cn/gtdfuxjzds.html

[U14] Py：分组收集到列表
来源：http://hz.yangfankeji.com/gtvlgofgkf.html

defaultdict(list)
来源：http://hz.haohaochexian.top/gtyuzucjqx.html

[U15] Py：高精度计时
来源：http://hz.tanke756.top/gtmrgoltdd.html

t = time.perf_counter()
来源：http://hz.zycfv.cn/gtylrtrlli.html

[U16] Py：命令行参数解析
来源：http://hz.daxiang520.top/gtvixpgbrh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.zhijiandao.cn/gtoahlzdrv.html

[U17] Py：初始化日志
来源：http://hz.tianlin.xyz/gtfbukqdta.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.gaohongyu789.top/gtcwrgycho.html

[U18] Py：预编译正则
来源：http://hz.xuanzx.com/gtvkhmywaf.html

pat = re.compile(r"\d+")
来源：http://hz.jinqigufen.top/gtnvjmfknr.html

[U19] Py：正则替换带回调
来源：http://hz.yueranfly.top/gtbnztwvzs.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.daxiang520.top/gtizfctkly.html

[U20] Py：缓存函数结果
来源：http://hz.jinqigufen.top/gtasazjpvz.html

@functools.lru_cache(maxsize=None)
来源：http://hz.316326.xyz/gtuyfccmen.html

[U21] Py：自定义上下文管理器
来源：http://hz.feifeiyinyue.top/gtxizpmtpv.html

@contextlib.contextmanager
来源：http://hz.zhiwuduotai.top/gtfygczemr.html

[U22] Py：矩阵转置
来源：http://hz.svipenyu.cn/gtwbzacyel.html

list(zip(*m))
来源：http://hz.yvedp.cn/gtphlxblso.html

[U23] Py：分块读取大文件
来源：http://hz.zhaomingkeji.xyz/gtbquvaebx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.ppjwa.cn/gtlhnjdcjh.html

[U24] Py：路径操作
来源：http://hz.yvedp.cn/gtaksnlvqx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.hnxiangtu.top/gtljknzcqh.html


<!-- 参考信息 -->