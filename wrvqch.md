代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.gogol.net.cn/gtkstrirrz.html

[R80] 查看脚本执行耗时
来源：http://hz.gzhubu.top/gttmoygwru.html

time ./run.sh
来源：http://hz.daria6918.cn/gtewvators.html

================================================================================
来源：http://hz.sufxvd.cn/gtklklbbef.html

S. C / C++ 专题
来源：http://hz.havefunace.top/gtczrqwrcz.html

================================================================================
来源：http://hz.mhx1999.top/gtryefpotb.html

[S01] C：Hello World
来源：http://hz.yuxming.cn/gtikvhnkmj.html

#include <stdio.h>
来源：http://hz.jqgfzy.top/gtrzfjjedu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhijiandao.cn/gtfwycqgom.html

[S02] C：变量与格式化输出
来源：http://hz.xuetiantiany.cn/gtwepjpuej.html

int a = 10; printf("%d\n", a);
来源：http://hz.andypj.xyz/gtlraeihui.html

[S03] C：读入整数
来源：http://hz.yuxming.cn/gtlxbnkfce.html

int x; scanf("%d", &x);
来源：http://hz.guannengcc.top/gtxfgvqhde.html

[S04] C：字符串复制
来源：http://hz.quarkkingdee.top/gtesgwuiqx.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.chenjidiqi.icu/gtssjnmdap.html

[S05] C：字符串长度
来源：http://hz.tianlin.xyz/gtcgmtuczg.html

strlen(s)
来源：http://hz.fzhhl.top/gttaffijtc.html

[S06] C：字符串比较
来源：http://hz.iojbl.cn/gtvkacnujq.html

strcmp(a, b) == 0
来源：http://hz.mhx1999.top/gtbnrgopnh.html

[S07] C：数组遍历求和
来源：http://hz.jinqigufen.top/gtlzhkzekn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.guannengcc.top/gthyszogbq.html

[S08] C：动态内存分配与释放
来源：http://hz.ybcxt.top/gtmegzzwjq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.316326.xyz/gthiwiyrdf.html

[S09] C：结构体定义与初始化
来源：http://hz.nanxinkj.top/gtzjsqbhhf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.shanyushiyangkeji.top/gtmnoiiczo.html

[S10] C：指针与解引用
来源：http://hz.svipenyu.cn/gtxphnsyao.html

int *p = &a;  *p = 5;
来源：http://hz.316326.xyz/gtgurqncxg.html

[S11] C：逐行读文件
来源：http://hz.nanxuanxn.top/gthtxmvjmk.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhoulong.xyz/gtiisghxse.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hammf.cn/gtwsvighsf.html

fclose(f);
来源：http://hz.andypj.xyz/gtftkkeaxj.html

[S12] C：写文件
来源：http://hz.hammf.cn/gtmqsuzjpk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ywan-chungtsiang.top/gtdprbvgip.html

[S13] C：宏定义
来源：http://hz.shzxlz.cn/gtkhcsetms.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.wangshuangyany.cn/gtmynfhskl.html

[S14] C：枚举
来源：http://hz.snrcjt.cn/gtbyxycuxu.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.snrcjt.cn/gtcsrshwvi.html

[S15] C：类型转换
来源：http://hz.c1oappe.top/gtkabavcgd.html

(double) a / b
来源：http://hz.xziqi.cn/gtqlsixzgz.html

[S16] C：位操作置位
来源：http://hz.sxryk.cn/gtipfiojgy.html

x |= (1 << 3);
来源：http://hz.hywenlv.cn/gtalkhqdqq.html

[S17] C：安全拼接字符串
来源：http://hz.sufxvd.cn/gtjzbcquce.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.cheryme.top/gtrbdlppxa.html

[S18] C：命令行参数
来源：http://hz.chenzaomai.com/gtdzevxngi.html

int main(int argc, char **argv)
来源：http://hz.havefunace.top/gtlrlohrpv.html

[S19] C：快速排序
来源：http://hz.ehwqpu.com/gtczlvnnoz.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.mhx1999.top/gtdcmmfbrm.html

[S20] C：二分查找
来源：http://hz.ehwqpu.com/gtgyzoazfk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.xuetiantiany.cn/gtkloptvzn.html

[S21] C：字符类别判断
来源：http://hz.yj202588.top/gtkacuwaee.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xuanzx.com/gtqpdagsng.html

[S22] C：字符串转数字
来源：http://hz.dashuyun.cn/gtpprfrxha.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.quarkkingdee.top/gtmabgyfel.html

