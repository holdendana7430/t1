代发 wailian999

S. C / C++ 专题
来源：http://hz.ppjwa.cn/gtbwvfksax.html

================================================================================
来源：http://hz.hysaishi.cn/gtqspxkxej.html

[S01] C：Hello World
来源：http://hz.jyoumei.cn/gtxhdfkcwp.html

#include <stdio.h>
来源：http://hz.shuidangran.top/gtoigtiroa.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.xingfuxueyuan.xyz/gtjrndhyjm.html

[S02] C：变量与格式化输出
来源：http://hz.xingfuxueyuan.xyz/gtnxeakbmt.html

int a = 10; printf("%d\n", a);
来源：http://hz.birdmap.top/gtvudvjbpa.html

[S03] C：读入整数
来源：http://hz.yj20258888.top/gtaxubbsfc.html

int x; scanf("%d", &x);
来源：http://hz.quarkkingdee.top/gtscvfwyrw.html

[S04] C：字符串复制
来源：http://hz.mhx1999.top/gtfyzzzmul.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.shanyushiyangtech.top/gtjbctdcfl.html

[S05] C：字符串长度
来源：http://hz.yanxiufei.cn/gteuertwkq.html

strlen(s)
来源：http://hz.zhiwuduotai.top/gtbcywevcp.html

[S06] C：字符串比较
来源：http://hz.smart0.xyz/gttjhwvehm.html

strcmp(a, b) == 0
来源：http://hz.sufxvd.cn/gtvqnzyjvb.html

[S07] C：数组遍历求和
来源：http://hz.ehwqpu.com/gtnwbrxsec.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hfpthk.cn/gtebjyxrok.html

[S08] C：动态内存分配与释放
来源：http://hz.aizwys.cn/gtecdrdbzj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yueranfly.top/gtzlnxxsaq.html

[S09] C：结构体定义与初始化
来源：http://hz.svipenyu.cn/gtwkvyaogo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jqgufenzy.top/gtfvvpyeje.html

[S10] C：指针与解引用
来源：http://hz.zycfv.cn/gtnmvbytaa.html

int *p = &a;  *p = 5;
来源：http://hz.zhoulong.xyz/gtgleafnms.html

[S11] C：逐行读文件
来源：http://hz.cqqwz.cn/gttwbexbiw.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.cucudq.cn/gtmpxozupk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hysaishi.cn/gthqvsipcn.html

fclose(f);
来源：http://hz.zhixingplan.top/gtztabekso.html

[S12] C：写文件
来源：http://hz.dianchejie.cn/gtyyexfokt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jqgfzy.top/gtjmixmsgn.html

[S13] C：宏定义
来源：http://hz.yvedp.cn/gtpbbxuqmq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.sxryk.cn/gtspudkvbm.html

[S14] C：枚举
来源：http://hz.redwolf501.top/gtddfbcjmr.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.aibaodan.cn/gtgnerjijw.html

[S15] C：类型转换
来源：http://hz.tianlin.xyz/gtajopiqob.html

(double) a / b
来源：http://hz.haohaochexian.top/gtbhphgdza.html

[S16] C：位操作置位
来源：http://hz.iojbl.cn/gtmioaxgaw.html

x |= (1 << 3);
来源：http://hz.ehwqpu.com/gtshcskhiv.html

[S17] C：安全拼接字符串
来源：http://hz.chenzaomai.com/gtxxuklcyn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.pycfn.com/gtknlrrful.html

[S18] C：命令行参数
来源：http://hz.cdnleiting.top/gtxfaisaim.html

int main(int argc, char **argv)
来源：http://hz.hnqzz.top/gtaomcrzbw.html

[S19] C：快速排序
来源：http://hz.vqdsnc.cn/gtilqxwvxn.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zhongyouzk.top/gtzlkjyyuv.html

[S20] C：二分查找
来源：http://hz.dianchejie.cn/gtxkdtzvbu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.cucudq.cn/gttqyagobu.html

[S21] C：字符类别判断
来源：http://hz.xziqi.cn/gtfcdysnav.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.chenjidiqi.icu/gtfbydpnmr.html

[S22] C：字符串转数字
来源：http://hz.ydjk.org.cn/gtrzfnkjwa.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ivvv.top/gtpmxywefc.html

[S23] C：随机数
来源：http://hz.0kj1m.cn/gtfgsasfzd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yangfankeji.com/gthqwfscce.html

