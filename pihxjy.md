代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jqgufenzy.top/gtwyybvhua.html

[S02] C：变量与格式化输出
来源：http://hz.sweek.top/gtpochesat.html

int a = 10; printf("%d\n", a);
来源：http://hz.hysaishi.cn/gtkrwunbqy.html

[S03] C：读入整数
来源：http://hz.mhx1999.top/gtgnichuem.html

int x; scanf("%d", &x);
来源：http://hz.zhixingplan.top/gteelqqfpr.html

[S04] C：字符串复制
来源：http://hz.iojbl.cn/gtxmscjvgg.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.shangyingyoupin.top/gtaunzfulb.html

[S05] C：字符串长度
来源：http://hz.daxiang520.top/gtkhzwwdzx.html

strlen(s)
来源：http://hz.xinyue.icu/gtaivexagw.html

[S06] C：字符串比较
来源：http://hz.xziqi.cn/gtxhrmvnoz.html

strcmp(a, b) == 0
来源：http://hz.andypj.xyz/gtsukkilwu.html

[S07] C：数组遍历求和
来源：http://hz.yuanzhike.top/gtbmrxxqpq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xylfe.cn/gthixytgio.html

[S08] C：动态内存分配与释放
来源：http://hz.9152youxi.cn/gtxbryxuxq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zycfv.cn/gtipexdvat.html

[S09] C：结构体定义与初始化
来源：http://hz.cdnleiting.top/gtzwxydisu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ppjwa.cn/gtntkuwulg.html

[S10] C：指针与解引用
来源：http://hz.zhixingplan.top/gtmjltfvyw.html

int *p = &a;  *p = 5;
来源：http://hz.shuidangran.top/gtemxgsttn.html

[S11] C：逐行读文件
来源：http://hz.xylfe.cn/gtzughfeiu.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.quarkkingdee.top/gtipjczzpx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.gogol.net.cn/gtejapxvim.html

fclose(f);
来源：http://hz.tianlin.xyz/gtpfzdcywi.html

[S12] C：写文件
来源：http://hz.vqdsnc.cn/gtkfakgggo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.birdmap.top/gtorfswufo.html

[S13] C：宏定义
来源：http://hz.daxiang520.top/gtajswcpgm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.shuidangran.top/gtascsglzl.html

[S14] C：枚举
来源：http://hz.haohaochexian.top/gtowpdmykz.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhengqikj.top/gtdshthnrh.html

[S15] C：类型转换
来源：http://hz.jianghu66.top/gtosoypxxk.html

(double) a / b
来源：http://hz.xylfe.cn/gtuwygysax.html

[S16] C：位操作置位
来源：http://hz.ydjk.org.cn/gtaywyfuew.html

x |= (1 << 3);
来源：http://hz.wangdashe.top/gtuxwwfhld.html

[S17] C：安全拼接字符串
来源：http://hz.sweek.top/gtqpqbfhls.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhiwuduotai.top/gtceutfdkm.html

[S18] C：命令行参数
来源：http://hz.316326.xyz/gtixxtnjtj.html

int main(int argc, char **argv)
来源：http://hz.ppjwa.cn/gtnhktorvm.html

[S19] C：快速排序
来源：http://hz.snrcjt.cn/gthxvjhrwa.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jyoumei.cn/gtighapmyy.html

[S20] C：二分查找
来源：http://hz.jinghuilouyu.cn/gtjfmvusjs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.redwolf501.top/gtcflisldn.html

[S21] C：字符类别判断
来源：http://hz.redwolf501.top/gttkiyzatu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.sxryk.cn/gtblhtehaq.html

[S22] C：字符串转数字
来源：http://hz.c1oappe.top/gtogsqtxvt.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ehwqpu.com/gtgnxjetdd.html

[S23] C：随机数
来源：http://hz.yanxiufei.cn/gtnlzsncox.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yj20258.top/gtxtxstvct.html

[S24] C：获取本地时间
来源：http://hz.xinyue.icu/gtqsfwjkbs.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.52xcode.cn/gtltbzidhe.html

[S25] C：内存拷贝
来源：http://hz.jianghu66.top/gteqxapuin.html

memcpy(dst, src, n);
来源：http://hz.fzhhl.top/gtqligqxbv.html

[S26] C：内存清零
来源：http://hz.shanyushiyangtech.top/gtrhbdeldt.html

memset(a, 0, sizeof a);
来源：http://hz.hywenlv.cn/gtxppafwoj.html