[S23] C：随机数
来源：http://hz.kuanghao11.cn/gtwnovzamu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.chenjidiqi.icu/gtjipwgrnu.html

[S24] C：获取本地时间
来源：http://hz.cashguo.top/gtqjgotrkl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ivvv.top/gtqjnwgpbg.html

[S25] C：内存拷贝
来源：http://hz.pengpengdd.cyou/gtidfktiqv.html

memcpy(dst, src, n);
来源：http://hz.0kj1m.cn/gtzwayglio.html

[S26] C：内存清零
来源：http://hz.nanxuanxn.top/gtihvebaiv.html

memset(a, 0, sizeof a);
来源：http://hz.xylfe.cn/gtvcngpudj.html

[S27] C：定义常量
来源：http://hz.cheryme.top/gtgbuytnsu.html

const double PI = 3.14159;
来源：http://hz.shzxlz.cn/gtigsbfnxt.html

[S28] C：静态变量
来源：http://hz.aizwys.cn/gtonlzjczp.html

static int counter = 0;
来源：http://hz.xuetiantiany.cn/gttzcbzwul.html

[S29] C：变参函数
来源：http://hz.gzhubu.top/gtgjiwcfsk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yj20258888.top/gtgwhdwrcq.html

[S30] C：头文件保护
来源：http://hz.jyoumei.cn/gtaspqpqma.html

#ifndef X_H
来源：http://hz.cqqwz.cn/gtgqciruqx.html

#define X_H
来源：http://hz.wangshuangyany.cn/gtpwdbrhst.html

#endif
来源：http://hz.snrcjt.cn/gtexoqdrhk.html

[S31] C++：Hello World
来源：http://hz.pycfn.com/gtwprvdult.html

#include <iostream>
来源：http://hz.hammf.cn/gtcakaqjre.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.iojbl.cn/gtnbzkiafw.html

[S32] C++：字符串
来源：http://hz.cheryme.top/gtsbwggtoq.html

std::string s = "hi";  s += "!";
来源：http://hz.chenzaomai.com/gtjvigksjc.html

[S33] C++：vector 增删
来源：http://hz.yueranfly.top/gtijirswcj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.tanke756.top/gtlmyeewlu.html

[S34] C++：遍历 vector
来源：http://hz.ppjwa.cn/gtjpfklxox.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhoulong.xyz/gtyxcmtzky.html

[S35] C++：map
来源：http://hz.havefunace.top/gtextufabr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hfpthk.cn/gtdtojzzim.html

[S36] C++：unordered_map
来源：http://hz.guannengcc.top/gtqdjooxfz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.aibaodan.cn/gtbdtqzjte.html

[S37] C++：set
来源：http://hz.guowangkeji.top/gtrlxxeiya.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.shangyingyoupin.top/gtylsrager.html

[S38] C++：排序
来源：http://hz.smart0.xyz/gthisfzcxp.html

std::sort(v.begin(), v.end());
来源：http://hz.cashguo.top/gtkadmicqk.html

[S39] C++：自定义比较器排序
来源：http://hz.gogol.net.cn/gtkwmgaddn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jlsjyb.cn/gtzzcgdwlb.html

[S40] C++：查找元素
来源：http://hz.iojbl.cn/gtjxycsuon.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.smart0.xyz/gtnbzwivhh.html

[S41] C++：类与构造函数
来源：http://hz.pengpengdd.cyou/gtcxpzpkbb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.tian-w.cn/gtexirwocf.html

[S42] C++：继承与虚函数
来源：http://hz.chenzaomai.com/gtxiokzemz.html

class B : public Base { public: void f() override {} };
来源：http://hz.hysaishi.cn/gtgweivyfe.html

[S43] C++：智能指针
来源：http://hz.9152youxi.cn/gtbzcajqcz.html

auto p = std::make_unique<int>(5);
来源：http://hz.tian-w.cn/gtxmeejsxx.html

[S44] C++：引用传参
来源：http://hz.ppjwa.cn/gtjsmrramq.html

void inc(int &x) { ++x; }
来源：http://hz.gotoacloud.top/gtplzauxoz.html

[S45] C++：lambda
来源：http://hz.meibo888.top/gtxclehdxm.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jinyuanbaomall.cn/gtorpkuwpk.html

[S46] C++：函数模板
来源：http://hz.0kj1m.cn/gtkudfmlmz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhoulong.xyz/gtzjfltwhp.html