[S24] C：获取本地时间
来源：http://hz.shanyushiyangkeji.top/gtlqhbdgbu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.c1oappe.top/gtjcvywfcg.html

[S25] C：内存拷贝
来源：http://hz.gotoacloud.top/gtmqzgbkok.html

memcpy(dst, src, n);
来源：http://hz.shanyushiyangtech.top/gtijdeoomd.html

[S26] C：内存清零
来源：http://hz.tianlin.xyz/gtsoiwhprl.html

memset(a, 0, sizeof a);
来源：http://hz.cqqwz.cn/gtoshjecmq.html

[S27] C：定义常量
来源：http://hz.316326.xyz/gtybkzdoyo.html

const double PI = 3.14159;
来源：http://hz.xylfe.cn/gtnnczgqbl.html

[S28] C：静态变量
来源：http://hz.hongshengwenyu.top/gtibsprgmb.html

static int counter = 0;
来源：http://hz.shzxlz.cn/gtufzypacq.html

[S29] C：变参函数
来源：http://hz.yj202588.top/gtqfqrnxcy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jinyuanbaomall.cn/gtjrhtncha.html

[S30] C：头文件保护
来源：http://hz.zhijiandao.cn/gtpchornft.html

#ifndef X_H
来源：http://hz.bjfxy.top/gtblfothbl.html

#define X_H
来源：http://hz.vqdsnc.cn/gtbomchhjs.html

#endif
来源：http://hz.hfpthk.cn/gtymgtykfc.html

[S31] C++：Hello World
来源：http://hz.nanxinkj.top/gtlobfojym.html

#include <iostream>
来源：http://hz.sysykeji.top/gtwosltoad.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zhixingplan.top/gtwfpkxara.html

[S32] C++：字符串
来源：http://hz.yongpay.top/gtegurgcda.html

std::string s = "hi";  s += "!";
来源：http://hz.shuidangran.top/gtrdnpjutp.html

[S33] C++：vector 增删
来源：http://hz.yj20258.top/gtwvhulgnn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shangyingyoupin.top/gtfrbniufk.html

[S34] C++：遍历 vector
来源：http://hz.nanxinkj.top/gtkudziuze.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.0kj1m.cn/gtjpcfhski.html

[S35] C++：map
来源：http://hz.snrcjt.cn/gtqyqjgukv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.c1oappe.top/gtaojmyefj.html

[S36] C++：unordered_map
来源：http://hz.cheryme.top/gtecgkziwa.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cheryme.top/gtkxnfjvru.html

[S37] C++：set
来源：http://hz.mhx1999.top/gtdebabvda.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.cheryme.top/gtnwamiuye.html

[S38] C++：排序
来源：http://hz.ydjk.org.cn/gtqnojjgqk.html

std::sort(v.begin(), v.end());
来源：http://hz.yj20258.top/gtmfvzywak.html

[S39] C++：自定义比较器排序
来源：http://hz.sysykeji.top/gtjvkbvxqm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.cqqwz.cn/gtnmohfnry.html

[S40] C++：查找元素
来源：http://hz.c1oappe.top/gtckacnici.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.meibo888.top/gtcmifaaob.html

[S41] C++：类与构造函数
来源：http://hz.smart0.xyz/gtdlvmwxta.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.chenjidiqi.icu/gtcumeywcz.html

[S42] C++：继承与虚函数
来源：http://hz.havefunace.top/gtkdvbobur.html

class B : public Base { public: void f() override {} };
来源：http://hz.sysykeji.top/gtobpbypre.html

[S43] C++：智能指针
来源：http://hz.jqgufenzy.top/gttyglvjgt.html

auto p = std::make_unique<int>(5);
来源：http://hz.ppjwa.cn/gtenrsenva.html

[S44] C++：引用传参
来源：http://hz.xinyue.icu/gtwoygpnnf.html

void inc(int &x) { ++x; }
来源：http://hz.sufxvd.cn/gtjldordjw.html

[S45] C++：lambda
来源：http://hz.hywenlv.cn/gttrdxrikg.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cucudq.cn/gthedvxbjn.html

[S46] C++：函数模板
来源：http://hz.nanxinkj.top/gtctlltnvm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ydjk.org.cn/gtwtxlqxat.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhongyouzk.top/gtcqtkdzcb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ywan-chungtsiang.top/gtghcjwapg.html

[S48] C++：逐行读文件
来源：http://hz.fengsongda.top/gtfpsdkjvf.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jinghuilouyu.cn/gtrqfmazdm.html