[S27] C：定义常量
来源：http://hz.sufxvd.cn/gtzcoqscsp.html

const double PI = 3.14159;
来源：http://hz.52xcode.cn/gtixvwjwme.html

[S28] C：静态变量
来源：http://hz.xinyue.icu/gtvfyshdek.html

static int counter = 0;
来源：http://hz.shzxlz.cn/gtuxvqwilp.html

[S29] C：变参函数
来源：http://hz.havefunace.top/gtgmlejqpq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hammf.cn/gtbzskslcl.html

[S30] C：头文件保护
来源：http://hz.tanke756.top/gtupbmcixq.html

#ifndef X_H
来源：http://hz.nanxuanxn.top/gtfskfxxfn.html

#define X_H
来源：http://hz.redwolf501.top/gtinryalns.html

#endif
来源：http://hz.cucudq.cn/gtqexzlnkr.html

[S31] C++：Hello World
来源：http://hz.cqqwz.cn/gtbfqfsctk.html

#include <iostream>
来源：http://hz.smart0.xyz/gtcjnupmcr.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.shzxlz.cn/gtindrsdcx.html

[S32] C++：字符串
来源：http://hz.bjfxy.top/gtzzitzfcl.html

std::string s = "hi";  s += "!";
来源：http://hz.daria6918.cn/gthaywcjvb.html

[S33] C++：vector 增删
来源：http://hz.svipenyu.cn/gtpwuevpnu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.haohaochexian.top/gtsatcgskx.html

[S34] C++：遍历 vector
来源：http://hz.316326.xyz/gtnltnhgkx.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.feifeiyinyue.top/gtjibmphib.html

[S35] C++：map
来源：http://hz.hongshengwenyu.top/gtjfgsrnbk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yuanzhike.top/gtvvenqnqj.html

[S36] C++：unordered_map
来源：http://hz.cashguo.top/gtowproomk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tian-w.cn/gtnoinkdzo.html

[S37] C++：set
来源：http://hz.0kj1m.cn/gtvarcsent.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hnqzz.top/gtudhhmacd.html

[S38] C++：排序
来源：http://hz.pengpengdd.cyou/gtmbinrgil.html

std::sort(v.begin(), v.end());
来源：http://hz.yj202588.top/gtgmurksym.html

[S39] C++：自定义比较器排序
来源：http://hz.vqdsnc.cn/gtwbbmnxak.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.aizwys.cn/gtkvtcuate.html

[S40] C++：查找元素
来源：http://hz.yongpay.top/gttgbyjazm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.chenjidiqi.icu/gtnmyszlzh.html

[S41] C++：类与构造函数
来源：http://hz.zhiwuduotai.top/gtzwhlrfer.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.shzxlz.cn/gtgbozfdwu.html

[S42] C++：继承与虚函数
来源：http://hz.cheryme.top/gtxcrxaegm.html

class B : public Base { public: void f() override {} };
来源：http://hz.nanxuanxn.top/gtsotopajv.html

[S43] C++：智能指针
来源：http://hz.jlsjyb.cn/gtfxtpqwvx.html

auto p = std::make_unique<int>(5);
来源：http://hz.hnxiangtu.top/gtzxocponu.html

[S44] C++：引用传参
来源：http://hz.cheryme.top/gtipiywhyv.html

void inc(int &x) { ++x; }
来源：http://hz.yonumen.top/gtedqhrqab.html

[S45] C++：lambda
来源：http://hz.tianlin.xyz/gtnrzxpqql.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.c1oappe.top/gtnzqxtzar.html

[S46] C++：函数模板
来源：http://hz.gaohongyu789.top/gtbqdbfgmt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ybcxt.top/gtlxruocez.html

[S47] C++：结构化绑定遍历
来源：http://hz.dianchejie.cn/gteogdttjq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ehwqpu.com/gtsxlbbewj.html

[S48] C++：逐行读文件
来源：http://hz.chenlongwang.top/gtbrqxhqvm.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.daria6918.cn/gtwaejptki.html

while (std::getline(in, line)) { }
来源：http://hz.jianghu66.top/gtnzganies.html

[S49] C++：写文件
来源：http://hz.0kj1m.cn/gthfslkyya.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.cashguo.top/gtyajjeqpj.html

[S50] C++：格式化数字
来源：http://hz.hysaishi.cn/gtkoeffflm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.52xcode.cn/gtmjaddcgu.html

[S51] C++：显式类型转换
来源：http://hz.hnxiangtu.top/gtqsqfpgrt.html