[S47] C++：结构化绑定遍历
来源：http://hz.tianlin.xyz/gtyjsybqmz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ydjk.org.cn/gtywpzsoir.html

[S48] C++：逐行读文件
来源：http://hz.aibaodan.cn/gtwhfranol.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shzxlz.cn/gtjdgloctz.html

while (std::getline(in, line)) { }
来源：http://hz.jiagoushi.top/gtxpcbdhmk.html

[S49] C++：写文件
来源：http://hz.316326.xyz/gtvczzsshr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yuxming.cn/gtqjhjlykl.html

[S50] C++：格式化数字
来源：http://hz.pengpengdd.cyou/gtprrshlle.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zdqjudy.top/gtpybyujbc.html

[S51] C++：显式类型转换
来源：http://hz.ybcxt.top/gtrnpzwnpo.html

static_cast<double>(a) / b
来源：http://hz.zhengqikj.top/gthzyalomv.html

[S52] C++：const 与 noexcept
来源：http://hz.zdqjudy.top/gtasqaqeel.html

int size() const noexcept { return n_; }
来源：http://hz.zhaomingkeji.xyz/gtzzxutmqu.html

[S53] C++：移动语义
来源：http://hz.c1oappe.top/gtetehsmnv.html

std::vector<int> w = std::move(v);
来源：http://hz.daxiang520.top/gtsahrfotp.html

[S54] C++：异常处理
来源：http://hz.shanyushiyangkeji.top/gtwlzmsala.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.cashguo.top/gtqmevbmgp.html

[S55] C++：结构化绑定
来源：http://hz.ydzc1.top/gtyorhzrvn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.gzhubu.top/gtghoshfrf.html

[S56] C++：optional
来源：http://hz.andypj.xyz/gttqmorkkz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jianghu66.top/gtzqvpazrr.html

[S57] C++：编译期常量
来源：http://hz.quarkkingdee.top/gtokrxuxjl.html

constexpr int N = 10;
来源：http://hz.zdqjudy.top/gtwtwzjmhf.html

[S58] C++：命名空间
来源：http://hz.tian-w.cn/gtvtfpapqr.html

namespace ns { int f() { return 1; } }
来源：http://hz.yj20258888.top/gtoflzschd.html

[S59] C++：静态断言
来源：http://hz.zdqjudy.top/gtxcexrwos.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.kuanghao11.cn/gtmvnscrbk.html

[S60] C++：遍历并删除元素
来源：http://hz.tianlin.xyz/gticzwhqwd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.sufxvd.cn/gtcrilyjkc.html

================================================================================
来源：http://hz.cqqwz.cn/gtbofrtdne.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ydjk.org.cn/gtsduujvfi.html

================================================================================
来源：http://hz.yongpay.top/gtdkhonrxy.html

[T01] Kotlin：Hello World
来源：http://hz.zhoulong.xyz/gtbatvbpzd.html

println("Hello")
来源：http://hz.dianchejie.cn/gtnjjneqvu.html

[T02] Kotlin：变量
来源：http://hz.daxiang520.top/gtghqnyjie.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.chenjidiqi.icu/gtvqrwuewp.html

[T03] Kotlin：字符串模板
来源：http://hz.zhengqikj.top/gtioqxdsrs.html

"值: $b"
来源：http://hz.gotoacloud.top/gtxovolqbh.html

[T04] Kotlin：空安全
来源：http://hz.daria6918.cn/gtrpdqyylu.html

val n: String? = null;  n?.length
来源：http://hz.dashuyun.cn/gtdlgksmaz.html

[T05] Kotlin：when 表达式
来源：http://hz.cheryme.top/gtpwnxjwtx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.dashuyun.cn/gtsqpqmhhg.html

[T06] Kotlin：集合映射
来源：http://hz.ivvv.top/gtkkocaqai.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.dianchejie.cn/gtgpllbifc.html

[T07] Kotlin：集合过滤
来源：http://hz.jinyuanbaomall.cn/gtzdwdhwdr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yangfankeji.com/gtqytezdag.html

[T08] Kotlin：数据类
来源：http://hz.jiagoushi.top/gtmzsgpnei.html

data class User(val name: String, val age: Int)
来源：http://hz.jinghuilouyu.cn/gtnzjzluct.html

[T09] Kotlin：扩展函数
来源：http://hz.dashuyun.cn/gtubmhhqpz.html

fun String.exclaim() = this + "!"
来源：http://hz.yangfankeji.com/gtwnctzbla.html