while (std::getline(in, line)) { }
来源：http://hz.wangshuangyany.cn/gtqsfsojlk.html

[S49] C++：写文件
来源：http://hz.fengsongda.top/gtgaebpahg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.gotoacloud.top/gtydprisze.html

[S50] C++：格式化数字
来源：http://hz.316326.xyz/gtvrlmhxpx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hammf.cn/gturfneuga.html

[S51] C++：显式类型转换
来源：http://hz.smart0.xyz/gtfufuaskf.html

static_cast<double>(a) / b
来源：http://hz.zhijiandao.cn/gtnwckkamq.html

[S52] C++：const 与 noexcept
来源：http://hz.ivvv.top/gtxytcbhsj.html

int size() const noexcept { return n_; }
来源：http://hz.feifeiyinyue.top/gtilvknadp.html

[S53] C++：移动语义
来源：http://hz.yongpay.top/gthkuvaxxq.html

std::vector<int> w = std::move(v);
来源：http://hz.guannengcc.top/gtxidvjldh.html

[S54] C++：异常处理
来源：http://hz.mhx1999.top/gtrpehvfix.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hongshengwenyu.top/gtqwfgtath.html

[S55] C++：结构化绑定
来源：http://hz.yongpay.top/gtcbupyius.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yj20258888.top/gtlitxkcix.html

[S56] C++：optional
来源：http://hz.gzhubu.top/gttjyhktbj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.daria6918.cn/gtjnrdjwoo.html

[S57] C++：编译期常量
来源：http://hz.cucudq.cn/gtltqrgmas.html

constexpr int N = 10;
来源：http://hz.yj20258.top/gtgbevsvxo.html

[S58] C++：命名空间
来源：http://hz.hnxiangtu.top/gtlnjlhrsq.html

namespace ns { int f() { return 1; } }
来源：http://hz.nwbrower.top/gtockcfwgb.html

[S59] C++：静态断言
来源：http://hz.xinyue.icu/gtnkuahxfx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.andypj.xyz/gtujlamxcf.html

[S60] C++：遍历并删除元素
来源：http://hz.ydjk.org.cn/gtxtqytdbb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.dianchejie.cn/gtkjniuxhc.html

================================================================================
来源：http://hz.yj20258888.top/gthrnuioav.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.dashuyun.cn/gtbnyifdzr.html

================================================================================
来源：http://hz.ivvv.top/gthjcvktbc.html

[T01] Kotlin：Hello World
来源：http://hz.yj20258888.top/gtwvyzmuqq.html

println("Hello")
来源：http://hz.aizwys.cn/gtcpsehxah.html

[T02] Kotlin：变量
来源：http://hz.xuetiantiany.cn/gtrqsfduiy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.shuidangran.top/gtmolmiwig.html

[T03] Kotlin：字符串模板
来源：http://hz.gogol.net.cn/gtsmmzzefq.html

"值: $b"
来源：http://hz.shangyingyoupin.top/gtmsufxcgd.html

[T04] Kotlin：空安全
来源：http://hz.feifeiyinyue.top/gtlkuzhmho.html

val n: String? = null;  n?.length
来源：http://hz.ydzc1.top/gtkesugskd.html

[T05] Kotlin：when 表达式
来源：http://hz.hongshengwenyu.top/gtmayjguem.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.tanke756.top/gthqrpjnen.html

[T06] Kotlin：集合映射
来源：http://hz.zdqjudy.top/gtasnftfdr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.meibo888.top/gtuahgsfju.html

[T07] Kotlin：集合过滤
来源：http://hz.meibo888.top/gtercgewaq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jinqigufen.top/gtmepsqxyc.html

[T08] Kotlin：数据类
来源：http://hz.fzhhl.top/gtwktqedyj.html

data class User(val name: String, val age: Int)
来源：http://hz.havefunace.top/gtkuxiptgj.html

[T09] Kotlin：扩展函数
来源：http://hz.aizwys.cn/gtsikifycg.html

fun String.exclaim() = this + "!"
来源：http://hz.sufxvd.cn/gtjpszpewa.html

[T10] Kotlin：默认参数
来源：http://hz.chenjidiqi.icu/gtuqbxvlwr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.gaohongyu789.top/gtciftpfyr.html

[T11] Kotlin：协程
来源：http://hz.daria6918.cn/gtijhhkhhl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.iojbl.cn/gtezektrwj.html

[T12] Kotlin：解构声明
来源：http://hz.vqdsnc.cn/gtublornxg.html