static_cast<double>(a) / b
来源：http://hz.0kj1m.cn/gtnvxzgwos.html

[S52] C++：const 与 noexcept
来源：http://hz.haohaochexian.top/gtjkljmiuw.html

int size() const noexcept { return n_; }
来源：http://hz.aibaodan.cn/gteugttbvg.html

[S53] C++：移动语义
来源：http://hz.zycfv.cn/gtbppmiowu.html

std::vector<int> w = std::move(v);
来源：http://hz.hongshengwenyu.top/gthwojufmn.html

[S54] C++：异常处理
来源：http://hz.ybcxt.top/gtmbnygtsg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.sweek.top/gtkckclpkn.html

[S55] C++：结构化绑定
来源：http://hz.jlsjyb.cn/gtkzmtvxmp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.fzhhl.top/gtnrjlkxtm.html

[S56] C++：optional
来源：http://hz.jlsjyb.cn/gtqvcztlxk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hongshengwenyu.top/gtfgntltad.html

[S57] C++：编译期常量
来源：http://hz.sysykeji.top/gtxuylgxto.html

constexpr int N = 10;
来源：http://hz.cdnleiting.top/gtssqwvmel.html

[S58] C++：命名空间
来源：http://hz.yanxiufei.cn/gtwwjwtcuh.html

namespace ns { int f() { return 1; } }
来源：http://hz.cheryme.top/gtpnphtpgq.html

[S59] C++：静态断言
来源：http://hz.zycfv.cn/gtqbuqgsvs.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.sxryk.cn/gtzymacipp.html

[S60] C++：遍历并删除元素
来源：http://hz.316326.xyz/gtjpobjlcz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.shanyushiyangkeji.top/gtryvecfun.html

================================================================================
来源：http://hz.zhengqikj.top/gtygavhkkt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.guowangkeji.top/gtpguxtoyo.html

================================================================================
来源：http://hz.hammf.cn/gtnkgdomcg.html

[T01] Kotlin：Hello World
来源：http://hz.xuanzx.com/gtptvmboco.html

println("Hello")
来源：http://hz.shanyushiyangtech.top/gttbqabawt.html

[T02] Kotlin：变量
来源：http://hz.yj202588.top/gtbglbfucp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.aibaodan.cn/gtugvjrphg.html

[T03] Kotlin：字符串模板
来源：http://hz.shuidangran.top/gtdbuavyre.html

"值: $b"
来源：http://hz.svipenyu.cn/gticshptvj.html

[T04] Kotlin：空安全
来源：http://hz.ybcxt.top/gtopfmanqi.html

val n: String? = null;  n?.length
来源：http://hz.iojbl.cn/gtdkotqsjl.html

[T05] Kotlin：when 表达式
来源：http://hz.jyoumei.cn/gtaqgpbrse.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yj20258888.top/gtotrudzqj.html

[T06] Kotlin：集合映射
来源：http://hz.yj20258.top/gtxmtylknw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.xuanzx.com/gtzfsrhslf.html

[T07] Kotlin：集合过滤
来源：http://hz.hongshengwenyu.top/gtfnrotwgs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.pengpengdd.cyou/gtgewqkchp.html

[T08] Kotlin：数据类
来源：http://hz.9152youxi.cn/gtlzvhiumx.html

data class User(val name: String, val age: Int)
来源：http://hz.zdqjudy.top/gtvjwyjzcf.html

[T09] Kotlin：扩展函数
来源：http://hz.cheryme.top/gtjozbkunw.html

fun String.exclaim() = this + "!"
来源：http://hz.ybcxt.top/gtcvzylowm.html

[T10] Kotlin：默认参数
来源：http://hz.jinqigufen.top/gtfdgvdlqp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.c1oappe.top/gtjccfgccb.html

[T11] Kotlin：协程
来源：http://hz.zhiwuduotai.top/gtgmcacsld.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yonumen.top/gtctcjcnwc.html

[T12] Kotlin：解构声明
来源：http://hz.gotoacloud.top/gtmvopcrpm.html

val (a, b) = Pair(1, 2)
来源：http://hz.cqqwz.cn/gtjsxkvlqy.html

[T13] Kotlin：只读 Map
来源：http://hz.jyoumei.cn/gteznhixyk.html

val m = mapOf("a" to 1)
来源：http://hz.gogol.net.cn/gtedrfdxwc.html

[T14] Kotlin：循环
来源：http://hz.ydjk.org.cn/gtylkxjusm.html