[T10] Kotlin：默认参数
来源：http://hz.zhaomingkeji.xyz/gtmvibukpn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.tanke756.top/gtygpprdqs.html

[T11] Kotlin：协程
来源：http://hz.cdnleiting.top/gtqwnmppxl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.mhx1999.top/gtiqlqsdgv.html

[T12] Kotlin：解构声明
来源：http://hz.yangfankeji.com/gtvxkvztnw.html

val (a, b) = Pair(1, 2)
来源：http://hz.sxryk.cn/gtjkxjhifj.html

[T13] Kotlin：只读 Map
来源：http://hz.xziqi.cn/gtubzgecnl.html

val m = mapOf("a" to 1)
来源：http://hz.dashuyun.cn/gtgqmduzjz.html

[T14] Kotlin：循环
来源：http://hz.aibaodan.cn/gtccmtvicc.html

for (i in 1..10) println(i)
来源：http://hz.jinqigufen.top/gttmwqvzph.html

[T15] Kotlin：接口
来源：http://hz.yuanzhike.top/gtjercucxi.html

interface Shape { fun area(): Double }
来源：http://hz.redwolf501.top/gtpwinhkkc.html

[T16] Swift：Hello World
来源：http://hz.kuanghao11.cn/gtsgbdvwzr.html

print("Hello")
来源：http://hz.shanyushiyangkeji.top/gtxeqwxkef.html

[T17] Swift：变量与常量
来源：http://hz.feifeiyinyue.top/gtreurvsyc.html

var a = 1;  let b = 2
来源：http://hz.yongpay.top/gtlwmuyjyh.html

[T18] Swift：字符串插值
来源：http://hz.ehwqpu.com/gtvaivrmuc.html

"值: \(b)"
来源：http://hz.cdnleiting.top/gtpcmhwfnz.html

[T19] Swift：可选绑定
来源：http://hz.mhx1999.top/gtcjodtsti.html

if let n = opt { print(n) }
来源：http://hz.jqgufenzy.top/gtjcufiadz.html

[T20] Swift：数组操作
来源：http://hz.cqqwz.cn/gtdfpxudcy.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jinqigufen.top/gtotppfecm.html

[T21] Swift：遍历
来源：http://hz.jlsjyb.cn/gtkfxsevbn.html

for x in a { print(x) }
来源：http://hz.9152youxi.cn/gtfbvwwtms.html

[T22] Swift：字典
来源：http://hz.jlsjyb.cn/gtqkqmpfmt.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.52xcode.cn/gtkrvkwxug.html

[T23] Swift：函数
来源：http://hz.xziqi.cn/gtwfcfgbze.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.gotoacloud.top/gtofspjpyr.html

[T24] Swift：闭包
来源：http://hz.yonumen.top/gtoyvngepi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.316326.xyz/gtfpqktddz.html

[T25] Swift：结构体
来源：http://hz.yangfankeji.com/gtdxxdjwsq.html

struct P { var x: Int }
来源：http://hz.hammf.cn/gtqxgtbisa.html

[T26] Swift：类与重写
来源：http://hz.xuanzx.com/gtasumqaee.html

class A: Base { override func f() {} }
来源：http://hz.guannengcc.top/gtxrakyagi.html

[T27] Swift：错误处理
来源：http://hz.jlsjyb.cn/gtyvoetwwu.html

do { try f() } catch { print(error) }
来源：http://hz.xuetiantiany.cn/gtuklawvna.html

[T28] Swift：枚举
来源：http://hz.jlsjyb.cn/gtnubheseg.html

enum Color { case red, green }
来源：http://hz.jianghu66.top/gtbwrgweuq.html

[T29] Swift：guard 提前返回
来源：http://hz.xziqi.cn/gttmoqvmqj.html

guard let x = opt else { return }
来源：http://hz.jinyuanbaomall.cn/gtarfdqmcp.html

[T30] Swift：协议
来源：http://hz.fzhhl.top/gtaslxcjzx.html

protocol Shape { func area() -> Double }
来源：http://hz.yueranfly.top/gtpgvlnuti.html

[T31] Lua：Hello World
来源：http://hz.birdmap.top/gtdhwjeeyd.html

print("Hello")
来源：http://hz.sweek.top/gtzkljweft.html

[T32] Lua：局部变量
来源：http://hz.yangfankeji.com/gtjiqjnrpl.html

local a = 1
来源：http://hz.fengsongda.top/gtvfcpnwwb.html

[T33] Lua：表（数组）
来源：http://hz.shangyingyoupin.top/gtaxhnjwzg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.aizwys.cn/gtrwobtfjz.html