val (a, b) = Pair(1, 2)
来源：http://hz.gotoacloud.top/gtvmanwkmc.html

[T13] Kotlin：只读 Map
来源：http://hz.yvedp.cn/gtpejjtyqa.html

val m = mapOf("a" to 1)
来源：http://hz.yongpay.top/gtjddgdgtu.html

[T14] Kotlin：循环
来源：http://hz.chenzaomai.com/gtoqynhmub.html

for (i in 1..10) println(i)
来源：http://hz.shzxlz.cn/gtdoeshzef.html

[T15] Kotlin：接口
来源：http://hz.mhx1999.top/gtrklnvcfu.html

interface Shape { fun area(): Double }
来源：http://hz.sxryk.cn/gtrcerszca.html

[T16] Swift：Hello World
来源：http://hz.iojbl.cn/gtlinwznzl.html

print("Hello")
来源：http://hz.yueranfly.top/gtgrmgimhu.html

[T17] Swift：变量与常量
来源：http://hz.ehwqpu.com/gtdvhzzruo.html

var a = 1;  let b = 2
来源：http://hz.cdnleiting.top/gtfkixqmev.html

[T18] Swift：字符串插值
来源：http://hz.shanyushiyangkeji.top/gtxqnbxars.html

"值: \(b)"
来源：http://hz.jqgufenzy.top/gtwridcfdc.html

[T19] Swift：可选绑定
来源：http://hz.jinqigfzy.top/gthjyagehd.html

if let n = opt { print(n) }
来源：http://hz.sweek.top/gtfxywdwis.html

[T20] Swift：数组操作
来源：http://hz.9152youxi.cn/gtswhwctfo.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.xylfe.cn/gtpchxblcz.html

[T21] Swift：遍历
来源：http://hz.52xcode.cn/gtdydwhjig.html

for x in a { print(x) }
来源：http://hz.yangfankeji.com/gttchlejoj.html

[T22] Swift：字典
来源：http://hz.cdnleiting.top/gthngsuwij.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ydjk.org.cn/gtenpcencc.html

[T23] Swift：函数
来源：http://hz.xinyue.icu/gtbvjnxkxw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.chenlongwang.top/gtnantgtpq.html

[T24] Swift：闭包
来源：http://hz.guowangkeji.top/gtqcaudgkj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.gogol.net.cn/gtcwezxmyt.html

[T25] Swift：结构体
来源：http://hz.c1oappe.top/gtwrbuxmqw.html

struct P { var x: Int }
来源：http://hz.birdmap.top/gtofzimaho.html

[T26] Swift：类与重写
来源：http://hz.smart0.xyz/gttcjzyqbl.html

class A: Base { override func f() {} }
来源：http://hz.zhijiandao.cn/gtppvabwtf.html

[T27] Swift：错误处理
来源：http://hz.yueranfly.top/gtutsqkzqa.html

do { try f() } catch { print(error) }
来源：http://hz.shanyushiyangtech.top/gtmcmbdgia.html

[T28] Swift：枚举
来源：http://hz.pycfn.com/gteqquddcb.html

enum Color { case red, green }
来源：http://hz.yvedp.cn/gtktzaotqx.html

[T29] Swift：guard 提前返回
来源：http://hz.bjfxy.top/gtdlvmdepf.html

guard let x = opt else { return }
来源：http://hz.shzxlz.cn/gtrkklgwri.html

[T30] Swift：协议
来源：http://hz.zdqjudy.top/gthavbgalt.html

protocol Shape { func area() -> Double }
来源：http://hz.xuetiantiany.cn/gtxmvgdrki.html

[T31] Lua：Hello World
来源：http://hz.kuanghao11.cn/gtttigulaj.html

print("Hello")
来源：http://hz.ybcxt.top/gtcemchbae.html

[T32] Lua：局部变量
来源：http://hz.jinqigufen.top/gtgmkdoqxy.html

local a = 1
来源：http://hz.sufxvd.cn/gtjnqplhdw.html

[T33] Lua：表（数组）
来源：http://hz.c1oappe.top/gtliplffwf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.cqqwz.cn/gtzkljvsey.html

[T34] Lua：遍历表
来源：http://hz.zhongyouzk.top/gtgepzypjv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.nanxuanxn.top/gtggmgiigb.html

[T35] Lua：字典表
来源：http://hz.iojbl.cn/gtwknxomsz.html

local d = { a = 1 };  d.b = 2
来源：http://hz.shanyushiyangkeji.top/gtirgvabqi.html