for (i in 1..10) println(i)
来源：http://hz.ppjwa.cn/gtncxfksuz.html

[T15] Kotlin：接口
来源：http://hz.fzhhl.top/gtpnpcpmqr.html

interface Shape { fun area(): Double }
来源：http://hz.chenzaomai.com/gtlhlasrmx.html

[T16] Swift：Hello World
来源：http://hz.nanxinkj.top/gthvxsnbjq.html

print("Hello")
来源：http://hz.316326.xyz/gtbhdvyxxm.html

[T17] Swift：变量与常量
来源：http://hz.zhaomingkeji.xyz/gtsatfimbz.html

var a = 1;  let b = 2
来源：http://hz.nanxuanxn.top/gtrmmoskta.html

[T18] Swift：字符串插值
来源：http://hz.zhoulong.xyz/gtsjrwppsc.html

"值: \(b)"
来源：http://hz.vqdsnc.cn/gtgrmqbtyt.html

[T19] Swift：可选绑定
来源：http://hz.guowangkeji.top/gtywkjehle.html

if let n = opt { print(n) }
来源：http://hz.xuetiantiany.cn/gtvqedhlge.html

[T20] Swift：数组操作
来源：http://hz.yueranfly.top/gtjrqflybr.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.andypj.xyz/gtvhqzyvnk.html

[T21] Swift：遍历
来源：http://hz.havefunace.top/gtkdzildyx.html

for x in a { print(x) }
来源：http://hz.cheryme.top/gtbsibxwqs.html

[T22] Swift：字典
来源：http://hz.shuidangran.top/gtzkvtyrbx.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.sweek.top/gtwjbugsiw.html

[T23] Swift：函数
来源：http://hz.cdnleiting.top/gtzikaqfvb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.tanke756.top/gtlbsvxghb.html

[T24] Swift：闭包
来源：http://hz.quarkkingdee.top/gtbdphbjox.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.hywenlv.cn/gtadehktln.html

[T25] Swift：结构体
来源：http://hz.vqdsnc.cn/gtuzjjwpku.html

struct P { var x: Int }
来源：http://hz.wangshuangyany.cn/gtvebcyndb.html

[T26] Swift：类与重写
来源：http://hz.yanxiufei.cn/gthuhyqxhf.html

class A: Base { override func f() {} }
来源：http://hz.jinyuanbaomall.cn/gtomslfvbg.html

[T27] Swift：错误处理
来源：http://hz.sysykeji.top/gtvqmzxgka.html

do { try f() } catch { print(error) }
来源：http://hz.bjfxy.top/gtnntoitex.html

[T28] Swift：枚举
来源：http://hz.cucudq.cn/gtfvvdxogc.html

enum Color { case red, green }
来源：http://hz.ehwqpu.com/gtcpvucuaj.html

[T29] Swift：guard 提前返回
来源：http://hz.tian-w.cn/gtdvrwzpzg.html

guard let x = opt else { return }
来源：http://hz.shzxlz.cn/gtlodtwmra.html

[T30] Swift：协议
来源：http://hz.fzhhl.top/gtsiatlfzv.html

protocol Shape { func area() -> Double }
来源：http://hz.jlsjyb.cn/gtgedfxcbn.html

[T31] Lua：Hello World
来源：http://hz.aizwys.cn/gtuklmuecf.html

print("Hello")
来源：http://hz.gaohongyu789.top/gtpfnwjesh.html

[T32] Lua：局部变量
来源：http://hz.zhixingplan.top/gtseplaxve.html

local a = 1
来源：http://hz.fzhhl.top/gtwjmckcdc.html

[T33] Lua：表（数组）
来源：http://hz.shzxlz.cn/gtjhqpqvzk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.hysaishi.cn/gtjnzkilqt.html

[T34] Lua：遍历表
来源：http://hz.hongshengwenyu.top/gtyytwnqng.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.316326.xyz/gtjdtvpnda.html

[T35] Lua：字典表
来源：http://hz.daria6918.cn/gtiieczfke.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jiagoushi.top/gtrcqetjqr.html

[T36] Lua：函数
来源：http://hz.jinqigfzy.top/gtldsduwmr.html

function add(a, b) return a + b end
来源：http://hz.smart0.xyz/gtdognhpce.html

[T37] Lua：字符串拼接
来源：http://hz.hammf.cn/gtilgcywwj.html

"a" .. "b"
来源：http://hz.hfpthk.cn/gtgrwhabeo.html