[T34] Lua：遍历表
来源：http://hz.gzhubu.top/gtlckwyxkz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.vqdsnc.cn/gtmcqdyqgp.html

[T35] Lua：字典表
来源：http://hz.snrcjt.cn/gticllhiwu.html

local d = { a = 1 };  d.b = 2
来源：http://hz.hywenlv.cn/gtzappsejo.html

[T36] Lua：函数
来源：http://hz.yvedp.cn/gtzxuleszh.html

function add(a, b) return a + b end
来源：http://hz.zhijiandao.cn/gtdtmaauzu.html

[T37] Lua：字符串拼接
来源：http://hz.pengpengdd.cyou/gtzqjaxcnw.html

"a" .. "b"
来源：http://hz.shanyushiyangtech.top/gtobvvbgdt.html

[T38] Lua：条件
来源：http://hz.zdqjudy.top/gtpocnmhuj.html

if x > 0 then print("正") end
来源：http://hz.jinqigufen.top/gtgkbcewzv.html

[T39] Lua：模式匹配
来源：http://hz.cqqwz.cn/gtkrxqpeyq.html

string.find(s, "%d+")
来源：http://hz.zycfv.cn/gtktypetkb.html

[T40] Lua：元表
来源：http://hz.daria6918.cn/gtutczzirc.html

setmetatable({}, { __index = base })
来源：http://hz.ybcxt.top/gtgwuynbgo.html

[T41] Perl：Hello World
来源：http://hz.cdnleiting.top/gtbywjchzj.html

print "Hello\n";
来源：http://hz.jyoumei.cn/gtjmawvvcg.html

[T42] Perl：变量类型
来源：http://hz.bjfxy.top/gtqhcvviwe.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.fengsongda.top/gtgabyebko.html

[T43] Perl：字符串插值
来源：http://hz.wangdashe.top/gtdgpyynye.html

"值: $a"
来源：http://hz.ivvv.top/gtijwoyxwn.html

[T44] Perl：条件
来源：http://hz.yuanzhike.top/gtxyhcrndl.html

if ($a > 0) { print "正"; }
来源：http://hz.birdmap.top/gtkksnzysf.html

[T45] Perl：数组遍历
来源：http://hz.tanke756.top/gtenfvfxfx.html

for my $x (@arr) { print $x; }
来源：http://hz.sysykeji.top/gtijakdhnp.html

[T46] Perl：哈希操作
来源：http://hz.sysykeji.top/gtehihhbgp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.tanke756.top/gtmlsggqwc.html

[T47] Perl：正则捕获
来源：http://hz.snrcjt.cn/gtacqdyomj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.andypj.xyz/gtwyyuqosv.html

[T48] Perl：正则替换
来源：http://hz.zhiwuduotai.top/gtpvoeoqqf.html

$s =~ s/old/new/g;
来源：http://hz.daria6918.cn/gtjovkijqo.html

[T49] Perl：函数
来源：http://hz.fzhhl.top/gtsqxpefpf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jinqigufen.top/gtgueqxery.html

[T50] Perl：逐行读文件
来源：http://hz.jqgfzy.top/gthbpwepth.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.haohaochexian.top/gtmzammfbp.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.pengpengdd.cyou/gtrlyqyjxw.html

[T51] Scala：Hello World
来源：http://hz.xuetiantiany.cn/gtmbbpiqnh.html

println("Hello")
来源：http://hz.nanxuanxn.top/gtrbfpnzte.html

[T52] Scala：变量
来源：http://hz.meibo888.top/gtsnrnupvm.html

val a = 1;  var b = 2
来源：http://hz.zhongyouzk.top/gteyhhgfax.html

[T53] Scala：字符串插值
来源：http://hz.tian-w.cn/gtqldegdfo.html

s"值: $b"
来源：http://hz.dianchejie.cn/gtdwahwccm.html

[T54] Scala：集合映射
来源：http://hz.gotoacloud.top/gtltfcvprl.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.ppjwa.cn/gteofegplx.html

[T55] Scala：集合过滤
来源：http://hz.vqdsnc.cn/gtbcumabob.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.ydzc1.top/gtonekvcgr.html

[T56] Scala：样例类
来源：http://hz.yongpay.top/gtugbjqkec.html

case class User(name: String, age: Int)
来源：http://hz.jinghuilouyu.cn/gtbtamhjeo.html

[T57] Scala：模式匹配
来源：http://hz.jianghu66.top/gtluyiordz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.gogol.net.cn/gtflexjsud.html