[T36] Lua：函数
来源：http://hz.ybcxt.top/gtjkxmvfdb.html

function add(a, b) return a + b end
来源：http://hz.jinqigufen.top/gtevbvombl.html

[T37] Lua：字符串拼接
来源：http://hz.kuanghao11.cn/gtlijvbbnf.html

"a" .. "b"
来源：http://hz.snrcjt.cn/gtoqztlxbr.html

[T38] Lua：条件
来源：http://hz.chenzaomai.com/gtxqtmzkiz.html

if x > 0 then print("正") end
来源：http://hz.316326.xyz/gtejbyvicc.html

[T39] Lua：模式匹配
来源：http://hz.havefunace.top/gtoyuahcjw.html

string.find(s, "%d+")
来源：http://hz.hywenlv.cn/gtwctkbxly.html

[T40] Lua：元表
来源：http://hz.hysaishi.cn/gtlxyvhwgq.html

setmetatable({}, { __index = base })
来源：http://hz.pycfn.com/gtwwbciygf.html

[T41] Perl：Hello World
来源：http://hz.yanxiufei.cn/gtujjgottt.html

print "Hello\n";
来源：http://hz.andypj.xyz/gtunteugdx.html

[T42] Perl：变量类型
来源：http://hz.ywan-chungtsiang.top/gttfzfmrxy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zhongyouzk.top/gtsyyuvztv.html

[T43] Perl：字符串插值
来源：http://hz.zhijiandao.cn/gtzjdviope.html

"值: $a"
来源：http://hz.gaohongyu789.top/gtchzlhldi.html

[T44] Perl：条件
来源：http://hz.gzhubu.top/gtsdvdnyxk.html

if ($a > 0) { print "正"; }
来源：http://hz.aizwys.cn/gtvlrormat.html

[T45] Perl：数组遍历
来源：http://hz.316326.xyz/gtvwtrfksv.html

for my $x (@arr) { print $x; }
来源：http://hz.sxryk.cn/gtnlbkwmtq.html

[T46] Perl：哈希操作
来源：http://hz.sysykeji.top/gtgbobdscy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.feifeiyinyue.top/gtoxnpijmt.html

[T47] Perl：正则捕获
来源：http://hz.yueranfly.top/gtsftsmcxe.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.hnxiangtu.top/gtkfctesge.html

[T48] Perl：正则替换
来源：http://hz.xuetiantiany.cn/gtcueaevbg.html

$s =~ s/old/new/g;
来源：http://hz.yonumen.top/gtxcyrpyur.html

[T49] Perl：函数
来源：http://hz.yj20258888.top/gtgtnczoap.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.dianchejie.cn/gtkyvgfjsi.html

[T50] Perl：逐行读文件
来源：http://hz.nanxinkj.top/gtumipkrwy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.meibo888.top/gtmmynxcvt.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.havefunace.top/gtbvflswpa.html

[T51] Scala：Hello World
来源：http://hz.tian-w.cn/gtxtaflzbz.html

println("Hello")
来源：http://hz.havefunace.top/gtiqaougyv.html

[T52] Scala：变量
来源：http://hz.shangyingyoupin.top/gteagfgxsu.html

val a = 1;  var b = 2
来源：http://hz.zhixingplan.top/gttaodivsh.html

[T53] Scala：字符串插值
来源：http://hz.hammf.cn/gtnbnughmh.html

s"值: $b"
来源：http://hz.aizwys.cn/gtifyukdkn.html

[T54] Scala：集合映射
来源：http://hz.zhixingplan.top/gtikhldoag.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.daria6918.cn/gtkayfszjf.html

[T55] Scala：集合过滤
来源：http://hz.cashguo.top/gtfizcsrbj.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.gzhubu.top/gtiuruqdaa.html

[T56] Scala：样例类
来源：http://hz.zhengqikj.top/gtbnrjziml.html

case class User(name: String, age: Int)
来源：http://hz.zhixingplan.top/gtjwubtgcp.html

[T57] Scala：模式匹配
来源：http://hz.yangfankeji.com/gtjdytmpel.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.yangfankeji.com/gtvamnlgor.html

[T58] Scala：函数定义
来源：http://hz.316326.xyz/gtgmjbgiko.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.wangdashe.top/gtembcwyal.html

[T59] Scala：循环
来源：http://hz.fengsongda.top/gtcfuteciu.html

for (i <- 1 to 10) println(i)
来源：http://hz.shangyingyoupin.top/gtwqenochr.html