[T38] Lua：条件
来源：http://hz.guowangkeji.top/gteyfxpovz.html

if x > 0 then print("正") end
来源：http://hz.hnqzz.top/gtgoprgrsi.html

[T39] Lua：模式匹配
来源：http://hz.yangfankeji.com/gtnofnjvvp.html

string.find(s, "%d+")
来源：http://hz.chenzaomai.com/gtdnxqqkac.html

[T40] Lua：元表
来源：http://hz.yuanzhike.top/gtsoournej.html

setmetatable({}, { __index = base })
来源：http://hz.cdnleiting.top/gtqzdxpgxd.html

[T41] Perl：Hello World
来源：http://hz.hysaishi.cn/gtmnysuvte.html

print "Hello\n";
来源：http://hz.wangshuangyany.cn/gtpmdxgbsb.html

[T42] Perl：变量类型
来源：http://hz.hnxiangtu.top/gtdadhvign.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.bjfxy.top/gtviegyvug.html

[T43] Perl：字符串插值
来源：http://hz.hammf.cn/gtemjenbqo.html

"值: $a"
来源：http://hz.gotoacloud.top/gtajjeutmu.html

[T44] Perl：条件
来源：http://hz.xinyue.icu/gtwzscjmis.html

if ($a > 0) { print "正"; }
来源：http://hz.wangshuangyany.cn/gtxtiiphxs.html

[T45] Perl：数组遍历
来源：http://hz.jqgufenzy.top/gtcefwexba.html

for my $x (@arr) { print $x; }
来源：http://hz.gaohongyu789.top/gtzjkizzhe.html

[T46] Perl：哈希操作
来源：http://hz.fzhhl.top/gtqhbdxdph.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jqgfzy.top/gtwgkvxgxy.html

[T47] Perl：正则捕获
来源：http://hz.daria6918.cn/gtkhcmjqqh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jqgufenzy.top/gtngvrqkbh.html

[T48] Perl：正则替换
来源：http://hz.smart0.xyz/gtjoyogbke.html

$s =~ s/old/new/g;
来源：http://hz.xuanzx.com/gtiuahgbwf.html

[T49] Perl：函数
来源：http://hz.jqgufenzy.top/gtjwisrhql.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.guowangkeji.top/gtdeossthn.html

[T50] Perl：逐行读文件
来源：http://hz.wangshuangyany.cn/gtvibzingb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.zhijiandao.cn/gtllohkynf.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jinyuanbaomall.cn/gtzgofmqxj.html

[T51] Scala：Hello World
来源：http://hz.yuanzhike.top/gtxnjfjzbd.html

println("Hello")
来源：http://hz.gogol.net.cn/gtiwrtiksj.html

[T52] Scala：变量
来源：http://hz.jlsjyb.cn/gtucffhuhw.html

val a = 1;  var b = 2
来源：http://hz.zhongyouzk.top/gtpdohmeii.html

[T53] Scala：字符串插值
来源：http://hz.dianchejie.cn/gtxiuiehmg.html

s"值: $b"
来源：http://hz.tianlin.xyz/gttorpsrvd.html

[T54] Scala：集合映射
来源：http://hz.sxryk.cn/gtagfqztzn.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.gzhubu.top/gtgvucbvza.html

[T55] Scala：集合过滤
来源：http://hz.shanyushiyangkeji.top/gtfotxzbca.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.fengsongda.top/gtvmupxqww.html

[T56] Scala：样例类
来源：http://hz.dashuyun.cn/gtqzbmrglt.html

case class User(name: String, age: Int)
来源：http://hz.smart0.xyz/gtuxgtpnay.html

[T57] Scala：模式匹配
来源：http://hz.zycfv.cn/gtlinyhrtv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.jianghu66.top/gthfqprgfp.html

[T58] Scala：函数定义
来源：http://hz.sysykeji.top/gtcvcrhlpg.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.tianlin.xyz/gtubfhwggd.html

[T59] Scala：循环
来源：http://hz.daria6918.cn/gttpztfvhq.html

for (i <- 1 to 10) println(i)
来源：http://hz.jinyuanbaomall.cn/gtjcqxnuiu.html

[T60] Scala：折叠
来源：http://hz.zhijiandao.cn/gtdieymhhh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.snrcjt.cn/gthnrwozpj.html

================================================================================
来源：http://hz.hnxiangtu.top/gtsexnoowb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhijiandao.cn/gthmnxbopl.html

================================================================================
来源：http://hz.guannengcc.top/gtcojvtlrr.html