[T58] Scala：函数定义
来源：http://hz.hongshengwenyu.top/gtbgtlenic.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.ydjk.org.cn/gtjgiixxfg.html

[T59] Scala：循环
来源：http://hz.pengpengdd.cyou/gtcelbqvwk.html

for (i <- 1 to 10) println(i)
来源：http://hz.jqgufenzy.top/gtlyrgsnop.html

[T60] Scala：折叠
来源：http://hz.ehwqpu.com/gtviblphoc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.gaohongyu789.top/gtihcioopi.html

================================================================================
来源：http://hz.shuidangran.top/gtzskniclh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.tanke756.top/gtpvmcfuro.html

================================================================================
来源：http://hz.guowangkeji.top/gtdlrdsrpq.html

[U01] Py：创建虚拟环境
来源：http://hz.316326.xyz/gtprkmxmco.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.hnxiangtu.top/gtevabvsmo.html

[U02] Py：导出 / 安装依赖
来源：http://hz.zycfv.cn/gtshainulv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.0kj1m.cn/gtxmstxnin.html

[U03] Py：加载 .env 配置
来源：http://hz.316326.xyz/gteolecbae.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jianghu66.top/gtqzhkttdn.html

[U04] Py：变量调试打印
来源：http://hz.guowangkeji.top/gttwgyjpyz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.ywan-chungtsiang.top/gtgtxppamd.html

[U05] Py：列表去重且保序
来源：http://hz.zhiwuduotai.top/gtztkhcbds.html

list(dict.fromkeys(arr))
来源：http://hz.chenjidiqi.icu/gthgqqwivh.html

[U06] Py：合并两个字典
来源：http://hz.jinyuanbaomall.cn/gtjcxdhukx.html

{**a, **b}
来源：http://hz.wangdashe.top/gtvexrqhsr.html

[U07] Py：反转字典键值
来源：http://hz.gogol.net.cn/gtedxkoyzg.html

{v: k for k, v in d.items()}
来源：http://hz.hammf.cn/gthnwszapz.html

[U08] Py：展平二维列表
来源：http://hz.jinqigfzy.top/gtubjspldx.html

[y for x in nested for y in x]
来源：http://hz.sweek.top/gtlfttsnqs.html

[U09] Py：字典取最大值的键
来源：http://hz.snrcjt.cn/gtpzktxksk.html

max(d, key=d.get)
来源：http://hz.meibo888.top/gtptxkgidj.html

[U10] Py：按值排序字典
来源：http://hz.shzxlz.cn/gtmvkkknko.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.feifeiyinyue.top/gtogjhmqye.html

[U11] Py：生成器表达式
来源：http://hz.wangdashe.top/gthhwvpree.html

(x * 2 for x in arr)
来源：http://hz.yj202588.top/gtgknaogpn.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.xinyue.icu/gtpmxbmccm.html

Counter(arr).most_common(3)
来源：http://hz.zdqjudy.top/gtoqdxkcbz.html

[U13] Py：固定长度队列
来源：http://hz.shanyushiyangtech.top/gtrnzwzdzl.html

deque(maxlen=10)
来源：http://hz.yj202588.top/gtwvpaxfze.html

[U14] Py：分组收集到列表
来源：http://hz.yuanzhike.top/gthitaijud.html

defaultdict(list)
来源：http://hz.daria6918.cn/gtsscjsjex.html

[U15] Py：高精度计时
来源：http://hz.zhiwuduotai.top/gtoplcnbkl.html

t = time.perf_counter()
来源：http://hz.yj20258.top/gtijtfnjww.html

[U16] Py：命令行参数解析
来源：http://hz.jqgfzy.top/gtanwjwcpi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jlsjyb.cn/gteywpyaco.html

[U17] Py：初始化日志
来源：http://hz.jinqigufen.top/gtqworifgq.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.zhaomingkeji.xyz/gtyjbqxwtk.html

[U18] Py：预编译正则
来源：http://hz.yueranfly.top/gttlovmgqm.html

pat = re.compile(r"\d+")
来源：http://hz.zhengqikj.top/gtoydbxyte.html

[U19] Py：正则替换带回调
来源：http://hz.jinqigufen.top/gtlqhaadur.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.hammf.cn/gtvirwozav.html

[U20] Py：缓存函数结果
来源：http://hz.ybcxt.top/gtgpzrcjuv.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jinghuilouyu.cn/gthjepwtnu.html


<!-- 参考信息 -->