[T60] Scala：折叠
来源：http://hz.yj20258.top/gtiulffikr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.ywan-chungtsiang.top/gtfuzcjugu.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtydytjusu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.gogol.net.cn/gtgtzeqmoa.html

================================================================================
来源：http://hz.gaohongyu789.top/gtyppnsycj.html

[U01] Py：创建虚拟环境
来源：http://hz.shanyushiyangkeji.top/gttnidxred.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.tian-w.cn/gtpyeyzham.html

[U02] Py：导出 / 安装依赖
来源：http://hz.meibo888.top/gthopretjo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.zhengqikj.top/gtdwijiggq.html

[U03] Py：加载 .env 配置
来源：http://hz.zhaomingkeji.xyz/gtccxuqizj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yueranfly.top/gtycewbaqz.html

[U04] Py：变量调试打印
来源：http://hz.svipenyu.cn/gtxbaiqrue.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yangfankeji.com/gtqqkflrdc.html

[U05] Py：列表去重且保序
来源：http://hz.ivvv.top/gtuhwssfez.html

list(dict.fromkeys(arr))
来源：http://hz.smart0.xyz/gtzvwgwdhp.html

[U06] Py：合并两个字典
来源：http://hz.tanke756.top/gtqpzhhzlg.html

{**a, **b}
来源：http://hz.hammf.cn/gthvwfsknq.html

[U07] Py：反转字典键值
来源：http://hz.wangdashe.top/gtbzybdqof.html

{v: k for k, v in d.items()}
来源：http://hz.xingfuxueyuan.xyz/gtrlkognvf.html

[U08] Py：展平二维列表
来源：http://hz.yonumen.top/gtjicxfvgo.html

[y for x in nested for y in x]
来源：http://hz.ydjk.org.cn/gtgxxatqjv.html

[U09] Py：字典取最大值的键
来源：http://hz.ybcxt.top/gtsqsfrbsv.html

max(d, key=d.get)
来源：http://hz.xylfe.cn/gtzulhyazx.html

[U10] Py：按值排序字典
来源：http://hz.shangyingyoupin.top/gtjegnhrjs.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.jlsjyb.cn/gtoenvrxfa.html

[U11] Py：生成器表达式
来源：http://hz.xinyue.icu/gtdzqglejl.html

(x * 2 for x in arr)
来源：http://hz.aibaodan.cn/gtpruxpfmv.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yvedp.cn/gtukhbufkv.html

Counter(arr).most_common(3)
来源：http://hz.jinqigufen.top/gtftxmzblr.html

[U13] Py：固定长度队列
来源：http://hz.ydjk.org.cn/gtmevvfwee.html

deque(maxlen=10)
来源：http://hz.jinghuilouyu.cn/gtjswcixcz.html

[U14] Py：分组收集到列表
来源：http://hz.cqqwz.cn/gtqwwmsjhc.html

defaultdict(list)
来源：http://hz.havefunace.top/gtuiekpoei.html

[U15] Py：高精度计时
来源：http://hz.sysykeji.top/gtnjggmtvj.html

t = time.perf_counter()
来源：http://hz.ywan-chungtsiang.top/gtmihjfven.html

[U16] Py：命令行参数解析
来源：http://hz.nwbrower.top/gtvoahmwoe.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yanxiufei.cn/gtjzmzjncr.html

[U17] Py：初始化日志
来源：http://hz.yuxming.cn/gtmccfqwwm.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.nwbrower.top/gtryjcrpgm.html

[U18] Py：预编译正则
来源：http://hz.aizwys.cn/gtzfgcpres.html

pat = re.compile(r"\d+")
来源：http://hz.tian-w.cn/gthzmstgqa.html

[U19] Py：正则替换带回调
来源：http://hz.ppjwa.cn/gtalxrkrwz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.xuanzx.com/gtapiouvdv.html

[U20] Py：缓存函数结果
来源：http://hz.ydjk.org.cn/gtdlmlqnjz.html

@functools.lru_cache(maxsize=None)
来源：http://hz.snrcjt.cn/gtckyygtwm.html

[U21] Py：自定义上下文管理器
来源：http://hz.hnqzz.top/gttaiazxxa.html

@contextlib.contextmanager
来源：http://hz.dashuyun.cn/gtrqfgjlgd.html

[U22] Py：矩阵转置
来源：http://hz.xinyue.icu/gtpxdrordr.html

list(zip(*m))
来源：http://hz.316326.xyz/gtiqkcuskp.html


<!-- 参考信息 -->