[U01] Py：创建虚拟环境
来源：http://hz.daxiang520.top/gtahovbxiq.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.ppjwa.cn/gtmasntfst.html

[U02] Py：导出 / 安装依赖
来源：http://hz.shuidangran.top/gtfbzgxred.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.xingfuxueyuan.xyz/gtaaxfpkbe.html

[U03] Py：加载 .env 配置
来源：http://hz.ehwqpu.com/gtzfvenxzv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jinqigfzy.top/gtmsqeucqp.html

[U04] Py：变量调试打印
来源：http://hz.quarkkingdee.top/gtmvlvedfl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.gogol.net.cn/gtxheyzqwj.html

[U05] Py：列表去重且保序
来源：http://hz.fengsongda.top/gtcbfzvbyn.html

list(dict.fromkeys(arr))
来源：http://hz.0kj1m.cn/gtjaadzemr.html

[U06] Py：合并两个字典
来源：http://hz.shanyushiyangtech.top/gtyhchgtww.html

{**a, **b}
来源：http://hz.zhaomingkeji.xyz/gtsnmfilse.html

[U07] Py：反转字典键值
来源：http://hz.birdmap.top/gtyfmxumcu.html

{v: k for k, v in d.items()}
来源：http://hz.shangyingyoupin.top/gtljxlynqg.html

[U08] Py：展平二维列表
来源：http://hz.jinqigfzy.top/gtbdxbrjmv.html

[y for x in nested for y in x]
来源：http://hz.guannengcc.top/gtfvdhlilq.html

[U09] Py：字典取最大值的键
来源：http://hz.zhaomingkeji.xyz/gtnsqwexzv.html

max(d, key=d.get)
来源：http://hz.zhoulong.xyz/gtdsuidkge.html

[U10] Py：按值排序字典
来源：http://hz.meibo888.top/gtrihqluql.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.hongshengwenyu.top/gtaixnhoyg.html

[U11] Py：生成器表达式
来源：http://hz.yueranfly.top/gtnjgxvkrl.html

(x * 2 for x in arr)
来源：http://hz.shanyushiyangtech.top/gtzbsbpvct.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.svipenyu.cn/gtxjfeuprm.html

Counter(arr).most_common(3)
来源：http://hz.gaohongyu789.top/gtlzrzsyam.html

[U13] Py：固定长度队列
来源：http://hz.cheryme.top/gtminbxhtg.html

deque(maxlen=10)
来源：http://hz.wangdashe.top/gtvemwwjae.html

[U14] Py：分组收集到列表
来源：http://hz.zycfv.cn/gtdoumxvea.html

defaultdict(list)
来源：http://hz.sweek.top/gttbjdhyrh.html

[U15] Py：高精度计时
来源：http://hz.yj20258888.top/gtrpacbckh.html

t = time.perf_counter()
来源：http://hz.chenjidiqi.icu/gtyoyteikg.html

[U16] Py：命令行参数解析
来源：http://hz.9152youxi.cn/gthrzduehg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.shuidangran.top/gttefhiblx.html

[U17] Py：初始化日志
来源：http://hz.redwolf501.top/gtakdroobg.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.jqgfzy.top/gtzjbfavgi.html

[U18] Py：预编译正则
来源：http://hz.jqgfzy.top/gtryxzgbnk.html

pat = re.compile(r"\d+")
来源：http://hz.hywenlv.cn/gtcndotsbs.html

[U19] Py：正则替换带回调
来源：http://hz.sweek.top/gtmuagypcf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.quarkkingdee.top/gtsnbkrzxa.html

[U20] Py：缓存函数结果
来源：http://hz.gotoacloud.top/gtrbpcbsxs.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yongpay.top/gtlrxbtupp.html

[U21] Py：自定义上下文管理器
来源：http://hz.316326.xyz/gtdkxgzelu.html

@contextlib.contextmanager
来源：http://hz.feifeiyinyue.top/gthoceyurq.html

[U22] Py：矩阵转置
来源：http://hz.zycfv.cn/gtyufcbkox.html

list(zip(*m))
来源：http://hz.feifeiyinyue.top/gtbvrdqytd.html

[U23] Py：分块读取大文件
来源：http://hz.hysaishi.cn/gtcrxuifyu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.haohaochexian.top/gtioawfcbs.html

[U24] Py：路径操作
来源：http://hz.daxiang520.top/gtygqayznn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.bjfxy.top/gtrqzjghuu.html


<!-- 参考信息 -->